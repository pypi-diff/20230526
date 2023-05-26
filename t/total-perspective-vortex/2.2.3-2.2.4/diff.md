# Comparing `tmp/total-perspective-vortex-2.2.3.tar.gz` & `tmp/total-perspective-vortex-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total-perspective-vortex-2.2.3.tar", last modified: Thu May  4 12:52:08 2023, max compression
+gzip compressed data, was "total-perspective-vortex-2.2.4.tar", last modified: Fri May 26 07:54:11 2023, max compression
```

## Comparing `total-perspective-vortex-2.2.3.tar` & `total-perspective-vortex-2.2.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_destinations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_merge_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_params_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_resubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/tpv/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/tpv/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/dryrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/tpv/commands/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/test/mock_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/tpv/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34887 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/tpv/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/rules/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_merge_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_params_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_mapper_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tests/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 07:54:11.000000 total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/dryrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/commands/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/commands/test/mock_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35031 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:11.380432 total-perspective-vortex-2.2.4/tpv/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-26 07:54:01.000000 total-perspective-vortex-2.2.4/tpv/rules/gateway.py
```

### Comparing `total-perspective-vortex-2.2.3/LICENSE` & `total-perspective-vortex-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/PKG-INFO` & `total-perspective-vortex-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.2.3
+Version: 2.2.4
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.2.3/README.md` & `total-perspective-vortex-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/setup.py` & `total-perspective-vortex-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_entity.py` & `total-perspective-vortex-2.2.4/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_basic.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
+import re
 import unittest
 from tpv.rules import gateway
 from tpv.commands.test import mock_galaxy
 from galaxy.jobs.mapper import JobMappingException
 
 
 class TestMapperBasic(unittest.TestCase):
 
     @staticmethod
-    def _map_to_destination(tool):
+    def _map_to_destination(tool, tpv_config_path=None):
         galaxy_app = mock_galaxy.App(job_conf=os.path.join(os.path.dirname(__file__), 'fixtures/job_conf.yml'))
         job = mock_galaxy.Job()
         user = mock_galaxy.User('gargravarr', 'fairycake@vortex.org')
-        tpv_config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-basic.yml')
+        tpv_config = tpv_config_path or os.path.join(os.path.dirname(__file__),
+                                                     'fixtures/mapping-basic.yml')
         gateway.ACTIVE_DESTINATION_MAPPER = None
         return gateway.map_tool_to_destination(galaxy_app, job, tool, user, tpv_config_files=[tpv_config])
 
     def test_map_default_tool(self):
         tool = mock_galaxy.Tool('sometool')
         destination = self._map_to_destination(tool)
         self.assertEqual(destination.id, "local")
@@ -42,14 +44,20 @@
         self.assertEqual(destination.id, "k8s_environment")
 
     def test_map_tool_by_regex_mismatch(self):
         tool = mock_galaxy.Tool('regex_t_test')
         destination = self._map_to_destination(tool)
         self.assertEqual(destination.id, "local")
 
+    def test_map_tool_with_invalid_regex(self):
+        tool = mock_galaxy.Tool('sometool')
+        config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-invalid-regex.yml')
+        with self.assertRaisesRegex(re.error, "bad escape"):
+            self._map_to_destination(tool, tpv_config_path=config)
+
     def test_map_abstract_tool_should_fail(self):
         tool = mock_galaxy.Tool('my_abstract_tool')
         with self.assertRaisesRegex(JobMappingException, "This entity is abstract and cannot be mapped"):
             self._map_to_destination(tool)
 
     def test_map_concrete_descendant_should_succeed(self):
         tool = mock_galaxy.Tool('my_concrete_tool')
```

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_context.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_context.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_destinations.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_destinations.py`

 * *Files 10% similar despite different names*

```diff
@@ -128,59 +128,80 @@
         config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-destinations.yml')
 
         # an intermediate file size should compute correct values
         datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=12 * 1024 ** 3))]
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "my_concrete_destination")
 
-    def test_min_accepted_cpus_honoured(self):
+    def test_accepted_cpus_honoured(self):
         user = mock_galaxy.User('toolmatchuser', 'toolmatchuser@vortex.org')
         config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-destinations.yml')
         datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=12 * 1024 ** 3))]
 
         # First tool should not match
-        tool = mock_galaxy.Tool('tool_for_testing_min_cpu_acceptance_non_match')
+        tool = mock_galaxy.Tool('tool_for_testing_cpu_acceptance_non_match')
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "destination_without_min_cpu_accepted")
 
         # second tool should match the min requirements for the destination
-        tool = mock_galaxy.Tool('tool_for_testing_min_cpu_acceptance_match')
+        tool = mock_galaxy.Tool('tool_for_testing_cpu_acceptance_match')
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "destination_with_min_cpu_accepted")
 
-    def test_min_accepted_gpus_honoured(self):
+        # third tool requesting zero cpus should match either:
+        # - destination_without_min_cpu_accepted
+        # - destination_zero_max_cpu_accepted
+        tool = mock_galaxy.Tool('tool_for_testing_cpu_acceptance_zero')
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
+        self.assertIn(destination.id, {"destination_without_min_cpu_accepted", "destination_zero_max_cpu_accepted"})
+
+    def test_accepted_gpus_honoured(self):
         user = mock_galaxy.User('toolmatchuser', 'toolmatchuser@vortex.org')
         config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-destinations.yml')
         datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=12 * 1024 ** 3))]
 
         # First tool should not match
-        tool = mock_galaxy.Tool('tool_for_testing_min_gpu_acceptance_non_match')
+        tool = mock_galaxy.Tool('tool_for_testing_gpu_acceptance_non_match')
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "destination_without_min_gpu_accepted")
 
         # second tool should match the min requirements for the destination
-        tool = mock_galaxy.Tool('tool_for_testing_min_gpu_acceptance_match')
+        tool = mock_galaxy.Tool('tool_for_testing_gpu_acceptance_match')
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "destination_with_min_gpu_accepted")
 
-    def test_min_accepted_mem_honoured(self):
+        # third tool requesting zero gpus should match either:
+        # - destination_without_min_gpu_accepted
+        # - destination_zero_max_gpu_accepted
+        tool = mock_galaxy.Tool('tool_for_testing_gpu_acceptance_zero')
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
+        self.assertIn(destination.id, {"destination_without_min_gpu_accepted", "destination_zero_max_gpu_accepted"})
+
+    def test_accepted_mem_honoured(self):
         user = mock_galaxy.User('toolmatchuser', 'toolmatchuser@vortex.org')
         config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-destinations.yml')
         datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=12 * 1024 ** 3))]
 
         # First tool should not match
-        tool = mock_galaxy.Tool('tool_for_testing_min_mem_acceptance_non_match')
+        tool = mock_galaxy.Tool('tool_for_testing_mem_acceptance_non_match')
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "destination_without_min_mem_accepted")
 
         # second tool should match the min requirements for the destination
-        tool = mock_galaxy.Tool('tool_for_testing_min_mem_acceptance_match')
+        tool = mock_galaxy.Tool('tool_for_testing_mem_acceptance_match')
         destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
         self.assertEqual(destination.id, "destination_with_min_mem_accepted")
 
+        # third tool requesting zero mem should match either:
+        # - destination_without_min_mem_accepted
+        # - destination_zero_max_mem_accepted
+        tool = mock_galaxy.Tool('tool_for_testing_mem_acceptance_zero')
+        destination = self._map_to_destination(tool, user, datasets, tpv_config_paths=[config])
+        self.assertIn(destination.id, {"destination_without_min_mem_accepted", "destination_zero_max_mem_accepted"})
+
     def test_user_map_to_destination_accepting_offline(self):
         user = mock_galaxy.User('albo', 'pulsar_canberra_user@act.au')
 
         config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-destinations.yml')
 
         tool = mock_galaxy.Tool('toolshed_hifiasm')
         datasets = [mock_galaxy.DatasetAssociation("test", mock_galaxy.Dataset("test.txt", file_size=12 * 1024 ** 3))]
```

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_inheritance.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_inheritance.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_merge_multiple.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_merge_multiple.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_params_specific.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_params_specific.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_rank.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_rank.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_resubmit.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_resubmit.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_role.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_role.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_rules.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_rules.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_sample.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_sample.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_mapper_user.py` & `total-perspective-vortex-2.2.4/tests/test_mapper_user.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_scenarios.py` & `total-perspective-vortex-2.2.4/tests/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tests/test_shell.py` & `total-perspective-vortex-2.2.4/tests/test_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,24 @@
         self.assertTrue(
             "lint failed" in output,
             f"Expected lint to fail but output was: {output}")
         self.assertTrue(
             "oops syntax!" in output,
             f"Expected lint to fail but output was: {output}")
 
+    def test_lint_invalid_regex(self):
+        tpv_config = os.path.join(os.path.dirname(__file__), 'fixtures/linter/linter-invalid-regex.yml')
+        output = self.call_shell_command("tpv", "lint", tpv_config)
+        self.assertTrue(
+            "lint failed" in output,
+            f"Expected lint to fail but output was: {output}")
+        self.assertTrue(
+            "Failed to compile regex: bwa" in output,
+            f"Expected lint to fail but output was: {output}")
+
     def test_lint_no_runner_defined(self):
         tpv_config = os.path.join(os.path.dirname(__file__), 'fixtures/linter/linter-no-runner-defined.yml')
         output = self.call_shell_command("tpv", "-vv", "lint", tpv_config)
         self.assertTrue(
             "lint failed" in output,
             f"Expected lint to fail but output was: {output}")
         self.assertTrue(
```

### Comparing `total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/PKG-INFO` & `total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.2.3
+Version: 2.2.4
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/SOURCES.txt` & `total-perspective-vortex-2.2.4/total_perspective_vortex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tpv/commands/dryrunner.py` & `total-perspective-vortex-2.2.4/tpv/commands/dryrunner.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tpv/commands/formatter.py` & `total-perspective-vortex-2.2.4/tpv/commands/formatter.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tpv/commands/linter.py` & `total-perspective-vortex-2.2.4/tpv/commands/linter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import re
 
 from tpv.core.loader import TPVConfigLoader
 
 log = logging.getLogger(__name__)
 
 
 class TPVLintError(Exception):
@@ -19,15 +20,19 @@
     def lint(self):
         try:
             loader = TPVConfigLoader.from_url_or_path(self.url_or_path)
         except Exception as e:
             log.error(f"Linting failed due to syntax errors in yaml file: {e}")
             raise TPVLintError("Linting failed due to syntax errors in yaml file: ") from e
         default_inherits = loader.global_settings.get('default_inherits')
-        for tool in loader.tools.values():
+        for tool_regex, tool in loader.tools.items():
+            try:
+                re.compile(tool_regex)
+            except re.error:
+                self.errors.append(f"Failed to compile regex: {tool_regex}")
             if default_inherits == tool.id:
                 self.warnings.append(
                     f"The tool named: {default_inherits} is marked globally as the tool to inherit from "
                     "by default. You may want to mark it as abstract if it is not an actual tool and it "
                     "will be excluded from scheduling decisions.")
         for destination in loader.destinations.values():
             if not destination.runner and not destination.abstract:
```

### Comparing `total-perspective-vortex-2.2.3/tpv/commands/shell.py` & `total-perspective-vortex-2.2.4/tpv/commands/shell.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tpv/commands/test/mock_galaxy.py` & `total-perspective-vortex-2.2.4/tpv/commands/test/mock_galaxy.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tpv/core/entities.py` & `total-perspective-vortex-2.2.4/tpv/core/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,25 +638,25 @@
         This is used to check compatibility of a final set of combined tool requirements with its destination.
 
         :param destination:
         :return:
         """
         if self.abstract:
             return False
-        if self.max_accepted_cores and entity.cores and self.max_accepted_cores < entity.cores:
+        if self.max_accepted_cores is not None and entity.cores is not None and self.max_accepted_cores < entity.cores:
             return False
-        if self.max_accepted_mem and entity.mem and self.max_accepted_mem < entity.mem:
+        if self.max_accepted_mem is not None and entity.mem is not None and self.max_accepted_mem < entity.mem:
             return False
-        if self.max_accepted_gpus and entity.gpus and self.max_accepted_gpus < entity.gpus:
+        if self.max_accepted_gpus is not None and entity.gpus is not None and self.max_accepted_gpus < entity.gpus:
             return False
-        if self.min_accepted_cores and entity.cores and self.min_accepted_cores > entity.cores:
+        if self.min_accepted_cores is not None and entity.cores is not None and self.min_accepted_cores > entity.cores:
             return False
-        if self.min_accepted_mem and entity.mem and self.min_accepted_mem > entity.mem:
+        if self.min_accepted_mem is not None and entity.mem is not None and self.min_accepted_mem > entity.mem:
             return False
-        if self.min_accepted_gpus and entity.gpus and self.min_accepted_gpus > entity.gpus:
+        if self.min_accepted_gpus is not None and entity.gpus is not None and self.min_accepted_gpus > entity.gpus:
             return False
         return entity.tpv_tags.match(self.tpv_dest_tags or {})
 
     def score(self, entity):
         """
         Rank this destination against an entity based on how well the tags match
```

### Comparing `total-perspective-vortex-2.2.3/tpv/core/helpers.py` & `total-perspective-vortex-2.2.4/tpv/core/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,18 @@
     # and no require/prefer/accept tags in the exclude_tag_values list
     return (
         all([any(entity.tpv_tags.filter(tag_value=tag_value)) for tag_value in match_tag_values])
         and not any([any(entity.tpv_tags.filter(tag_value=tag_value)) for tag_value in exclude_tag_values])
     )
 
 
+def tool_version_eq(tool, version):
+    return packaging.version.parse(tool.version) == packaging.version.parse(version)
+
+
 def tool_version_lte(tool, version):
     return packaging.version.parse(tool.version) <= packaging.version.parse(version)
 
 
 def tool_version_lt(tool, version):
     return packaging.version.parse(tool.version) < packaging.version.parse(version)
```

### Comparing `total-perspective-vortex-2.2.3/tpv/core/loader.py` & `total-perspective-vortex-2.2.4/tpv/core/loader.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.3/tpv/core/mapper.py` & `total-perspective-vortex-2.2.4/tpv/core/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,19 @@
         self.destinations = loader.destinations
         self.default_inherits = loader.global_settings.get('default_inherits')
         self.global_context = loader.global_settings.get('context')
         self.lookup_tool_regex = functools.lru_cache(maxsize=None)(self.__compile_tool_regex)
         self.inherit_matching_entities = functools.lru_cache(maxsize=None)(self.__inherit_matching_entities)
 
     def __compile_tool_regex(self, key):
-        return re.compile(key)
+        try:
+            return re.compile(key)
+        except re.error:
+            log.error(f"Failed to compile regex: {key}")
+            raise
 
     def _find_entities_matching_id(self, entity_list, entity_name):
         matches = []
         for key in entity_list.keys():
             if self.lookup_tool_regex(key).match(entity_name):
                 match = entity_list[key]
                 if match.abstract:
```

### Comparing `total-perspective-vortex-2.2.3/tpv/rules/gateway.py` & `total-perspective-vortex-2.2.4/tpv/rules/gateway.py`

 * *Files identical despite different names*


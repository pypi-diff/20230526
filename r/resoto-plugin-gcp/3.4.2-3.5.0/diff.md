# Comparing `tmp/resoto-plugin-gcp-3.4.2.tar.gz` & `tmp/resoto-plugin-gcp-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.4.2.tar", last modified: Wed May 10 12:22:56 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.5.0.tar", last modified: Fri May 26 18:24:59 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.4.2.tar` & `resoto-plugin-gcp-3.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:56.670348 resoto-plugin-gcp-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 12:22:56.670348 resoto-plugin-gcp-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:56.666348 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64109 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/gcp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/gcp_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/project_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:56.666348 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   278367 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    41161 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:56.666348 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 12:22:56.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-10 12:22:56.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:56.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 12:22:56.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:56.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 12:22:56.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 12:22:56.000000 resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-10 12:22:56.670348 resoto-plugin-gcp-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:56.670348 resoto-plugin-gcp-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/test_project_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-10 12:19:36.000000 resoto-plugin-gcp-3.4.2/test/test_sqladmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.099375 resoto-plugin-gcp-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-26 18:24:59.099375 resoto-plugin-gcp-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.091375 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/gcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/project_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.095375 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   279213 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49454 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39342 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.095375 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 18:24:59.099375 resoto-plugin-gcp-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.099375 resoto-plugin-gcp-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_project_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_storage.py
```

### Comparing `resoto-plugin-gcp-3.4.2/PKG-INFO` & `resoto-plugin-gcp-3.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto GCP Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import multiprocessing
 from resotolib.args import Namespace
 from concurrent import futures
-from concurrent.futures import Executor
-from typing import Optional, Type, Dict, Any
+from typing import Optional, Dict, Any
 
 import resotolib.proc
 from resotolib.args import ArgumentParser
 from resotolib.baseplugin import BaseCollectorPlugin
+from resotolib.baseresources import Cloud
 from resotolib.config import Config, RunningConfig
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
 from resotolib.logger import log, setup_logger
-from .collector import GCPProjectCollector
+
+# from .collector import GCPProjectCollector
+from .project_collector import GcpProjectCollector
 from .config import GcpConfig
-from .gcp_resources import GCPProject
+
+# from .gcp_resources import GCPProject
+from .resources.base import GcpProject
 from .utils import Credentials
 
 
 class GCPCollectorPlugin(BaseCollectorPlugin):
     """Google Cloud Platform resoto collector plugin.
 
     Gets instantiated in resoto's Processor thread. The collect() method
@@ -36,76 +40,79 @@
         This method kicks off code that adds GCP resources to `self.graph`.
         When collect() finishes the parent thread will take `self.graph` and merge
         it with the global production graph.
         """
         log.debug("plugin: GCP collecting resources")
         assert self.core_feedback, "core_feedback is not set"  # will be set by the outer collector plugin
 
+        cloud = Cloud(id=self.cloud, name="Gcp")
+
         credentials = Credentials.all()
         if len(Config.gcp.project) > 0:
             for project in list(credentials.keys()):
                 if project not in Config.gcp.project:
                     del credentials[project]
 
         if len(credentials) == 0:
             return
 
         max_workers = (
             len(credentials) if len(credentials) < Config.gcp.project_pool_size else Config.gcp.project_pool_size
         )
+        collect_args = {}
         pool_args = {"max_workers": max_workers}
+        pool_executor = futures.ThreadPoolExecutor
         if Config.gcp.fork_process:
-            pool_args["mp_context"] = multiprocessing.get_context("spawn")
-            pool_args["initializer"] = resotolib.proc.initializer
-            pool_executor: Type[Executor] = futures.ProcessPoolExecutor
             collect_args = {
                 "args": ArgumentParser.args,
                 "running_config": Config.running_config,
                 "credentials": credentials if all(v is None for v in credentials.values()) else None,
             }
+            collect_method = collect_in_process
         else:
-            pool_executor = futures.ThreadPoolExecutor
-            collect_args = {}
+            collect_method = self.collect_project
 
         with pool_executor(**pool_args) as executor:
             wait_for = [
                 executor.submit(
-                    self.collect_project,
+                    collect_method,
                     project_id,
                     self.core_feedback.with_context("gcp"),
-                    **collect_args,  # type: ignore
+                    cloud,
+                    **collect_args,
                 )
                 for project_id in credentials.keys()
             ]
             for future in futures.as_completed(wait_for):
                 project_graph = future.result()
                 if not isinstance(project_graph, Graph):
                     log.error(f"Skipping invalid project_graph {type(project_graph)}")
                     continue
                 self.graph.merge(project_graph)
 
     @staticmethod
     def collect_project(
         project_id: str,
         core_feedback: CoreFeedback,
+        cloud: Cloud,
         args: Optional[Namespace] = None,
         running_config: Optional[RunningConfig] = None,
         credentials: Optional[Dict[str, Any]] = None,
     ) -> Optional[Graph]:
         """Collects an individual project.
 
         Is being called in collect() and either run within a thread or a spawned
         process. Depending on whether `gcp.fork_process` was specified or not.
 
         Because the spawned process does not inherit any of our memory or file
         descriptors we are passing the already parsed `args` Namespace() to this
         method.
         """
-        project = GCPProject(id=project_id, tags={})
-        collector_name = f"gcp_{project.id}"
+        project = GcpProject(id=project_id, name=project_id)
+        collector_name = f"gcp_{project_id}"
         resotolib.proc.set_thread_name(collector_name)
 
         if args is not None:
             ArgumentParser.args = args
             setup_logger("resotoworker-gcp", force=True, level=getattr(args, "log_level", None))
         if running_config is not None:
             Config.running_config.apply(running_config)
@@ -114,20 +121,36 @@
             Credentials._credentials = credentials
             Credentials._initialized = True
 
         log.debug(f"Starting new collect process for project {project.dname}")
 
         try:
             core_feedback.progress_done(project_id, 0, 1)
-            gpc = GCPProjectCollector(project)
+            gpc = GcpProjectCollector(Config.gcp, cloud, project, core_feedback)
             gpc.collect()
             core_feedback.progress_done(project_id, 1, 1)
         except Exception as ex:
             core_feedback.with_context("gcp", project_id).error(f"Failed to collect project: {ex}", log)
             return None
         else:
             return gpc.graph
 
     @staticmethod
     def add_config(config: Config) -> None:
         """Called by resoto upon startup to populate the Config store"""
         config.add_config(GcpConfig)
+
+
+def collect_project_proxy(*args, queue: multiprocessing.Queue, **kwargs) -> None:  # type: ignore
+    resotolib.proc.initializer()
+    queue.put(GCPCollectorPlugin.collect_project(*args, **kwargs))
+
+
+def collect_in_process(*args, **kwargs) -> Optional[Graph]:  # type: ignore
+    ctx = multiprocessing.get_context("spawn")
+    queue = ctx.Queue()
+    kwargs["queue"] = queue
+    process = ctx.Process(target=collect_project_proxy, args=args, kwargs=kwargs)
+    process.start()
+    graph = queue.get()
+    process.join()
+    return graph  # type: ignore
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,7 +20,14 @@
         factory=num_default_threads,
         metadata={"description": "GCP project thread/process pool size"},
     )
     fork_process: bool = field(
         default=True,
         metadata={"description": "Fork collector process instead of using threads"},
     )
+
+    def should_collect(self, name: str) -> bool:
+        if self.collect:
+            return name in self.collect
+        if self.no_collect:
+            return name not in self.no_collect
+        return True
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/gcp_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+from copy import deepcopy
 from typing import Optional, List, Dict, Any, Set
 
 from attr import define
 from google.auth.credentials import Credentials
 from googleapiclient import discovery
 
 from resoto_plugin_gcp.utils import MemoryCache
@@ -23,14 +25,51 @@
     version: str
     accessors: List[str]
     action: str
     request_parameter: Dict[str, str]
     request_parameter_in: Set[str]
     response_path: str
     response_regional_sub_path: Optional[str] = None
+    set_label_identifier: str = "resource"
+    get_identifier: Optional[str] = None
+    delete_identifier: Optional[str] = None
+
+    def for_delete(self) -> GcpApiSpec:
+        api_spec = deepcopy(self)
+        api_spec.action = "delete"
+        api_spec.request_parameter[self._delete_identifier] = "{resource}"
+        if self.is_zone_specific:
+            api_spec.request_parameter["zone"] = "{zone}"
+        return api_spec
+
+    def for_get(self) -> GcpApiSpec:
+        api_spec = deepcopy(self)
+        api_spec.action = "get"
+        api_spec.request_parameter[self._get_identifier] = "{resource}"
+        if self.is_zone_specific:
+            api_spec.request_parameter["zone"] = "{zone}"
+        return api_spec
+
+    def for_set_labels(self) -> GcpApiSpec:
+        api_spec = deepcopy(self)
+        api_spec.action = "setLabels"
+        api_spec.request_parameter[self.set_label_identifier] = "{resource}"
+        if self.is_zone_specific:
+            api_spec.request_parameter["zone"] = "{zone}"
+        return api_spec
+
+    @property
+    def _get_identifier(self) -> str:
+        return (
+            self.get_identifier or self.accessors[-1][:-1]
+        )  # Poor persons `singularize(), i.e. ["vpnTunnels"] -> "vpnTunnel"`
+
+    @property
+    def _delete_identifier(self) -> str:
+        return self.delete_identifier or self._get_identifier
 
     @property
     def next_action(self) -> str:
         return self.action + "_next"
 
     @property
     def is_zone_specific(self) -> bool:
@@ -52,23 +91,34 @@
         core_feedback: Optional[CoreFeedback] = None,
     ) -> None:
         self.credentials = credentials
         self.project_id = project_id
         self.region = region
         self.core_feedback = core_feedback
 
+    def delete(self, api_spec: GcpApiSpec, **kwargs: Any) -> Json:
+        return self.call_single(api_spec, None, **kwargs)
+
     def get(self, api_spec: GcpApiSpec, **kwargs: Any) -> Json:
+        return self.call_single(api_spec, None, **kwargs)
+
+    def set_labels(self, api_spec: GcpApiSpec, body: Dict[str, Any], **kwargs: Any) -> Json:
+        return self.call_single(api_spec, body, **kwargs)
+
+    def call_single(self, api_spec: GcpApiSpec, body: Optional[Any] = None, **kwargs: Any) -> Json:
         client = _discovery_function(
             api_spec.service, api_spec.version, credentials=self.credentials, cache=MemoryCache()
         )
         executor = client
         for accessor in api_spec.accessors:
             executor = getattr(executor, accessor)()
         params_map = {**{"project": self.project_id, "region": self.region}, **kwargs}
         params = {k: v.format_map(params_map) for k, v in api_spec.request_parameter.items()}
+        if body:
+            params.update({"body": body})
         request = getattr(executor, api_spec.action)(**params)
         result: Json = request.execute()
         return result
 
     def list(self, api_spec: GcpApiSpec, **kwargs: Any) -> List[Json]:
         # todo add caching
         client = _discovery_function(
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/project_collector.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/project_collector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from concurrent.futures import ThreadPoolExecutor
 import logging
-from queue import Queue
 from typing import Type, List
 
-from resoto_plugin_gcp import GcpConfig, Credentials
-from resoto_plugin_gcp.resources import compute, container, billing, sqladmin
+from resoto_plugin_gcp.config import GcpConfig
+from resoto_plugin_gcp.utils import Credentials
+from resoto_plugin_gcp.resources import compute, container, billing, sqladmin, storage
 from resoto_plugin_gcp.resources.base import GcpResource, GcpProject, ExecutorQueue, GraphBuilder, GcpRegion, GcpZone
 from resotolib.baseresources import Cloud
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
 
 log = logging.getLogger("resoto.plugins.gcp")
 all_resources: List[Type[GcpResource]] = (
-    compute.resources + container.resources + billing.resources + sqladmin.resources
+    compute.resources + container.resources + billing.resources + sqladmin.resources + storage.resources
 )
 
 
 class GcpProjectCollector:
     def __init__(self, config: GcpConfig, cloud: Cloud, project: GcpProject, core_feedback: CoreFeedback) -> None:
         self.config = config
         self.cloud = cloud
@@ -29,43 +29,52 @@
         with ThreadPoolExecutor(
             thread_name_prefix=f"gcp_{self.project.id}", max_workers=self.config.project_pool_size
         ) as executor:
             # The shared executor is used to parallelize the collection of resources "as fast as possible"
             # It should only be used in scenarios, where it is safe to do so.
             # This executor is shared between all regions.
             shared_queue = ExecutorQueue(executor, self.project.safe_name)
+            project_global_region = GcpRegion.fallback_global_region(self.project)
             global_builder = GraphBuilder(
-                self.graph, self.cloud, self.project, self.credentials, shared_queue, self.core_feedback
+                self.graph,
+                self.cloud,
+                self.project,
+                self.credentials,
+                shared_queue,
+                self.core_feedback,
+                project_global_region,
             )
+            global_builder.add_node(project_global_region, {})
 
             # fetch available regions and zones
-            self.core_feedback.progress_done(self.project.dname, 0, 1, context=[self.cloud.id])
             log.info(f"[Gcp:{self.project.id}] Collecting project wide resources.")
             GcpRegion.collect_resources(global_builder)
             global_builder.prepare_region_zone_lookup()
             GcpZone.collect_resources(global_builder)
             global_builder.prepare_region_zone_lookup()
 
             # fetch all project level resources
             for resource_class in all_resources:
+                if not self.config.should_collect(resource_class.kind):
+                    continue
                 if resource_class.api_spec and resource_class.api_spec.is_project_level:
                     global_builder.submit_work(resource_class.collect_resources, global_builder)
 
             # fetch all region level resources
             for region in global_builder.resources_of(GcpRegion):
+                if region.name == "global":
+                    continue
                 global_builder.submit_work(self.collect_region, region, global_builder.for_region(region))
 
             global_builder.executor.wait_for_submitted_work()
             # connect nodes
             for node, data in list(self.graph.nodes(data=True)):
                 if isinstance(node, GcpResource):
                     node.connect_in_graph(global_builder, data.get("source", {}))
 
-            self.core_feedback.progress_done(self.project.dname, 1, 1, context=[self.cloud.id])
-
             log.info(f"[GCP:{self.project.id}] Collecting resources done.")
             self.remove_unconnected_nodes()
 
     def remove_unconnected_nodes(self):
         remove_nodes = set()
 
         def rmnodes(cls) -> None:
@@ -74,36 +83,21 @@
                     remove_nodes.add(node)
             for node in remove_nodes:
                 self.graph.remove_node(node)
             log.debug(f"Removing {len(remove_nodes)} unreferenced nodes of type {cls}")
             remove_nodes.clear()
 
         # nodes need to be removed in the correct order
-        rmnodes((compute.GcpMachineType, compute.GcpDiskType))
+        rmnodes((compute.GcpNodeType, compute.GcpMachineType, compute.GcpDiskType, compute.GcpAcceleratorType))
         rmnodes(billing.GcpSku)
         rmnodes(billing.GcpService)
 
     def collect_region(self, region: GcpRegion, regional_builder: GraphBuilder) -> None:
         # fetch all region level resources
         for resource_class in all_resources:
+            if not self.config.should_collect(resource_class.kind):
+                continue
             if resource_class.api_spec and not resource_class.api_spec.is_project_level:
                 log.info(
                     f"Collecting {resource_class.__name__} for project {self.project.id} in region {region.rtdname}"
                 )
                 resource_class.collect_resources(regional_builder)
-
-
-if __name__ == "__main__":
-    # TODO: remove this only here for local testing
-    from google.oauth2.service_account import Credentials as OauthCredentials
-
-    cloud = Cloud(id="Gcp", name="Gcp")
-    project = GcpProject(id="vpc-host-nonprod-320811", name="vpc-host-nonprod-320811")
-    feedback = CoreFeedback("test", "test", "test", Queue())
-    Credentials._credentials[project.id] = OauthCredentials.from_service_account_file(
-        "/Users/anja/.gcp/vpc_host_nonprod.json"
-    )
-    Credentials._initialized = True
-    collector = GcpProjectCollector(GcpConfig(), cloud, project, feedback)
-    collector.collect()
-    for nd in collector.graph.nodes:
-        print(nd)
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,41 @@
 import concurrent
 import logging
 from concurrent.futures import Executor, Future
 from threading import Lock
 from typing import Callable, List, ClassVar, Optional, TypeVar, Type, Any, Dict
 
 from attr import define, field
-from google.auth.credentials import Credentials
+from google.auth.credentials import Credentials as GoogleAuthCredentials
 
 from resoto_plugin_gcp.gcp_client import GcpClient, GcpApiSpec, InternalZoneProp, RegionProp
-from resoto_plugin_gcp.utils import delete_resource, update_label
+from resoto_plugin_gcp.utils import Credentials
 from resotolib.baseresources import BaseResource, BaseAccount, Cloud, EdgeType, BaseRegion, BaseZone, BaseQuota
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph, EdgeKey
 from resotolib.json import from_json as from_js, to_json as to_js
 from resotolib.json_bender import bend, Bender, S, Bend
 from resotolib.types import Json
 
 log = logging.getLogger("resoto.plugins.gcp")
 
 
 T = TypeVar("T")
 
 
+def get_client(resource: BaseResource) -> GcpClient:
+    project = resource.account()
+    assert isinstance(project, GcpProject)
+    return GcpClient(
+        Credentials.get(project.id),
+        project_id=project.id,
+        region=resource.region().name if resource.region() else None,
+    )
+
+
 class CancelOnFirstError(Exception):
     pass
 
 
 @define
 class ExecutorQueue:
     executor: Executor
@@ -88,31 +98,33 @@
 
 class GraphBuilder:
     def __init__(
         self,
         graph: Graph,
         cloud: Cloud,
         project: GcpProject,
-        credentials: Credentials,
+        credentials: GoogleAuthCredentials,
         executor: ExecutorQueue,
         core_feedback: CoreFeedback,
+        fallback_global_region: GcpRegion,
         region: Optional[GcpRegion] = None,
         graph_nodes_access: Optional[Lock] = None,
         graph_edges_access: Optional[Lock] = None,
     ) -> None:
         self.graph = graph
         self.cloud = cloud
         self.region = region
         self.project = project
         self.client = GcpClient(
             credentials, project_id=project.id, region=region.name if region else None, core_feedback=core_feedback
         )
         self.executor = executor
         self.name = f"GCP:{project.name}"
         self.core_feedback = core_feedback
+        self.fallback_global_region = fallback_global_region
         self.region_by_name: Dict[str, GcpRegion] = {}
         self.region_by_zone_name: Dict[str, GcpRegion] = {}
         self.zone_by_name: Dict[str, GcpZone] = {}
         self.graph_nodes_access = graph_nodes_access or Lock()
         self.graph_edges_access = graph_edges_access or Lock()
 
     def submit_work(self, fn: Callable[..., T], *args: Any, **kwargs: Any) -> Future[T]:
@@ -207,16 +219,16 @@
 
         # Fallback to GraphBuilder region, i.e. regional collection
         if self.region is not None:
             node._region = self.region
             self.add_edge(node, node=self.region, reverse=True)
             return
 
-        # Fallback to project, i.e. for non-regional resources
-        self.add_edge(node, node=self.project, reverse=True)
+        # Fallback to global region
+        self.add_edge(node, node=self.fallback_global_region, reverse=True)
         return
 
     def add_edge(
         self,
         from_node: BaseResource,
         edge_type: EdgeType = EdgeType.default,
         reverse: bool = False,
@@ -280,14 +292,15 @@
         return GraphBuilder(
             self.graph,
             self.cloud,
             self.project,
             self.client.credentials,
             self.executor,
             self.core_feedback,
+            self.fallback_global_region,
             region,
             self.graph_nodes_access,
             self.graph_edges_access,
         )
 
 
 @define(eq=False, slots=False)
@@ -298,21 +311,58 @@
 
     description: Optional[str] = None
     deprecation_status: Optional[GcpDeprecationStatus] = None
     link: Optional[str] = None
     label_fingerprint: Optional[str] = None
 
     def delete(self, graph: Graph) -> bool:
-        return delete_resource(self)
+        if not self.api_spec:
+            return False
+        client = get_client(self)
+        client.delete(
+            self.api_spec.for_delete(),
+            zone=self.zone().name,
+            resource=self.name,
+        )
+        return True
 
-    def update_tag(self, key: str, value: str) -> bool:
-        return update_label(self, key, value)
+    def update_tag(self, key: str, value: Optional[str]) -> bool:
+        if not self.api_spec:
+            return False
+        client = get_client(self)
+
+        labels = dict(self.tags)
+        if value is None:
+            if key in labels:
+                del labels[key]
+            else:
+                return False
+        else:
+            labels.update({key: value})
+        try:
+            client.set_labels(
+                self.api_spec.for_set_labels(),
+                body={"labels": labels, "labelFingerprint": self.label_fingerprint},
+                zone=self.zone().name,
+                resource=self.name,
+            )
+        except AttributeError:
+            log.debug(f"resources of type {self.kind} cannot be labeled.")
+            return False
+        # Retrieve updated label fingerprint
+        result = client.get(
+            self.api_spec.for_get(),
+            zone=self.zone().name,
+            resource=self.name,
+        )
+        self.label_fingerprint = result.get("labelFingerprint")
+        return True
 
     def delete_tag(self, key: str) -> bool:
-        return update_label(self, key, None)
+        return self.update_tag(key, None)
 
     def adjust_from_api(self, graph_builder: GraphBuilder, source: Json) -> GcpResource:
         """
         Hook method to adjust the resource before it is added to the graph.
         Default: do not change the resource.
         """
         return self
@@ -421,15 +471,15 @@
         accessors=["regions"],
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "description": S("description"),
         "status": S("status"),
@@ -437,14 +487,18 @@
         "region_supports_pzs": S("supportsPzs"),
     }
     description: Optional[str] = field(default=None)
     status: Optional[str] = field(default=None)
     region_deprecated: Optional[GcpDeprecationStatus] = field(default=None)
     region_supports_pzs: Optional[bool] = field(default=None)
 
+    @classmethod
+    def fallback_global_region(cls: Type[GcpRegion], project: GcpProject) -> GcpRegion:
+        return cls(id="global", tags={}, name="global", account=project)
+
     def post_process(self, graph_builder: GraphBuilder, source: Json) -> None:
         for quota_js in source.get("quotas", []):
             quota = GcpQuota.from_api(quota_js)
             quota._region = self
             graph_builder.add_node(quota, quota_js)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
@@ -463,15 +517,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "description": S("description"),
         "status": S("status"),
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/billing.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         action="list",
         request_parameter={},
         request_parameter_in=set(),
         response_path="billingAccounts",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -59,29 +59,29 @@
         action="list",
         request_parameter={"name": "{name}"},
         request_parameter_in={"name"},
         response_path="projectBillingInfo",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "billing_account_name": S("billingAccountName"),
         "billing_enabled": S("billingEnabled"),
-        "project_id": S("projectId"),
+        "project_billing_info_project_id": S("projectId"),
     }
     billing_account_name: Optional[str] = field(default=None)
     billing_enabled: Optional[bool] = field(default=None)
-    project_id: Optional[str] = field(default=None)
+    project_billing_info_project_id: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpService(GcpResource):
     kind: ClassVar[str] = "gcp_service"
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {"default": ["gcp_sku"]},
@@ -253,29 +253,29 @@
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "category": S("category", default={}) >> Bend(GcpCategory.mapping),
         "geo_taxonomy": S("geoTaxonomy", default={}) >> Bend(GcpGeoTaxonomy.mapping),
-        "pricing_info": S("pricingInfo", default=[]) >> ForallBend(GcpPricingInfo.mapping),
+        "sku_pricing_info": S("pricingInfo", default=[]) >> ForallBend(GcpPricingInfo.mapping),
         "service_provider_name": S("serviceProviderName"),
         "service_regions": S("serviceRegions", default=[]),
         "sku_id": S("skuId"),
     }
     category: Optional[GcpCategory] = field(default=None)
     geo_taxonomy: Optional[GcpGeoTaxonomy] = field(default=None)
-    pricing_info: List[GcpPricingInfo] = field(factory=list)
+    sku_pricing_info: List[GcpPricingInfo] = field(factory=list)
     service_provider_name: Optional[str] = field(default=None)
     service_regions: List[str] = field(factory=list)
     usage_unit_nanos: Optional[int] = field(default=None)
 
     def post_process(self, graph_builder: GraphBuilder, source: Json) -> None:
-        if len(self.pricing_info) > 0:
-            if not (pricing_expression := self.pricing_info[0].pricing_expression):
+        if len(self.sku_pricing_info) > 0:
+            if not (pricing_expression := self.sku_pricing_info[0].pricing_expression):
                 return
 
             tiered_rates = pricing_expression.tiered_rates
             cost = -1
             if len(tiered_rates) == 1:
                 if tiered_rates[0].unit_price and tiered_rates[0].unit_price.nanos:
                     cost = tiered_rates[0].unit_price.nanos
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="acceleratorTypes",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -67,17 +67,18 @@
         version="v1",
         accessors=["addresses"],
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="addresses",
+        get_identifier="address",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -206,19 +207,19 @@
 
 @define(eq=False, slots=False)
 class GcpScalingScheduleStatus:
     kind: ClassVar[str] = "gcp_scaling_schedule_status"
     mapping: ClassVar[Dict[str, Bender]] = {
         "last_start_time": S("lastStartTime"),
         "next_start_time": S("nextStartTime"),
-        "state": S("state"),
+        "scaling_schedule_status_state": S("state"),
     }
     last_start_time: Optional[datetime] = field(default=None)
     next_start_time: Optional[datetime] = field(default=None)
-    state: Optional[str] = field(default=None)
+    scaling_schedule_status_state: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpAutoscalerStatusDetails:
     kind: ClassVar[str] = "gcp_autoscaler_status_details"
     mapping: ClassVar[Dict[str, Bender]] = {"message": S("message"), "type": S("type")}
     message: Optional[str] = field(default=None)
@@ -241,15 +242,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="autoscalers",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -345,22 +346,22 @@
         "name": S("bucketName"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "bucket_name": S("bucketName"),
-        "cdn_policy": S("cdnPolicy", default={}) >> Bend(GcpBackendBucketCdnPolicy.mapping),
+        "backend_bucket_cdn_policy": S("cdnPolicy", default={}) >> Bend(GcpBackendBucketCdnPolicy.mapping),
         "compression_mode": S("compressionMode"),
         "custom_response_headers": S("customResponseHeaders", default=[]),
         "edge_security_policy": S("edgeSecurityPolicy"),
         "enable_cdn": S("enableCdn"),
     }
     bucket_name: Optional[str] = field(default=None)
-    cdn_policy: Optional[GcpBackendBucketCdnPolicy] = field(default=None)
+    backend_bucket_cdn_policy: Optional[GcpBackendBucketCdnPolicy] = field(default=None)
     compression_mode: Optional[str] = field(default=None)
     custom_response_headers: Optional[List[str]] = field(default=None)
     edge_security_policy: Optional[str] = field(default=None)
     enable_cdn: Optional[bool] = field(default=None)
 
 
 @define(eq=False, slots=False)
@@ -649,25 +650,25 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="backendServices",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "affinity_cookie_ttl_sec": S("affinityCookieTtlSec"),
-        "backends": S("backends", default=[]) >> ForallBend(GcpBackend.mapping),
-        "cdn_policy": S("cdnPolicy", default={}) >> Bend(GcpBackendServiceCdnPolicy.mapping),
+        "backend_service_backends": S("backends", default=[]) >> ForallBend(GcpBackend.mapping),
+        "backend_service_cdn_policy": S("cdnPolicy", default={}) >> Bend(GcpBackendServiceCdnPolicy.mapping),
         "circuit_breakers": S("circuitBreakers", default={}) >> Bend(GcpCircuitBreakers.mapping),
         "compression_mode": S("compressionMode"),
         "connection_draining": S("connectionDraining", "drainingTimeoutSec"),
         "connection_tracking_policy": S("connectionTrackingPolicy", default={})
         >> Bend(GcpBackendServiceConnectionTrackingPolicy.mapping),
         "consistent_hash": S("consistentHash", default={}) >> Bend(GcpConsistentHashLoadBalancerSettings.mapping),
         "custom_request_headers": S("customRequestHeaders", default=[]),
@@ -678,31 +679,31 @@
         "fingerprint": S("fingerprint"),
         "health_checks": S("healthChecks", default=[]),
         "iap": S("iap", default={}) >> Bend(GcpBackendServiceIAP.mapping),
         "load_balancing_scheme": S("loadBalancingScheme"),
         "locality_lb_policies": S("localityLbPolicies", default=[])
         >> ForallBend(GcpBackendServiceLocalityLoadBalancingPolicyConfig.mapping),
         "locality_lb_policy": S("localityLbPolicy"),
-        "log_config": S("logConfig", default={}) >> Bend(GcpBackendServiceLogConfig.mapping),
+        "backend_service_log_config": S("logConfig", default={}) >> Bend(GcpBackendServiceLogConfig.mapping),
         "max_stream_duration": S("maxStreamDuration", default={}) >> Bend(GcpDuration.mapping),
         "network": S("network"),
         "outlier_detection": S("outlierDetection", default={}) >> Bend(GcpOutlierDetection.mapping),
         "port": S("port"),
         "port_name": S("portName"),
         "protocol": S("protocol"),
         "security_policy": S("securityPolicy"),
         "security_settings": S("securitySettings", default={}) >> Bend(GcpSecuritySettings.mapping),
         "service_bindings": S("serviceBindings", default=[]),
         "session_affinity": S("sessionAffinity"),
         "subsetting": S("subsetting", "policy"),
         "timeout_sec": S("timeoutSec"),
     }
     affinity_cookie_ttl_sec: Optional[int] = field(default=None)
-    backends: Optional[List[GcpBackend]] = field(default=None)
-    cdn_policy: Optional[GcpBackendServiceCdnPolicy] = field(default=None)
+    backend_service_backends: Optional[List[GcpBackend]] = field(default=None)
+    backend_service_cdn_policy: Optional[GcpBackendServiceCdnPolicy] = field(default=None)
     circuit_breakers: Optional[GcpCircuitBreakers] = field(default=None)
     compression_mode: Optional[str] = field(default=None)
     connection_draining: Optional[int] = field(default=None)
     connection_tracking_policy: Optional[GcpBackendServiceConnectionTrackingPolicy] = field(default=None)
     consistent_hash: Optional[GcpConsistentHashLoadBalancerSettings] = field(default=None)
     custom_request_headers: Optional[List[str]] = field(default=None)
     custom_response_headers: Optional[List[str]] = field(default=None)
@@ -711,15 +712,15 @@
     failover_policy: Optional[GcpBackendServiceFailoverPolicy] = field(default=None)
     fingerprint: Optional[str] = field(default=None)
     health_checks: Optional[List[str]] = field(default=None)
     iap: Optional[GcpBackendServiceIAP] = field(default=None)
     load_balancing_scheme: Optional[str] = field(default=None)
     locality_lb_policies: Optional[List[GcpBackendServiceLocalityLoadBalancingPolicyConfig]] = field(default=None)
     locality_lb_policy: Optional[str] = field(default=None)
-    log_config: Optional[GcpBackendServiceLogConfig] = field(default=None)
+    backend_service_log_config: Optional[GcpBackendServiceLogConfig] = field(default=None)
     max_stream_duration: Optional[GcpDuration] = field(default=None)
     network: Optional[str] = field(default=None)
     outlier_detection: Optional[GcpOutlierDetection] = field(default=None)
     port: Optional[int] = field(default=None)
     port_name: Optional[str] = field(default=None)
     protocol: Optional[str] = field(default=None)
     security_policy: Optional[str] = field(default=None)
@@ -728,15 +729,15 @@
     session_affinity: Optional[str] = field(default=None)
     subsetting: Optional[str] = field(default=None)
     timeout_sec: Optional[int] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         for check in self.health_checks or []:
             builder.dependant_node(self, clazz=health_check_types(), link=check)
-        for backend in self.backends or []:
+        for backend in self.backend_service_backends or []:
             if backend.group:
                 builder.dependant_node(self, link=backend.group)
         if self.network:
             builder.add_edge(self, reverse=True, clazz=GcpNetwork, link=self.network)
 
 
 @define(eq=False, slots=False)
@@ -749,15 +750,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="diskTypes",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -793,15 +794,15 @@
             if sku.category.resource_family != "Storage" or sku.category.usage_type != "OnDemand":
                 return False
             if not sku.category.resource_group == resource_group:
                 return False
 
             if self.name == "pd-balanced" and not sku.description.startswith("Balanced"):
                 return False
-            if self.name != "pd-balanced" and sku.description.startswith("Balanced"):
+            if self.name != "pd-balanced" and "Balanced" in sku.description:
                 return False
             if self.zone().name != "undefined" and sku.description.startswith("Regional"):
                 # Zonal (i.e. not regional?) disk_type but regional SKU
                 return False
             if (
                 # Zonal disk_type, but regional SKU and ALSO
                 # not of type pd-balanced
@@ -844,29 +845,29 @@
     resource_manager_tags: Optional[Dict[str, str]] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpDisk(GcpResource, BaseVolume):
     kind: ClassVar[str] = "gcp_disk"
     reference_kinds: ClassVar[ModelReference] = {
-        "predecessors": {"default": ["gcp_disk_type"], "delete": ["gcp_instance"]},
-        "successors": {"default": ["gcp_instance"]},
+        "predecessors": {"default": ["gcp_disk_type", "gcp_instance"]},
+        "successors": {"delete": ["gcp_instance"]},
     }
     api_spec: ClassVar[GcpApiSpec] = GcpApiSpec(
         service="compute",
         version="v1",
         accessors=["disks"],
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="disks",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -875,15 +876,15 @@
         "guest_os_features": S("guestOsFeatures", default=[]) >> ForallBend(S("type")),
         "last_attach_timestamp": S("lastAttachTimestamp"),
         "last_detach_timestamp": S("lastDetachTimestamp"),
         "license_codes": S("licenseCodes", default=[]),
         "licenses": S("licenses", default=[]),
         "location_hint": S("locationHint"),
         "options": S("options"),
-        "params": S("params", default={}) >> Bend(GcpDiskParams.mapping),
+        "disk_params": S("params", default={}) >> Bend(GcpDiskParams.mapping),
         "physical_block_size_bytes": S("physicalBlockSizeBytes"),
         "provisioned_iops": S("provisionedIops"),
         "replica_zones": S("replicaZones", default=[]),
         "resource_policies": S("resourcePolicies", default=[]),
         "satisfies_pzs": S("satisfiesPzs"),
         "size_gb": S("sizeGb"),
         "source_disk": S("sourceDisk"),
@@ -923,15 +924,15 @@
     guest_os_features: Optional[List[str]] = field(default=None)
     last_attach_timestamp: Optional[datetime] = field(default=None)
     last_detach_timestamp: Optional[datetime] = field(default=None)
     license_codes: Optional[List[str]] = field(default=None)
     licenses: Optional[List[str]] = field(default=None)
     location_hint: Optional[str] = field(default=None)
     options: Optional[str] = field(default=None)
-    params: Optional[GcpDiskParams] = field(default=None)
+    disk_params: Optional[GcpDiskParams] = field(default=None)
     physical_block_size_bytes: Optional[str] = field(default=None)
     provisioned_iops: Optional[str] = field(default=None)
     replica_zones: Optional[List[str]] = field(default=None)
     resource_policies: Optional[List[str]] = field(default=None)
     satisfies_pzs: Optional[bool] = field(default=None)
     size_gb: Optional[str] = field(default=None)
     source_disk: Optional[str] = field(default=None)
@@ -945,15 +946,15 @@
     source_storage_object: Optional[str] = field(default=None)
     status: Optional[str] = field(default=None)
     type: Optional[str] = field(default=None)
     users: Optional[List[str]] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         for user in source.get("users", []):
-            builder.dependant_node(self, clazz=GcpInstance, link=user)
+            builder.dependant_node(self, clazz=GcpInstance, link=user, reverse=True, delete_same_as_default=False)
         builder.add_edge(self, reverse=True, clazz=GcpDiskType, link=self.volume_type)
 
 
 @define(eq=False, slots=False)
 class GcpExternalVpnGatewayInterface:
     kind: ClassVar[str] = "gcp_external_vpn_gateway_interface"
     mapping: ClassVar[Dict[str, Bender]] = {"id": S("id"), "ip_address": S("ipAddress")}
@@ -971,26 +972,27 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
-        "interfaces": S("interfaces", default=[]) >> ForallBend(GcpExternalVpnGatewayInterface.mapping),
+        "external_vpn_gateway_interfaces": S("interfaces", default=[])
+        >> ForallBend(GcpExternalVpnGatewayInterface.mapping),
         "redundancy_type": S("redundancyType"),
     }
-    interfaces: Optional[List[GcpExternalVpnGatewayInterface]] = field(default=None)
+    external_vpn_gateway_interfaces: Optional[List[GcpExternalVpnGatewayInterface]] = field(default=None)
     redundancy_type: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpFirewallPolicyAssociation:
     kind: ClassVar[str] = "gcp_firewall_policy_association"
     mapping: ClassVar[Dict[str, Bender]] = {
@@ -1014,17 +1016,17 @@
     ip_protocol: Optional[str] = field(default=None)
     ports: Optional[List[str]] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpFirewallPolicyRuleSecureTag:
     kind: ClassVar[str] = "gcp_firewall_policy_rule_secure_tag"
-    mapping: ClassVar[Dict[str, Bender]] = {"name": S("name"), "state": S("state")}
+    mapping: ClassVar[Dict[str, Bender]] = {"name": S("name"), "firewall_policy_rule_secure_tag_state": S("state")}
     name: Optional[str] = field(default=None)
-    state: Optional[str] = field(default=None)
+    firewall_policy_rule_secure_tag_state: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpFirewallPolicyRuleMatcher:
     kind: ClassVar[str] = "gcp_firewall_policy_rule_matcher"
     mapping: ClassVar[Dict[str, Bender]] = {
         "dest_ip_ranges": S("destIpRanges", default=[]),
@@ -1082,42 +1084,42 @@
         action="list",
         request_parameter={},
         request_parameter_in=set(),
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "associations": S("associations", default=[]) >> ForallBend(GcpFirewallPolicyAssociation.mapping),
         "display_name": S("displayName"),
         "fingerprint": S("fingerprint"),
         "parent": S("parent"),
         "rule_tuple_count": S("ruleTupleCount"),
-        "rules": S("rules", default=[]) >> ForallBend(GcpFirewallPolicyRule.mapping),
+        "firewall_policy_rules": S("rules", default=[]) >> ForallBend(GcpFirewallPolicyRule.mapping),
         "self_link_with_id": S("selfLinkWithId"),
         "short_name": S("shortName"),
     }
     associations: Optional[List[GcpFirewallPolicyAssociation]] = field(default=None)
     display_name: Optional[str] = field(default=None)
     fingerprint: Optional[str] = field(default=None)
     parent: Optional[str] = field(default=None)
     rule_tuple_count: Optional[int] = field(default=None)
-    rules: Optional[List[GcpFirewallPolicyRule]] = field(default=None)
+    firewall_policy_rules: Optional[List[GcpFirewallPolicyRule]] = field(default=None)
     self_link_with_id: Optional[str] = field(default=None)
     short_name: Optional[str] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
-        for rule in self.rules or []:
+        for rule in self.firewall_policy_rules or []:
             for resource in rule.target_resources or []:
                 builder.add_edge(self, clazz=GcpNetwork, link=resource)
 
 
 @define(eq=False, slots=False)
 class GcpAllowed:
     kind: ClassVar[str] = "gcp_allowed"
@@ -1153,42 +1155,42 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "allowed": S("allowed", default=[]) >> ForallBend(GcpAllowed.mapping),
         "denied": S("denied", default=[]) >> ForallBend(GcpDenied.mapping),
         "destination_ranges": S("destinationRanges", default=[]),
         "direction": S("direction"),
         "disabled": S("disabled"),
-        "log_config": S("logConfig", default={}) >> Bend(GcpFirewallLogConfig.mapping),
+        "firewall_log_config": S("logConfig", default={}) >> Bend(GcpFirewallLogConfig.mapping),
         "network": S("network"),
         "priority": S("priority"),
         "source_ranges": S("sourceRanges", default=[]),
         "source_service_accounts": S("sourceServiceAccounts", default=[]),
         "source_tags": S("sourceTags", default=[]),
         "target_service_accounts": S("targetServiceAccounts", default=[]),
         "target_tags": S("targetTags", default=[]),
     }
     allowed: Optional[List[GcpAllowed]] = field(default=None)
     denied: Optional[List[GcpDenied]] = field(default=None)
     destination_ranges: Optional[List[str]] = field(default=None)
     direction: Optional[str] = field(default=None)
     disabled: Optional[bool] = field(default=None)
-    log_config: Optional[GcpFirewallLogConfig] = field(default=None)
+    firewall_log_config: Optional[GcpFirewallLogConfig] = field(default=None)
     network: Optional[str] = field(default=None)
     priority: Optional[int] = field(default=None)
     source_ranges: Optional[List[str]] = field(default=None)
     source_service_accounts: Optional[List[str]] = field(default=None)
     source_tags: Optional[List[str]] = field(default=None)
     target_service_accounts: Optional[List[str]] = field(default=None)
     target_tags: Optional[List[str]] = field(default=None)
@@ -1255,15 +1257,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="forwardingRules",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -1382,15 +1384,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="networkEndpointGroups",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -1531,15 +1533,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="operations",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -1613,15 +1615,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="publicDelegatedPrefixes",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -1674,16 +1676,16 @@
     port_specification: Optional[str] = field(default=None)
     proxy_header: Optional[str] = field(default=None)
     request_path: Optional[str] = field(default=None)
     response: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class GcpHTTPHealthCheck:
-    kind: ClassVar[str] = "gcp_http_health_check"
+class GcpHTTPHealthCheckSpec:
+    kind: ClassVar[str] = "gcp_http_health_check_spec"
     mapping: ClassVar[Dict[str, Bender]] = {
         "host": S("host"),
         "port": S("port"),
         "port_name": S("portName"),
         "port_specification": S("portSpecification"),
         "proxy_header": S("proxyHeader"),
         "request_path": S("requestPath"),
@@ -1695,16 +1697,16 @@
     port_specification: Optional[str] = field(default=None)
     proxy_header: Optional[str] = field(default=None)
     request_path: Optional[str] = field(default=None)
     response: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class GcpHTTPSHealthCheck:
-    kind: ClassVar[str] = "gcp_https_health_check"
+class GcpHTTPSHealthCheckSpec:
+    kind: ClassVar[str] = "gcp_https_health_check_spec"
     mapping: ClassVar[Dict[str, Bender]] = {
         "host": S("host"),
         "port": S("port"),
         "port_name": S("portName"),
         "port_specification": S("portSpecification"),
         "proxy_header": S("proxyHeader"),
         "request_path": S("requestPath"),
@@ -1767,42 +1769,42 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="healthChecks",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "check_interval_sec": S("checkIntervalSec"),
         "grpc_health_check": S("grpcHealthCheck", default={}) >> Bend(GcpGRPCHealthCheck.mapping),
         "healthy_threshold": S("healthyThreshold"),
         "http2_health_check": S("http2HealthCheck", default={}) >> Bend(GcpHTTP2HealthCheck.mapping),
-        "http_health_check": S("httpHealthCheck", default={}) >> Bend(GcpHTTPHealthCheck.mapping),
-        "https_health_check": S("httpsHealthCheck", default={}) >> Bend(GcpHTTPSHealthCheck.mapping),
-        "log_config": S("logConfig", "enable"),
+        "http_health_check": S("httpHealthCheck", default={}) >> Bend(GcpHTTPHealthCheckSpec.mapping),
+        "https_health_check": S("httpsHealthCheck", default={}) >> Bend(GcpHTTPSHealthCheckSpec.mapping),
+        "health_check_log_config": S("logConfig", "enable"),
         "ssl_health_check": S("sslHealthCheck", default={}) >> Bend(GcpSSLHealthCheck.mapping),
         "tcp_health_check": S("tcpHealthCheck", default={}) >> Bend(GcpTCPHealthCheck.mapping),
         "timeout_sec": S("timeoutSec"),
         "type": S("type"),
         "unhealthy_threshold": S("unhealthyThreshold"),
     }
     check_interval_sec: Optional[int] = field(default=None)
     grpc_health_check: Optional[GcpGRPCHealthCheck] = field(default=None)
     healthy_threshold: Optional[int] = field(default=None)
     http2_health_check: Optional[GcpHTTP2HealthCheck] = field(default=None)
-    http_health_check: Optional[GcpHTTPHealthCheck] = field(default=None)
-    https_health_check: Optional[GcpHTTPSHealthCheck] = field(default=None)
-    log_config: Optional[bool] = field(default=None)
+    http_health_check: Optional[GcpHTTPHealthCheckSpec] = field(default=None)
+    https_health_check: Optional[GcpHTTPSHealthCheckSpec] = field(default=None)
+    health_check_log_config: Optional[bool] = field(default=None)
     ssl_health_check: Optional[GcpSSLHealthCheck] = field(default=None)
     tcp_health_check: Optional[GcpTCPHealthCheck] = field(default=None)
     timeout_sec: Optional[int] = field(default=None)
     type: Optional[str] = field(default=None)
     unhealthy_threshold: Optional[int] = field(default=None)
 
 
@@ -1816,15 +1818,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -1855,15 +1857,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -1932,15 +1934,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -2068,17 +2070,20 @@
     auto_delete: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpStatefulPolicyPreservedState:
     kind: ClassVar[str] = "gcp_stateful_policy_preserved_state"
     mapping: ClassVar[Dict[str, Bender]] = {
-        "disks": S("disks", default={}) >> MapDict(value_bender=Bend(GcpStatefulPolicyPreservedStateDiskDevice.mapping))
+        "stateful_policy_preserved_state_disks": S("disks", default={})
+        >> MapDict(value_bender=Bend(GcpStatefulPolicyPreservedStateDiskDevice.mapping))
     }
-    disks: Optional[Dict[str, GcpStatefulPolicyPreservedStateDiskDevice]] = field(default=None)
+    stateful_policy_preserved_state_disks: Optional[Dict[str, GcpStatefulPolicyPreservedStateDiskDevice]] = field(
+        default=None
+    )
 
 
 @define(eq=False, slots=False)
 class GcpStatefulPolicy:
     kind: ClassVar[str] = "gcp_stateful_policy"
     mapping: ClassVar[Dict[str, Bender]] = {
         "preserved_state": S("preservedState", default={}) >> Bend(GcpStatefulPolicyPreservedState.mapping)
@@ -2163,15 +2168,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="instanceGroupManagers",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -2182,15 +2187,15 @@
         "distribution_policy": S("distributionPolicy", default={}) >> Bend(GcpDistributionPolicy.mapping),
         "fingerprint": S("fingerprint"),
         "instance_group": S("instanceGroup"),
         "instance_template": S("instanceTemplate"),
         "list_managed_instances_results": S("listManagedInstancesResults"),
         "named_ports": S("namedPorts", default=[]) >> ForallBend(GcpNamedPort.mapping),
         "stateful_policy": S("statefulPolicy", default={}) >> Bend(GcpStatefulPolicy.mapping),
-        "status": S("status", default={}) >> Bend(GcpInstanceGroupManagerStatus.mapping),
+        "instance_group_manager_status": S("status", default={}) >> Bend(GcpInstanceGroupManagerStatus.mapping),
         "target_pools": S("targetPools", default=[]),
         "target_size": S("targetSize"),
         "update_policy": S("updatePolicy", default={}) >> Bend(GcpInstanceGroupManagerUpdatePolicy.mapping),
         "versions": S("versions", default=[]) >> ForallBend(GcpInstanceGroupManagerVersion.mapping),
     }
     auto_healing_policies: Optional[List[GcpInstanceGroupManagerAutoHealingPolicy]] = field(default=None)
     base_instance_name: Optional[str] = field(default=None)
@@ -2198,15 +2203,15 @@
     distribution_policy: Optional[GcpDistributionPolicy] = field(default=None)
     fingerprint: Optional[str] = field(default=None)
     instance_group: Optional[str] = field(default=None)
     instance_template: Optional[str] = field(default=None)
     list_managed_instances_results: Optional[str] = field(default=None)
     named_ports: Optional[List[GcpNamedPort]] = field(default=None)
     stateful_policy: Optional[GcpStatefulPolicy] = field(default=None)
-    status: Optional[GcpInstanceGroupManagerStatus] = field(default=None)
+    instance_group_manager_status: Optional[GcpInstanceGroupManagerStatus] = field(default=None)
     target_pools: Optional[List[str]] = field(default=None)
     target_size: Optional[int] = field(default=None)
     update_policy: Optional[GcpInstanceGroupManagerUpdatePolicy] = field(default=None)
     versions: Optional[List[GcpInstanceGroupManagerVersion]] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if self.instance_group:
@@ -2235,15 +2240,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="instanceGroups",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -2624,15 +2629,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -2671,17 +2676,18 @@
         version="v1",
         accessors=["instances"],
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="instances",
+        set_label_identifier="instance",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -2701,15 +2707,15 @@
         "last_stop_timestamp": S("lastStopTimestamp"),
         "last_suspended_timestamp": S("lastSuspendedTimestamp"),
         "machine_type": S("machineType"),
         "instance_metadata": S("metadata", default={}) >> Bend(GcpMetadata.mapping),
         "min_cpu_platform": S("minCpuPlatform"),
         "network_interfaces": S("networkInterfaces", default=[]) >> ForallBend(GcpNetworkInterface.mapping),
         "network_performance_config": S("networkPerformanceConfig", "totalEgressBandwidthTier"),
-        "params": S("params", default={}) >> Bend(GcpInstanceParams.mapping),
+        "instance_params": S("params", default={}) >> Bend(GcpInstanceParams.mapping),
         "private_ipv6_google_access": S("privateIpv6GoogleAccess"),
         "reservation_affinity": S("reservationAffinity", default={}) >> Bend(GcpReservationAffinity.mapping),
         "resource_policies": S("resourcePolicies", default=[]),
         "resource_status": S("resourceStatus", "physicalHost"),
         "satisfies_pzs": S("satisfiesPzs"),
         "scheduling": S("scheduling", default={}) >> Bend(GcpScheduling.mapping),
         "service_accounts": S("serviceAccounts", default=[]) >> ForallBend(GcpServiceAccount.mapping),
@@ -2752,15 +2758,15 @@
     last_stop_timestamp: Optional[datetime] = field(default=None)
     last_suspended_timestamp: Optional[datetime] = field(default=None)
     machine_type: Optional[str] = field(default=None)
     instance_metadata: Optional[GcpMetadata] = field(default=None)
     min_cpu_platform: Optional[str] = field(default=None)
     network_interfaces: Optional[List[GcpNetworkInterface]] = field(default=None)
     network_performance_config: Optional[str] = field(default=None)
-    params: Optional[GcpInstanceParams] = field(default=None)
+    instance_params: Optional[GcpInstanceParams] = field(default=None)
     private_ipv6_google_access: Optional[str] = field(default=None)
     reservation_affinity: Optional[GcpReservationAffinity] = field(default=None)
     resource_policies: Optional[List[str]] = field(default=None)
     resource_status: Optional[str] = field(default=None)
     satisfies_pzs: Optional[bool] = field(default=None)
     scheduling: Optional[GcpScheduling] = field(default=None)
     service_accounts: Optional[List[GcpServiceAccount]] = field(default=None)
@@ -2848,15 +2854,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="interconnectAttachments",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -2881,15 +2887,15 @@
         "pairing_key": S("pairingKey"),
         "partner_asn": S("partnerAsn"),
         "partner_metadata": S("partnerMetadata", default={}) >> Bend(GcpInterconnectAttachmentPartnerMetadata.mapping),
         "private_interconnect_info": S("privateInterconnectInfo", "tag8021q"),
         "router": S("router"),
         "satisfies_pzs": S("satisfiesPzs"),
         "stack_type": S("stackType"),
-        "state": S("state"),
+        "interconnect_attachment_state": S("state"),
         "type": S("type"),
         "vlan_tag8021q": S("vlanTag8021q"),
     }
     admin_enabled: Optional[bool] = field(default=None)
     bandwidth: Optional[str] = field(default=None)
     candidate_ipv6_subnets: Optional[List[str]] = field(default=None)
     candidate_subnets: Optional[List[str]] = field(default=None)
@@ -2910,15 +2916,15 @@
     pairing_key: Optional[str] = field(default=None)
     partner_asn: Optional[str] = field(default=None)
     partner_metadata: Optional[GcpInterconnectAttachmentPartnerMetadata] = field(default=None)
     private_interconnect_info: Optional[int] = field(default=None)
     router: Optional[str] = field(default=None)
     satisfies_pzs: Optional[bool] = field(default=None)
     stack_type: Optional[str] = field(default=None)
-    state: Optional[str] = field(default=None)
+    interconnect_attachment_state: Optional[str] = field(default=None)
     type: Optional[str] = field(default=None)
     vlan_tag8021q: Optional[int] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpInterconnectLocationRegionInfo:
     kind: ClassVar[str] = "gcp_interconnect_location_region_info"
@@ -2942,15 +2948,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -2997,15 +3003,15 @@
         "affected_circuits": S("affectedCircuits", default=[]),
         "description": S("description"),
         "end_time": S("endTime"),
         "issue_type": S("issueType"),
         "name": S("name"),
         "source": S("source"),
         "start_time": S("startTime"),
-        "state": S("state"),
+        "interconnect_outage_notification_state": S("state"),
     }
     affected_circuits: Optional[List[str]] = field(default=None)
     description: Optional[str] = field(default=None)
     end_time: Optional[str] = field(default=None)
     issue_type: Optional[str] = field(default=None)
     name: Optional[str] = field(default=None)
     source: Optional[str] = field(default=None)
@@ -3023,15 +3029,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -3047,15 +3053,15 @@
         "location": S("location"),
         "noc_contact_email": S("nocContactEmail"),
         "operational_status": S("operationalStatus"),
         "peer_ip_address": S("peerIpAddress"),
         "provisioned_link_count": S("provisionedLinkCount"),
         "requested_link_count": S("requestedLinkCount"),
         "satisfies_pzs": S("satisfiesPzs"),
-        "state": S("state"),
+        "interconnect_state": S("state"),
     }
     admin_enabled: Optional[bool] = field(default=None)
     circuit_infos: Optional[List[GcpInterconnectCircuitInfo]] = field(default=None)
     customer_name: Optional[str] = field(default=None)
     expected_outages: Optional[List[GcpInterconnectOutageNotification]] = field(default=None)
     google_ip_address: Optional[str] = field(default=None)
     google_reference_id: Optional[str] = field(default=None)
@@ -3065,15 +3071,15 @@
     location: Optional[str] = field(default=None)
     noc_contact_email: Optional[str] = field(default=None)
     operational_status: Optional[str] = field(default=None)
     peer_ip_address: Optional[str] = field(default=None)
     provisioned_link_count: Optional[int] = field(default=None)
     requested_link_count: Optional[int] = field(default=None)
     satisfies_pzs: Optional[bool] = field(default=None)
-    state: Optional[str] = field(default=None)
+    interconnect_state: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpLicenseResourceRequirements:
     kind: ClassVar[str] = "gcp_license_resource_requirements"
     mapping: ClassVar[Dict[str, Bender]] = {
         "min_guest_cpu_count": S("minGuestCpuCount"),
@@ -3093,15 +3099,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -3182,30 +3188,30 @@
 @define(eq=False, slots=False)
 class GcpSourceInstanceProperties:
     kind: ClassVar[str] = "gcp_source_instance_properties"
     mapping: ClassVar[Dict[str, Bender]] = {
         "can_ip_forward": S("canIpForward"),
         "deletion_protection": S("deletionProtection"),
         "description": S("description"),
-        "disks": S("disks", default=[]) >> ForallBend(GcpSavedAttachedDisk.mapping),
+        "saved_disks": S("disks", default=[]) >> ForallBend(GcpSavedAttachedDisk.mapping),
         "guest_accelerators": S("guestAccelerators", default=[]) >> ForallBend(GcpAcceleratorConfig.mapping),
         "key_revocation_action_type": S("keyRevocationActionType"),
         "labels": S("labels"),
         "machine_type": S("machineType"),
         "metadata": S("metadata", default={}) >> Bend(GcpMetadata.mapping),
         "min_cpu_platform": S("minCpuPlatform"),
         "network_interfaces": S("networkInterfaces", default=[]) >> ForallBend(GcpNetworkInterface.mapping),
         "scheduling": S("scheduling", default={}) >> Bend(GcpScheduling.mapping),
         "service_accounts": S("serviceAccounts", default=[]) >> ForallBend(GcpServiceAccount.mapping),
         "tags": S("tags", default={}) >> Bend(GcpTags.mapping),
     }
     can_ip_forward: Optional[bool] = field(default=None)
     deletion_protection: Optional[bool] = field(default=None)
     description: Optional[str] = field(default=None)
-    disks: Optional[List[GcpSavedAttachedDisk]] = field(default=None)
+    saved_disks: Optional[List[GcpSavedAttachedDisk]] = field(default=None)
     guest_accelerators: Optional[List[GcpAcceleratorConfig]] = field(default=None)
     key_revocation_action_type: Optional[str] = field(default=None)
     labels: Optional[Dict[str, str]] = field(default=None)
     machine_type: Optional[str] = field(default=None)
     metadata: Optional[GcpMetadata] = field(default=None)
     min_cpu_platform: Optional[str] = field(default=None)
     network_interfaces: Optional[List[GcpNetworkInterface]] = field(default=None)
@@ -3229,15 +3235,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -3298,15 +3304,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="machineTypes",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -3339,15 +3345,15 @@
             request_parameter_in={"project", "zone", "machineType"},
         )
         result = builder.client.get(
             api_spec,
             zone=zone,
             machineType=name,
         )
-        result[InternalZoneProp] = zone
+        result[InternalZoneProp] = zone  # `add_node()` picks this up and sets proper zone/region
         machine_type_obj = GcpMachineType.from_api(result)
         builder.add_node(machine_type_obj, result)
 
     def _machine_type_matches_sku_description(self, sku_description: str) -> bool:
         if not self.name:
             return False
         mappings = [
@@ -3438,16 +3444,14 @@
                         ondemand_cost += sku.usage_unit_nanos * ram
                     builder.add_edge(self, reverse=True, node=sku)
 
             if ondemand_cost > 0:
                 self.ondemand_cost = ondemand_cost / 1000000000
             return
 
-        log.debug(f"Unable to determine SKU(s) for {self.rtdname}: {[sku.dname for sku in skus]}")
-
 
 @define(eq=False, slots=False)
 class GcpNetworkEdgeSecurityService(GcpResource):
     kind: ClassVar[str] = "gcp_network_edge_security_service"
     api_spec: ClassVar[GcpApiSpec] = GcpApiSpec(
         service="compute",
         version="v1",
@@ -3455,15 +3459,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="networkEdgeSecurityServices",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -3486,28 +3490,28 @@
         "export_subnet_routes_with_public_ip": S("exportSubnetRoutesWithPublicIp"),
         "import_custom_routes": S("importCustomRoutes"),
         "import_subnet_routes_with_public_ip": S("importSubnetRoutesWithPublicIp"),
         "name": S("name"),
         "network": S("network"),
         "peer_mtu": S("peerMtu"),
         "stack_type": S("stackType"),
-        "state": S("state"),
+        "network_peering_state": S("state"),
         "state_details": S("stateDetails"),
     }
     auto_create_routes: Optional[bool] = field(default=None)
     exchange_subnet_routes: Optional[bool] = field(default=None)
     export_custom_routes: Optional[bool] = field(default=None)
     export_subnet_routes_with_public_ip: Optional[bool] = field(default=None)
     import_custom_routes: Optional[bool] = field(default=None)
     import_subnet_routes_with_public_ip: Optional[bool] = field(default=None)
     name: Optional[str] = field(default=None)
     network: Optional[str] = field(default=None)
     peer_mtu: Optional[int] = field(default=None)
     stack_type: Optional[str] = field(default=None)
-    state: Optional[str] = field(default=None)
+    network_peering_state: Optional[str] = field(default=None)
     state_details: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpNetwork(GcpResource):
     kind: ClassVar[str] = "gcp_network"
     api_spec: ClassVar[GcpApiSpec] = GcpApiSpec(
@@ -3517,15 +3521,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -3605,15 +3609,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="nodeGroups",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -3675,46 +3679,46 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="nodeTemplates",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
-        "accelerators": S("accelerators", default=[]) >> ForallBend(GcpAcceleratorConfig.mapping),
+        "guest_accelerators": S("accelerators", default=[]) >> ForallBend(GcpAcceleratorConfig.mapping),
         "cpu_overcommit_type": S("cpuOvercommitType"),
-        "disks": S("disks", default=[]) >> ForallBend(GcpLocalDisk.mapping),
+        "local_disks": S("disks", default=[]) >> ForallBend(GcpLocalDisk.mapping),
         "node_affinity_labels": S("nodeAffinityLabels"),
         "node_type": S("nodeType"),
         "node_type_flexibility": S("nodeTypeFlexibility", default={})
         >> Bend(GcpNodeTemplateNodeTypeFlexibility.mapping),
         "server_binding": S("serverBinding", "type"),
         "status": S("status"),
         "status_message": S("statusMessage"),
     }
-    accelerators: Optional[List[GcpAcceleratorConfig]] = field(default=None)
+    guest_accelerators: Optional[List[GcpAcceleratorConfig]] = field(default=None)
     cpu_overcommit_type: Optional[str] = field(default=None)
-    disks: Optional[List[GcpLocalDisk]] = field(default=None)
+    local_disks: Optional[List[GcpLocalDisk]] = field(default=None)
     node_affinity_labels: Optional[Dict[str, str]] = field(default=None)
     node_type: Optional[str] = field(default=None)
     node_type_flexibility: Optional[GcpNodeTemplateNodeTypeFlexibility] = field(default=None)
     server_binding: Optional[str] = field(default=None)
     status: Optional[str] = field(default=None)
     status_message: Optional[str] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
-        if self.disks:
-            for disk in self.disks:
+        if self.local_disks:
+            for disk in self.local_disks:
                 builder.add_edge(self, reverse=True, clazz=GcpDiskType, link=disk.disk_type)
 
 
 @define(eq=False, slots=False)
 class GcpNodeType(GcpResource):
     kind: ClassVar[str] = "gcp_node_type"
     api_spec: ClassVar[GcpApiSpec] = GcpApiSpec(
@@ -3724,15 +3728,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="nodeTypes",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -3818,35 +3822,35 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="packetMirrorings",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "collector_ilb": S("collectorIlb", default={}) >> Bend(GcpPacketMirroringForwardingRuleInfo.mapping),
         "enable": S("enable"),
         "filter": S("filter", default={}) >> Bend(GcpPacketMirroringFilter.mapping),
         "mirrored_resources": S("mirroredResources", default={})
         >> Bend(GcpPacketMirroringMirroredResourceInfo.mapping),
-        "network": S("network", default={}) >> Bend(GcpPacketMirroringNetworkInfo.mapping),
+        "packet_mirroring_network": S("network", default={}) >> Bend(GcpPacketMirroringNetworkInfo.mapping),
         "priority": S("priority"),
     }
     collector_ilb: Optional[GcpPacketMirroringForwardingRuleInfo] = field(default=None)
     enable: Optional[str] = field(default=None)
     filter: Optional[GcpPacketMirroringFilter] = field(default=None)
     mirrored_resources: Optional[GcpPacketMirroringMirroredResourceInfo] = field(default=None)
-    network: Optional[GcpPacketMirroringNetworkInfo] = field(default=None)
+    packet_mirroring_network: Optional[GcpPacketMirroringNetworkInfo] = field(default=None)
     priority: Optional[int] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if mmr := self.mirrored_resources:
             for subnet in mmr.subnetworks or []:
                 builder.add_edge(self, reverse=True, clazz=GcpSubnetwork, link=subnet.url)
             for instance in mmr.instances or []:
@@ -3881,15 +3885,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -4027,38 +4031,38 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="commitments",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "auto_renew": S("autoRenew"),
-        "category": S("category"),
+        "commitment_category": S("category"),
         "end_timestamp": S("endTimestamp"),
         "license_resource": S("licenseResource", default={}) >> Bend(GcpLicenseResourceCommitment.mapping),
         "merge_source_commitments": S("mergeSourceCommitments", default=[]),
         "plan": S("plan"),
         "reservations": S("reservations", default=[]) >> ForallBend(GcpReservation.mapping),
         "resources": S("resources", default=[]) >> ForallBend(GcpResourceCommitment.mapping),
         "split_source_commitment": S("splitSourceCommitment"),
         "start_timestamp": S("startTimestamp"),
         "status": S("status"),
         "status_message": S("statusMessage"),
         "type": S("type"),
     }
     auto_renew: Optional[bool] = field(default=None)
-    category: Optional[str] = field(default=None)
+    commitment_category: Optional[str] = field(default=None)
     end_timestamp: Optional[datetime] = field(default=None)
     license_resource: Optional[GcpLicenseResourceCommitment] = field(default=None)
     merge_source_commitments: Optional[List[str]] = field(default=None)
     plan: Optional[str] = field(default=None)
     reservations: Optional[List[GcpReservation]] = field(default=None)
     resources: Optional[List[GcpResourceCommitment]] = field(default=None)
     split_source_commitment: Optional[str] = field(default=None)
@@ -4078,15 +4082,15 @@
         action="list",
         request_parameter={"project": "{project}", "region": "{region}"},
         request_parameter_in={"project", "region"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -4130,15 +4134,15 @@
         action="list",
         request_parameter={"project": "{project}", "region": "{region}"},
         request_parameter_in={"project", "region"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -4315,38 +4319,38 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="securityPolicies",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "adaptive_protection_config": S("adaptiveProtectionConfig", default={})
         >> Bend(GcpSecurityPolicyAdaptiveProtectionConfig.mapping),
         "advanced_options_config": S("advancedOptionsConfig", default={})
         >> Bend(GcpSecurityPolicyAdvancedOptionsConfig.mapping),
         "ddos_protection_config": S("ddosProtectionConfig", "ddosProtection"),
         "fingerprint": S("fingerprint"),
         "recaptcha_options_config": S("recaptchaOptionsConfig", "redirectSiteKey"),
-        "rules": S("rules", default=[]) >> ForallBend(GcpSecurityPolicyRule.mapping),
+        "security_policy_rules": S("rules", default=[]) >> ForallBend(GcpSecurityPolicyRule.mapping),
         "type": S("type"),
     }
     adaptive_protection_config: Optional[GcpSecurityPolicyAdaptiveProtectionConfig] = field(default=None)
     advanced_options_config: Optional[GcpSecurityPolicyAdvancedOptionsConfig] = field(default=None)
     ddos_protection_config: Optional[str] = field(default=None)
     fingerprint: Optional[str] = field(default=None)
     recaptcha_options_config: Optional[str] = field(default=None)
-    rules: Optional[List[GcpSecurityPolicyRule]] = field(default=None)
+    security_policy_rules: Optional[List[GcpSecurityPolicyRule]] = field(default=None)
     type: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpSslCertificateManagedSslCertificate:
     kind: ClassVar[str] = "gcp_ssl_certificate_managed_ssl_certificate"
     mapping: ClassVar[Dict[str, Bender]] = {
@@ -4377,15 +4381,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="sslCertificates",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -4416,15 +4420,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="sslPolicies",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -4457,15 +4461,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="targetHttpProxies",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -4496,15 +4500,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="targetHttpsProxies",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -4552,15 +4556,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -4918,15 +4922,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="urlMaps",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5114,34 +5118,35 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="resourcePolicies",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "group_placement_policy": S("groupPlacementPolicy", default={})
         >> Bend(GcpResourcePolicyGroupPlacementPolicy.mapping),
         "instance_schedule_policy": S("instanceSchedulePolicy", default={})
         >> Bend(GcpResourcePolicyInstanceSchedulePolicy.mapping),
-        "resource_status": S("resourceStatus", default={}) >> Bend(GcpResourcePolicyResourceStatus.mapping),
+        "resource_policy_resource_status": S("resourceStatus", default={})
+        >> Bend(GcpResourcePolicyResourceStatus.mapping),
         "snapshot_schedule_policy": S("snapshotSchedulePolicy", default={})
         >> Bend(GcpResourcePolicySnapshotSchedulePolicy.mapping),
         "status": S("status"),
     }
     group_placement_policy: Optional[GcpResourcePolicyGroupPlacementPolicy] = field(default=None)
     instance_schedule_policy: Optional[GcpResourcePolicyInstanceSchedulePolicy] = field(default=None)
-    resource_status: Optional[GcpResourcePolicyResourceStatus] = field(default=None)
+    resource_policy_resource_status: Optional[GcpResourcePolicyResourceStatus] = field(default=None)
     snapshot_schedule_policy: Optional[GcpResourcePolicySnapshotSchedulePolicy] = field(default=None)
     status: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpRouterAdvertisedIpRange:
     kind: ClassVar[str] = "gcp_router_advertised_ip_range"
@@ -5306,40 +5311,40 @@
     kind: ClassVar[str] = "gcp_router_nat"
     mapping: ClassVar[Dict[str, Bender]] = {
         "drain_nat_ips": S("drainNatIps", default=[]),
         "enable_dynamic_port_allocation": S("enableDynamicPortAllocation"),
         "enable_endpoint_independent_mapping": S("enableEndpointIndependentMapping"),
         "endpoint_types": S("endpointTypes", default=[]),
         "icmp_idle_timeout_sec": S("icmpIdleTimeoutSec"),
-        "log_config": S("logConfig", default={}) >> Bend(GcpRouterNatLogConfig.mapping),
+        "router_nat_log_config": S("logConfig", default={}) >> Bend(GcpRouterNatLogConfig.mapping),
         "max_ports_per_vm": S("maxPortsPerVm"),
         "min_ports_per_vm": S("minPortsPerVm"),
         "name": S("name"),
         "nat_ip_allocate_option": S("natIpAllocateOption"),
         "nat_ips": S("natIps", default=[]),
-        "rules": S("rules", default=[]) >> ForallBend(GcpRouterNatRule.mapping),
+        "router_nat_rules": S("rules", default=[]) >> ForallBend(GcpRouterNatRule.mapping),
         "source_subnetwork_ip_ranges_to_nat": S("sourceSubnetworkIpRangesToNat"),
         "subnetworks": S("subnetworks", default=[]) >> ForallBend(GcpRouterNatSubnetworkToNat.mapping),
         "tcp_established_idle_timeout_sec": S("tcpEstablishedIdleTimeoutSec"),
         "tcp_time_wait_timeout_sec": S("tcpTimeWaitTimeoutSec"),
         "tcp_transitory_idle_timeout_sec": S("tcpTransitoryIdleTimeoutSec"),
         "udp_idle_timeout_sec": S("udpIdleTimeoutSec"),
     }
     drain_nat_ips: Optional[List[str]] = field(default=None)
     enable_dynamic_port_allocation: Optional[bool] = field(default=None)
     enable_endpoint_independent_mapping: Optional[bool] = field(default=None)
     endpoint_types: Optional[List[str]] = field(default=None)
     icmp_idle_timeout_sec: Optional[int] = field(default=None)
-    log_config: Optional[GcpRouterNatLogConfig] = field(default=None)
+    router_nat_log_config: Optional[GcpRouterNatLogConfig] = field(default=None)
     max_ports_per_vm: Optional[int] = field(default=None)
     min_ports_per_vm: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     nat_ip_allocate_option: Optional[str] = field(default=None)
     nat_ips: Optional[List[str]] = field(default=None)
-    rules: Optional[List[GcpRouterNatRule]] = field(default=None)
+    router_nat_rules: Optional[List[GcpRouterNatRule]] = field(default=None)
     source_subnetwork_ip_ranges_to_nat: Optional[str] = field(default=None)
     subnetworks: Optional[List[GcpRouterNatSubnetworkToNat]] = field(default=None)
     tcp_established_idle_timeout_sec: Optional[int] = field(default=None)
     tcp_time_wait_timeout_sec: Optional[int] = field(default=None)
     tcp_transitory_idle_timeout_sec: Optional[int] = field(default=None)
     udp_idle_timeout_sec: Optional[int] = field(default=None)
 
@@ -5357,35 +5362,35 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="routers",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "bgp": S("bgp", default={}) >> Bend(GcpRouterBgp.mapping),
         "bgp_peers": S("bgpPeers", default=[]) >> ForallBend(GcpRouterBgpPeer.mapping),
         "encrypted_interconnect_router": S("encryptedInterconnectRouter"),
-        "interfaces": S("interfaces", default=[]) >> ForallBend(GcpRouterInterface.mapping),
+        "router_interfaces": S("interfaces", default=[]) >> ForallBend(GcpRouterInterface.mapping),
         "md5_authentication_keys": S("md5AuthenticationKeys", default=[])
         >> ForallBend(GcpRouterMd5AuthenticationKey.mapping),
         "nats": S("nats", default=[]) >> ForallBend(GcpRouterNat.mapping),
         "network": S("network"),
     }
     bgp: Optional[GcpRouterBgp] = field(default=None)
     bgp_peers: Optional[List[GcpRouterBgpPeer]] = field(default=None)
     encrypted_interconnect_router: Optional[bool] = field(default=None)
-    interfaces: Optional[List[GcpRouterInterface]] = field(default=None)
+    router_interfaces: Optional[List[GcpRouterInterface]] = field(default=None)
     md5_authentication_keys: Optional[List[GcpRouterMd5AuthenticationKey]] = field(default=None)
     nats: Optional[List[GcpRouterNat]] = field(default=None)
     network: Optional[str] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if self.network:
             builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=GcpNetwork, link=self.network)
@@ -5415,15 +5420,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5507,15 +5512,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="serviceAttachments",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5564,15 +5569,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5667,15 +5672,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="subnetworks",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5683,41 +5688,41 @@
         "external_ipv6_prefix": S("externalIpv6Prefix"),
         "fingerprint": S("fingerprint"),
         "gateway_address": S("gatewayAddress"),
         "internal_ipv6_prefix": S("internalIpv6Prefix"),
         "ip_cidr_range": S("ipCidrRange"),
         "ipv6_access_type": S("ipv6AccessType"),
         "ipv6_cidr_range": S("ipv6CidrRange"),
-        "log_config": S("logConfig", default={}) >> Bend(GcpSubnetworkLogConfig.mapping),
+        "subnetwork_log_config": S("logConfig", default={}) >> Bend(GcpSubnetworkLogConfig.mapping),
         "network": S("network"),
         "private_ip_google_access": S("privateIpGoogleAccess"),
         "private_ipv6_google_access": S("privateIpv6GoogleAccess"),
         "purpose": S("purpose"),
         "role": S("role"),
         "secondary_ip_ranges": S("secondaryIpRanges", default=[]) >> ForallBend(GcpSubnetworkSecondaryRange.mapping),
         "stack_type": S("stackType"),
-        "state": S("state"),
+        "subnetwork_state": S("state"),
     }
     enable_flow_logs: Optional[bool] = field(default=None)
     external_ipv6_prefix: Optional[str] = field(default=None)
     fingerprint: Optional[str] = field(default=None)
     gateway_address: Optional[str] = field(default=None)
     internal_ipv6_prefix: Optional[str] = field(default=None)
     ip_cidr_range: Optional[str] = field(default=None)
     ipv6_access_type: Optional[str] = field(default=None)
     ipv6_cidr_range: Optional[str] = field(default=None)
-    log_config: Optional[GcpSubnetworkLogConfig] = field(default=None)
+    subnetwork_log_config: Optional[GcpSubnetworkLogConfig] = field(default=None)
     network: Optional[str] = field(default=None)
     private_ip_google_access: Optional[bool] = field(default=None)
     private_ipv6_google_access: Optional[str] = field(default=None)
     purpose: Optional[str] = field(default=None)
     role: Optional[str] = field(default=None)
     secondary_ip_ranges: Optional[List[GcpSubnetworkSecondaryRange]] = field(default=None)
     stack_type: Optional[str] = field(default=None)
-    state: Optional[str] = field(default=None)
+    subnetwork_state: Optional[str] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if self.network:
             builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=GcpNetwork, link=self.network)
 
 
 @define(eq=False, slots=False)
@@ -5736,15 +5741,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5777,15 +5782,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="targetInstances",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5818,15 +5823,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="targetPools",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5865,15 +5870,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5898,28 +5903,27 @@
 
 
 @define(eq=False, slots=False)
 class GcpTargetVpnGateway(GcpResource):
     kind: ClassVar[str] = "gcp_target_vpn_gateway"
     reference_kinds: ClassVar[ModelReference] = {
         "predecessors": {"default": ["gcp_network"], "delete": ["gcp_network"]},
-        "successors": {"default": ["gcp_forwarding_rule"]},
     }
     api_spec: ClassVar[GcpApiSpec] = GcpApiSpec(
         service="compute",
         version="v1",
         accessors=["targetVpnGateways"],
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="targetVpnGateways",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -5930,17 +5934,14 @@
     }
     forwarding_rules: Optional[List[str]] = field(default=None)
     network: Optional[str] = field(default=None)
     status: Optional[str] = field(default=None)
     tunnels: Optional[List[str]] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
-        if self.forwarding_rules:
-            for rule in self.forwarding_rules:
-                builder.add_edge(self, clazz=GcpForwardingRule, link=rule)
         if self.network:
             builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=GcpNetwork, link=self.network)
 
 
 @define(eq=False, slots=False)
 class GcpVpnGatewayVpnGatewayInterface:
     kind: ClassVar[str] = "gcp_vpn_gateway_vpn_gateway_interface"
@@ -5968,15 +5969,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="vpnGateways",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -6013,15 +6014,15 @@
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="vpnTunnels",
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,15 +780,15 @@
         action="list",
         request_parameter={"parent": "projects/{project}/locations/-"},
         request_parameter_in={"project"},
         response_path="clusters",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -819,15 +819,16 @@
         "instance_group_urls": S("instanceGroupUrls", default=[]),
         "ip_allocation_policy": S("ipAllocationPolicy", default={}) >> Bend(GcpContainerIPAllocationPolicy.mapping),
         "legacy_abac": S("legacyAbac", "enabled"),
         "location": S("location"),
         "locations": S("locations", default=[]),
         "logging_config": S("loggingConfig", default={}) >> Bend(GcpContainerLoggingConfig.mapping),
         "logging_service": S("loggingService"),
-        "maintenance_policy": S("maintenancePolicy", default={}) >> Bend(GcpContainerMaintenancePolicy.mapping),
+        "container_cluster_maintenance_policy": S("maintenancePolicy", default={})
+        >> Bend(GcpContainerMaintenancePolicy.mapping),
         "master_auth": S("masterAuth", default={}) >> Bend(GcpContainerMasterAuth.mapping),
         "master_authorized_networks_config": S("masterAuthorizedNetworksConfig", default={})
         >> Bend(GcpContainerMasterAuthorizedNetworksConfig.mapping),
         "mesh_certificates": S("meshCertificates", "enableCertificates"),
         "monitoring_config": S("monitoringConfig", default={}) >> Bend(GcpContainerMonitoringConfig.mapping),
         "monitoring_service": S("monitoringService"),
         "network": S("network"),
@@ -880,15 +881,15 @@
     instance_group_urls: Optional[List[str]] = field(default=None)
     ip_allocation_policy: Optional[GcpContainerIPAllocationPolicy] = field(default=None)
     legacy_abac: Optional[bool] = field(default=None)
     location: Optional[str] = field(default=None)
     locations: Optional[List[str]] = field(default=None)
     logging_config: Optional[GcpContainerLoggingConfig] = field(default=None)
     logging_service: Optional[str] = field(default=None)
-    maintenance_policy: Optional[GcpContainerMaintenancePolicy] = field(default=None)
+    container_cluster_maintenance_policy: Optional[GcpContainerMaintenancePolicy] = field(default=None)
     master_auth: Optional[GcpContainerMasterAuth] = field(default=None)
     master_authorized_networks_config: Optional[GcpContainerMasterAuthorizedNetworksConfig] = field(default=None)
     mesh_certificates: Optional[bool] = field(default=None)
     monitoring_config: Optional[GcpContainerMonitoringConfig] = field(default=None)
     monitoring_service: Optional[str] = field(default=None)
     network: Optional[str] = field(default=None)
     network_config: Optional[GcpContainerNetworkConfig] = field(default=None)
@@ -965,43 +966,43 @@
         action="list",
         request_parameter={"parent": "projects/{project}/locations/-"},
         request_parameter_in={"project"},
         response_path="operations",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "cluster_conditions": S("clusterConditions", default=[]) >> ForallBend(GcpContainerStatusCondition.mapping),
         "detail": S("detail"),
         "end_time": S("endTime"),
-        "error": S("error", default={}) >> Bend(GcpContainerStatus.mapping),
+        "container_operation_error": S("error", default={}) >> Bend(GcpContainerStatus.mapping),
         "location": S("location"),
         "nodepool_conditions": S("nodepoolConditions", default=[]) >> ForallBend(GcpContainerStatusCondition.mapping),
         "operation_type": S("operationType"),
-        "progress": S("progress", default={}) >> Bend(GcpContainerOperationProgress.mapping),
+        "container_operation_progress": S("progress", default={}) >> Bend(GcpContainerOperationProgress.mapping),
         "start_time": S("startTime"),
         "status": S("status"),
         "status_message": S("statusMessage"),
         "target_link": S("targetLink"),
     }
     cluster_conditions: Optional[List[GcpContainerStatusCondition]] = field(default=None)
     detail: Optional[str] = field(default=None)
     end_time: Optional[datetime] = field(default=None)
-    error: Optional[GcpContainerStatus] = field(default=None)
+    container_operation_error: Optional[GcpContainerStatus] = field(default=None)
     location: Optional[str] = field(default=None)
     nodepool_conditions: Optional[List[GcpContainerStatusCondition]] = field(default=None)
     operation_type: Optional[str] = field(default=None)
-    progress: Optional[GcpContainerOperationProgress] = field(default=None)
+    container_operation_progress: Optional[GcpContainerOperationProgress] = field(default=None)
     start_time: Optional[datetime] = field(default=None)
     status: Optional[str] = field(default=None)
     status_message: Optional[str] = field(default=None)
     target_link: Optional[str] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if self.target_link:
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from attr import define, field
 
 from resoto_plugin_gcp.gcp_client import GcpApiSpec
 from resoto_plugin_gcp.resources.base import GcpResource, GcpDeprecationStatus, GraphBuilder
 from resoto_plugin_gcp.resources.compute import GcpSslCertificate
 from resotolib.baseresources import ModelReference
-from resotolib.json_bender import Bender, S, Bend, ForallBend
+from resotolib.json_bender import Bender, S, Bend, ForallBend, K
 from resotolib.types import Json
 
 log = logging.getLogger("resoto.plugins.gcp")
 
 
 @define(eq=False, slots=False)
 class GcpSqlOperationError:
@@ -34,42 +34,42 @@
         action="list",
         request_parameter={"instance": "{instance}", "project": "{project}"},
         request_parameter_in={"instance", "project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "backup_kind": S("backupKind"),
         "disk_encryption_configuration": S("diskEncryptionConfiguration", "kmsKeyName"),
         "disk_encryption_status": S("diskEncryptionStatus", "kmsKeyVersionName"),
         "end_time": S("endTime"),
         "enqueued_time": S("enqueuedTime"),
-        "error": S("error", default={}) >> Bend(GcpSqlOperationError.mapping),
+        "sql_operation_error": S("error", default={}) >> Bend(GcpSqlOperationError.mapping),
         "instance": S("instance"),
         "location": S("location"),
         "start_time": S("startTime"),
         "status": S("status"),
         "time_zone": S("timeZone"),
         "type": S("type"),
         "window_start_time": S("windowStartTime"),
     }
     backup_kind: Optional[str] = field(default=None)
     disk_encryption_configuration: Optional[str] = field(default=None)
     disk_encryption_status: Optional[str] = field(default=None)
     end_time: Optional[datetime] = field(default=None)
     enqueued_time: Optional[datetime] = field(default=None)
-    error: Optional[GcpSqlOperationError] = field(default=None)
+    sql_operation_error: Optional[GcpSqlOperationError] = field(default=None)
     instance: Optional[str] = field(default=None)
     location: Optional[str] = field(default=None)
     start_time: Optional[datetime] = field(default=None)
     status: Optional[str] = field(default=None)
     time_zone: Optional[str] = field(default=None)
     type: Optional[str] = field(default=None)
     window_start_time: Optional[datetime] = field(default=None)
@@ -101,15 +101,15 @@
         action="list",
         request_parameter={"instance": "{instance}", "project": "{project}"},
         request_parameter_in={"instance", "project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -130,55 +130,14 @@
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if self.instance:
             builder.add_edge(self, reverse=True, clazz=GcpSqlDatabaseInstance, name=self.instance)
 
 
 @define(eq=False, slots=False)
-class GcpSqlFlag(GcpResource):
-    kind: ClassVar[str] = "gcp_sql_flag"
-    api_spec: ClassVar[GcpApiSpec] = GcpApiSpec(
-        service="sqladmin",
-        version="v1",
-        accessors=["flags"],
-        action="list",
-        request_parameter={},
-        request_parameter_in=set(),
-        response_path="items",
-        response_regional_sub_path=None,
-    )
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
-        "tags": S("labels", default={}),
-        "name": S("name"),
-        "ctime": S("creationTimestamp"),
-        "description": S("description"),
-        "link": S("selfLink"),
-        "label_fingerprint": S("labelFingerprint"),
-        "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
-        "allowed_int_values": S("allowedIntValues", default=[]),
-        "allowed_string_values": S("allowedStringValues", default=[]),
-        "applies_to": S("appliesTo", default=[]),
-        "in_beta": S("inBeta"),
-        "max_value": S("maxValue"),
-        "min_value": S("minValue"),
-        "requires_restart": S("requiresRestart"),
-        "type": S("type"),
-    }
-    allowed_int_values: Optional[List[str]] = field(default=None)
-    allowed_string_values: Optional[List[str]] = field(default=None)
-    applies_to: Optional[List[str]] = field(default=None)
-    in_beta: Optional[bool] = field(default=None)
-    max_value: Optional[str] = field(default=None)
-    min_value: Optional[str] = field(default=None)
-    requires_restart: Optional[bool] = field(default=None)
-    type: Optional[str] = field(default=None)
-
-
-@define(eq=False, slots=False)
 class GcpSqlFailoverreplica:
     kind: ClassVar[str] = "gcp_sql_failoverreplica"
     mapping: ClassVar[Dict[str, Bender]] = {"available": S("available"), "name": S("name")}
     available: Optional[bool] = field(default=None)
     name: Optional[str] = field(default=None)
 
 
@@ -544,15 +503,15 @@
         action="list",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("createTime"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
@@ -583,15 +542,15 @@
         "root_password": S("rootPassword"),
         "satisfies_pzs": S("satisfiesPzs"),
         "scheduled_maintenance": S("scheduledMaintenance", default={}) >> Bend(GcpSqlSqlScheduledMaintenance.mapping),
         "secondary_gce_zone": S("secondaryGceZone"),
         "server_ca_cert": S("serverCaCert", default={}) >> Bend(GcpSqlSslCert.mapping),
         "service_account_email_address": S("serviceAccountEmailAddress"),
         "settings": S("settings", default={}) >> Bend(GcpSqlSettings.mapping),
-        "state": S("state"),
+        "sql_database_instance_state": S("state"),
         "suspension_reason": S("suspensionReason", default=[]),
     }
     available_maintenance_versions: Optional[List[str]] = field(default=None)
     backend_type: Optional[str] = field(default=None)
     connection_name: Optional[str] = field(default=None)
     create_time: Optional[datetime] = field(default=None)
     current_disk_size: Optional[str] = field(default=None)
@@ -616,15 +575,15 @@
     root_password: Optional[str] = field(default=None)
     satisfies_pzs: Optional[bool] = field(default=None)
     scheduled_maintenance: Optional[GcpSqlSqlScheduledMaintenance] = field(default=None)
     secondary_gce_zone: Optional[str] = field(default=None)
     server_ca_cert: Optional[GcpSqlSslCert] = field(default=None)
     service_account_email_address: Optional[str] = field(default=None)
     settings: Optional[GcpSqlSettings] = field(default=None)
-    state: Optional[str] = field(default=None)
+    sql_database_instance_state: Optional[str] = field(default=None)
     suspension_reason: Optional[List[str]] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if cert := self.server_ca_cert:
             if cert.self_link:
                 builder.add_edge(self, reverse=True, clazz=GcpSslCertificate, link=cert.self_link)
 
@@ -633,23 +592,14 @@
         for cls in classes:
             if spec := cls.api_spec:
                 items = graph_builder.client.list(spec, instance=self.name, project=self.project)
                 cls.collect(items, graph_builder)
 
 
 @define(eq=False, slots=False)
-class GcpSqlOperationErrors:
-    kind: ClassVar[str] = "gcp_sql_operation_errors"
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "errors": S("errors", default=[]) >> ForallBend(GcpSqlOperationError.mapping)
-    }
-    errors: Optional[List[GcpSqlOperationError]] = field(default=None)
-
-
-@define(eq=False, slots=False)
 class GcpSqlCsvexportoptions:
     kind: ClassVar[str] = "gcp_sql_csvexportoptions"
     mapping: ClassVar[Dict[str, Bender]] = {
         "escape_character": S("escapeCharacter"),
         "fields_terminated_by": S("fieldsTerminatedBy"),
         "lines_terminated_by": S("linesTerminatedBy"),
         "quote_character": S("quoteCharacter"),
@@ -772,39 +722,39 @@
         action="list",
         request_parameter={"instance": "{instance}", "project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "backup_context": S("backupContext", "backupId"),
         "end_time": S("endTime"),
-        "error": S("error", default={}) >> Bend(GcpSqlOperationErrors.mapping),
+        "sql_operation_errors": S("error", "errors", default=[]) >> ForallBend(GcpSqlOperationError.mapping),
         "export_context": S("exportContext", default={}) >> Bend(GcpSqlExportContext.mapping),
         "import_context": S("importContext", default={}) >> Bend(GcpSqlImportContext.mapping),
         "insert_time": S("insertTime"),
         "operation_type": S("operationType"),
         "start_time": S("startTime"),
         "status": S("status"),
         "target_id": S("targetId"),
         "target_link": S("targetLink"),
         "target_project": S("targetProject"),
         "user": S("user"),
     }
     backup_context: Optional[str] = field(default=None)
     end_time: Optional[datetime] = field(default=None)
-    error: Optional[GcpSqlOperationErrors] = field(default=None)
+    sql_operation_errors: List[GcpSqlOperationError] = field(factory=list)
     export_context: Optional[GcpSqlExportContext] = field(default=None)
     import_context: Optional[GcpSqlImportContext] = field(default=None)
     insert_time: Optional[datetime] = field(default=None)
     operation_type: Optional[str] = field(default=None)
     start_time: Optional[datetime] = field(default=None)
     status: Optional[str] = field(default=None)
     target_id: Optional[str] = field(default=None)
@@ -864,25 +814,25 @@
         action="list",
         request_parameter={"instance": "{instance}", "project": "{project}"},
         request_parameter_in={"instance", "project"},
         response_path="items",
         response_regional_sub_path=None,
     )
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("id").or_else(S("name")).or_else(S("selfLink")),
+        "id": S("name").or_else(K("(anonymous)@") + S("host", default="localhost")),
         "tags": S("labels", default={}),
-        "name": S("name"),
+        "name": S("name", default="(anonymous)"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "dual_password_type": S("dualPasswordType"),
         "etag": S("etag"),
-        "host": S("host"),
+        "host": S("host", default="localhost"),
         "instance": S("instance"),
         "password": S("password"),
         "password_policy": S("passwordPolicy", default={}) >> Bend(GcpSqlUserPasswordValidationPolicy.mapping),
         "project": S("project"),
         "sqlserver_user_details": S("sqlserverUserDetails", default={}) >> Bend(GcpSqlSqlServerUserDetails.mapping),
         "type": S("type"),
     }
@@ -897,8 +847,8 @@
     type: Optional[str] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if self.instance:
             builder.add_edge(self, reverse=True, clazz=GcpSqlDatabaseInstance)
 
 
-resources = [GcpSqlFlag, GcpSqlDatabaseInstance]
+resources = [GcpSqlDatabaseInstance]
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import socket
 from resotolib.baseresources import BaseResource
 from resotolib.config import Config
 from resotolib.graph import Graph
 from resotolib.lock import RWLock
 import resotolib.logger
-from typing import Iterable, List, Union, Callable, Any, Dict, Optional
+from typing import Iterable, List, Union, Callable, Any, Dict
 from googleapiclient import discovery
 from googleapiclient.errors import HttpError as GoogleApiClientHttpError
 from googleapiclient.discovery_cache.base import Cache as GoogleApiClientCache
 from google.oauth2 import service_account
 from datetime import datetime
 from retrying import retry
 from tenacity import Retrying, stop_after_attempt, retry_if_exception_type
@@ -224,42 +224,14 @@
 
     gr = gcp_resource(resource)
     request = gr.delete(**delete_kwargs)
     request.execute()
     return True
 
 
-def update_label(resource: BaseResource, key: str, value: Optional[str]) -> bool:
-    get_kwargs = {str(resource._get_identifier): resource.name}
-    set_labels_kwargs = {str(resource._set_label_identifier): resource.name}
-
-    common_kwargs = common_resource_kwargs(resource)
-    get_kwargs.update(common_kwargs)
-    set_labels_kwargs.update(common_kwargs)
-
-    labels = dict(resource.tags)
-    if value is None:
-        if key in labels:
-            del labels[key]
-        else:
-            return False
-    else:
-        labels.update({key: value})
-    body = {"labels": labels, "labelFingerprint": resource.label_fingerprint}
-    set_labels_kwargs["body"] = body
-    gr = gcp_resource(resource)
-    request = gr.setLabels(**set_labels_kwargs)
-    response = request.execute()
-    # Update label_fingerprint
-    request = gr.get(**get_kwargs)
-    response = request.execute()
-    resource.label_fingerprint = response.get("labelFingerprint")
-    return True
-
-
 def gcp_service(resource: BaseResource, graph: Graph = None):
     service_kwargs = {}
     if resource.account().id != "undefined":
         service_kwargs["credentials"] = Credentials.get(resource.account(graph).id)
     return gcp_client(resource.client, resource.api_version, **service_kwargs)
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto GCP Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.4.2/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 resoto_plugin_gcp/__init__.py
-resoto_plugin_gcp/collector.py
 resoto_plugin_gcp/config.py
 resoto_plugin_gcp/gcp_client.py
-resoto_plugin_gcp/gcp_resources.py
 resoto_plugin_gcp/project_collector.py
 resoto_plugin_gcp/utils.py
 resoto_plugin_gcp.egg-info/PKG-INFO
 resoto_plugin_gcp.egg-info/SOURCES.txt
 resoto_plugin_gcp.egg-info/dependency_links.txt
 resoto_plugin_gcp.egg-info/entry_points.txt
 resoto_plugin_gcp.egg-info/not-zip-safe
@@ -19,17 +17,19 @@
 resoto_plugin_gcp.egg-info/top_level.txt
 resoto_plugin_gcp/resources/__init__.py
 resoto_plugin_gcp/resources/base.py
 resoto_plugin_gcp/resources/billing.py
 resoto_plugin_gcp/resources/compute.py
 resoto_plugin_gcp/resources/container.py
 resoto_plugin_gcp/resources/sqladmin.py
+resoto_plugin_gcp/resources/storage.py
 test/__init__.py
 test/conftest.py
 test/random_client.py
 test/test_base.py
 test/test_billing.py
 test/test_compute.py
 test/test_config.py
 test/test_container.py
 test/test_project_collector.py
-test/test_sqladmin.py
+test/test_sqladmin.py
+test/test_storage.py
```

### Comparing `resoto-plugin-gcp-3.4.2/setup.py` & `resoto-plugin-gcp-3.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-gcp",
-    version="3.4.2",
+    version="3.5.0",
     description="Resoto GCP Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["gcp = resoto_plugin_gcp:GCPCollectorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-gcp-3.4.2/test/conftest.py` & `resoto-plugin-gcp-3.5.0/test/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from google.auth.credentials import AnonymousCredentials
 from googleapiclient import discovery
 from pytest import fixture
 
 from resoto_plugin_gcp import gcp_client
 from resoto_plugin_gcp.config import GcpConfig
-from resoto_plugin_gcp.resources.base import ExecutorQueue, GraphBuilder, GcpProject
+from resoto_plugin_gcp.resources.base import ExecutorQueue, GcpRegion, GraphBuilder, GcpProject
 from resotolib.baseresources import Cloud
 from resotolib.config import Config
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
 from .random_client import build_random_data_client, random_predefined
 
 
@@ -29,15 +29,20 @@
     # Initialise config
     Config.add_config(GcpConfig)
     Config.init_default_config()
     # change discovery function factory for tests
     gcp_client._discovery_function = build_random_data_client
     queue = ExecutorQueue(DummyExecutor(), "dummy")
     feedback = CoreFeedback("test", "test", "test", Queue())
-    builder = GraphBuilder(Graph(), Cloud(id="gcp"), GcpProject(id="test"), AnonymousCredentials(), queue, feedback)
+    project = GcpProject(id="test")
+    project_global_region = GcpRegion.fallback_global_region(project)
+    builder = GraphBuilder(
+        Graph(), Cloud(id="gcp"), project, AnonymousCredentials(), queue, feedback, project_global_region
+    )
+    builder.add_node(project_global_region, {})
     # add predefined regions and zones
     for predefined in random_predefined:
         builder.add_node(predefined)
     builder.prepare_region_zone_lookup()
     # provide the builder to the test method
     yield builder
     # rest the original discovery function
```

### Comparing `resoto-plugin-gcp-3.4.2/test/random_client.py` & `resoto-plugin-gcp-3.5.0/test/random_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.2/test/test_base.py` & `resoto-plugin-gcp-3.5.0/test/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from resoto_plugin_gcp.resources.compute import GcpMachineType
 
 
 def test_node_by_filter(random_builder: GraphBuilder) -> None:
     with open(os.path.dirname(__file__) + "/files/machine_type.json") as f:
         GcpMachineType.collect(raw=json.load(f)["items"]["machineTypes"], builder=random_builder)
 
-    assert random_builder.node(clazz=GcpMachineType, id="804416")
+    assert random_builder.node(clazz=GcpMachineType, name="m2-ultramem-416")
 
     def filter_1(node: GcpMachineType) -> bool:
         return node.name is not None and node.name.startswith("m2-ultramem") and node.kind == "gcp_machine_type"
 
     def filter_2(node: GcpMachineType) -> bool:
         return node.name is not None and node.name.startswith("m2-ultramem")
```

### Comparing `resoto-plugin-gcp-3.4.2/test/test_billing.py` & `resoto-plugin-gcp-3.5.0/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.2/test/test_compute.py` & `resoto-plugin-gcp-3.5.0/test/test_compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 def test_gcp_backend_bucket(random_builder: GraphBuilder) -> None:
     roundtrip(GcpBackendBucket, random_builder)
 
 
 def test_gcp_backend_service(random_builder: GraphBuilder) -> None:
     service = roundtrip(GcpBackendService, random_builder)
     assert service.health_checks
-    assert service.backends
+    assert service.backend_service_backends
     connect_resource(random_builder, service, GcpHealthCheck, selfLink=service.health_checks[0])
     assert len(random_builder.edges_of(GcpBackendService, GcpHealthCheck)) == 1
-    connect_resource(random_builder, service, GcpInstanceGroup, selfLink=service.backends[0].group)
+    connect_resource(random_builder, service, GcpInstanceGroup, selfLink=service.backend_service_backends[0].group)
     assert len(random_builder.edges_of(GcpBackendService, GcpInstanceGroup)) == 1
     connect_resource(random_builder, service, GcpNetwork, selfLink=service.network)
     assert len(random_builder.edges_of(GcpNetwork, GcpBackendService)) == 1
 
 
 def test_gcp_disk_type(random_builder: GraphBuilder) -> None:
     roundtrip(GcpDiskType, random_builder)
@@ -73,17 +73,17 @@
 
 def test_gcp_external_vpn_gateway(random_builder: GraphBuilder) -> None:
     roundtrip(GcpExternalVpnGateway, random_builder)
 
 
 def test_gcp_firewall_policy(random_builder: GraphBuilder) -> None:
     policy = roundtrip(GcpFirewallPolicy, random_builder)
-    assert policy.rules
-    assert policy.rules[0].target_resources
-    connect_resource(random_builder, policy, GcpNetwork, selfLink=policy.rules[0].target_resources[0])
+    assert policy.firewall_policy_rules
+    assert policy.firewall_policy_rules[0].target_resources
+    connect_resource(random_builder, policy, GcpNetwork, selfLink=policy.firewall_policy_rules[0].target_resources[0])
     assert len(random_builder.edges_of(GcpFirewallPolicy, GcpNetwork)) == 1
 
 
 def test_gcp_firewall(random_builder: GraphBuilder) -> None:
     firewall = roundtrip(GcpFirewall, random_builder)
     connect_resource(random_builder, firewall, GcpNetwork, selfLink=firewall.network)
     assert len(random_builder.edges_of(GcpFirewall, GcpNetwork)) == 1
```

### Comparing `resoto-plugin-gcp-3.4.2/test/test_config.py` & `resoto-plugin-gcp-3.5.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.2/test/test_container.py` & `resoto-plugin-gcp-3.5.0/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.2/test/test_project_collector.py` & `resoto-plugin-gcp-3.5.0/test/test_project_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.2/test/test_sqladmin.py` & `resoto-plugin-gcp-3.5.0/test/test_sqladmin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+import json
+import os
+
 from .random_client import connect_resource, roundtrip
 from resoto_plugin_gcp.resources.sqladmin import *
 from resoto_plugin_gcp.resources.base import GraphBuilder
 from resoto_plugin_gcp.resources.compute import GcpSslCertificate
 
 
-def test_gcp_sql_flag(random_builder: GraphBuilder) -> None:
-    roundtrip(GcpSqlFlag, random_builder)
-
-
 def test_gcp_sql_database_instance(random_builder: GraphBuilder) -> None:
     db = roundtrip(GcpSqlDatabaseInstance, random_builder)
     connect_resource(random_builder, db, GcpSslCertificate, selfLink=db.server_ca_cert.self_link)  # type: ignore
     assert len(random_builder.edges_of(GcpSslCertificate, GcpSqlDatabaseInstance)) == 1
     assert len(random_builder.resources_of(GcpSqlBackupRun)) > 0
     assert len(random_builder.edges_of(GcpSqlDatabaseInstance, GcpSqlBackupRun)) > 0
     assert len(random_builder.resources_of(GcpSqlDatabase)) > 0
     assert len(random_builder.resources_of(GcpSqlUser)) > 0
     assert len(random_builder.resources_of(GcpSqlOperation)) > 0
+
+
+def test_instance_with_settings(random_builder: GraphBuilder) -> None:
+    with open(os.path.dirname(__file__) + "/files/database_instance.json") as f:
+        GcpSqlDatabaseInstance.collect(raw=json.load(f)["items"], builder=random_builder)
+
+    db = random_builder.resources_of(GcpSqlDatabaseInstance)
+    assert db
```


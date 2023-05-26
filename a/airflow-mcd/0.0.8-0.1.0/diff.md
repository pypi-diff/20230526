# Comparing `tmp/airflow_mcd-0.0.8.tar.gz` & `tmp/airflow_mcd-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.0.8.tar", last modified: Wed May 24 15:04:11 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.1.0.tar", last modified: Fri May 26 20:09:12 2023, max compression
```

## Comparing `airflow_mcd-0.0.8.tar` & `airflow_mcd-0.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/Makefile
--rw-r--r--   0 root         (0) root         (0)     5259 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     4445 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     5457 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     5476 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     4690 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/airflow_mcd/operators/circuit_breaker_operators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5259 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      980 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 15:04:11.000000 airflow_mcd-0.0.8/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-24 15:04:11.977982 airflow_mcd-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1484 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10230 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:04:11.973982 airflow_mcd-0.0.8/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-05-24 15:03:07.000000 airflow_mcd-0.0.8/tests/operators/test_circuit_breaker_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     5575 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     4695 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/operators/circuit_breaker_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-26 20:09:12.883684 airflow_mcd-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/operators/test_circuit_breaker_op.py
```

### Comparing `airflow_mcd-0.0.8/.circleci/config.yml` & `airflow_mcd-0.1.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/.gitignore` & `airflow_mcd-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/LICENSE` & `airflow_mcd-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/Makefile` & `airflow_mcd-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/README-dev.md` & `airflow_mcd-0.1.0/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.1.0/airflow_mcd/callbacks/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 logger = logging.getLogger(__name__)
 
 
 @dataclass_json
 @dataclass
 class AirflowEnv:
     # these env vars are used to get additional information about the Airflow
-    # environment when running in AWS
-    env_name: str = os.environ.get('AIRFLOW_ENV_NAME', 'airflow')
-    env_id: Optional[str] = os.environ.get('AIRFLOW_ENV_ID')
-    version: Optional[str] = os.environ.get('AIRFLOW_VERSION')
+    # environment when running in AWS or GCP.
+    env_name: str = os.environ.get('AIRFLOW_ENV_NAME', os.environ.get('COMPOSER_ENVIRONMENT', 'airflow'))
+    env_id: Optional[str] = os.environ.get('AIRFLOW_ENV_ID', os.environ.get('COMPOSER_GKE_NAME'))
+    version: Optional[str] = os.environ.get('AIRFLOW_VERSION', os.environ.get('MAJOR_VERSION'))
     base_url: Optional[str] = os.environ.get('AIRFLOW__WEBSERVER__BASE_URL')
 
 
 @dataclass_json
 @dataclass
 class DagTaskInstanceResult:
     task_id: str
```

### Comparing `airflow_mcd-0.0.8/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.1.0/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,27 @@
     """
     try:
         AirflowEventsClientUtils.mcd_post_task_result(success=True, context=context)
     except Exception as ex:
         logger.exception(f'Failed to post task result to MCD: {ex}')
 
 
+def mcd_task_execute_callback(context: Dict):
+    """
+    Callback function that sends the Task execution event to Monte Carlo, it must be configured as
+    `on_execute_callback` in a Task object.
+    You can also manually invoke this function from your own callback code passing the same context you received.
+    :param context: The Airflow Task execution context.
+    """
+    try:
+        AirflowEventsClientUtils.mcd_post_task_result(success=True, context=context)
+    except Exception as ex:
+        logger.exception(f'Failed to post task result to MCD: {ex}')
+
+
 def mcd_task_failure_callback(context: Dict):
     """
     Callback function that sends the Task failure event to Monte Carlo, it must be configured as
     `on_failure_callback` in a Task object.
     You can also manually invoke this function from your own callback code passing the same context you received.
     :param context: The Airflow Task failure context.
     """
@@ -141,14 +154,15 @@
         logger.exception(f'Failed to post SLA misses result to MCD: {ex}')
 
 
 task_callbacks = {
     'on_success_callback': mcd_task_success_callback,
     'on_failure_callback': mcd_task_failure_callback,
     'on_retry_callback': mcd_task_retry_callback,
+    'on_execute_callback': mcd_task_execute_callback,
 }
 
 dag_callbacks = {
     'on_failure_callback': mcd_dag_failure_callback,
     'on_success_callback': mcd_dag_success_callback,
     'sla_miss_callback': mcd_sla_miss_callback,
 }
```

### Comparing `airflow_mcd-0.0.8/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.1.0/airflow_mcd/callbacks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             exception_message: Optional[str] = None
     ) -> DagTaskInstanceResult:
         return DagTaskInstanceResult(
             task_id=ti.task_id,
             state=ti.state,
             log_url=ti.log_url,
             prev_attempted_tries=ti.prev_attempted_tries,
-            duration=ti.duration,
+            duration=ti.duration or 0,
             execution_date=ti.execution_date.isoformat(),
             start_date=ti.start_date.isoformat(),
             end_date=ti.end_date.isoformat() if ti.end_date else datetime.now(tz=pytz.UTC).isoformat(),
             next_retry_datetime=cls._get_next_retry_datetime(ti),
             max_tries=ti.max_tries,
             try_number=ti.try_number,
             exception_message=exception_message,
```

### Comparing `airflow_mcd-0.0.8/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.1.0/airflow_mcd/hooks/session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.1.0/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.1.0/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.1.0/airflow_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/examples/sample_circuit_dag.py` & `airflow_mcd-0.1.0/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/setup.py` & `airflow_mcd-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     author='Monte Carlo Data, Inc',
     author_email='info@montecarlodata.com',
     url='https://www.montecarlodata.com/',
     packages=find_packages(exclude=['tests*', 'examples*']),
     include_package_data=True,
     install_requires=parse_requirements(),
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `airflow_mcd-0.0.8/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.1.0/tests/callbacks/test_callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,23 @@
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_dag_result_failure(self, mock_client_upload_result):
         self._test_upload_dag_result(False, mock_client_upload_result)
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_success(self, mock_client_upload_result):
-        self._test_upload_task_result(True, mock_client_upload_result)
+        self._test_upload_task_result(True, False, mock_client_upload_result)
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_failure(self, mock_client_upload_result):
-        self._test_upload_task_result(False, mock_client_upload_result)
+        self._test_upload_task_result(False, False, mock_client_upload_result)
+
+    @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
+    def test_upload_task_result_running(self, mock_client_upload_result):
+        self._test_upload_task_result(True, True, mock_client_upload_result)
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_sla_misses(self, mock_client_upload_result):
         utils = AirflowEventsClientUtils()
 
         dag = create_autospec(DAG)
         dag.dag_id = "dag_123"
@@ -139,24 +143,25 @@
         return {
             "env_name": "airflow",
             "env_id": None,
             "version": None,
             "base_url": None
         }
 
-    def _create_dag_context(self, success: bool) -> Dict:
+    def _create_dag_context(self, success: bool, task_running: bool = False) -> Dict:
         dag = create_autospec(DAG)
         dag.dag_id = "dag_123"
         dag.params = {}
         dag_run = create_autospec(DagRun)
         task_instances = [
             self._create_task_instance(
                 dag_id=dag.dag_id,
                 task_id="task_123",
-                state="success",
+                state="running" if task_running else "success",
+                running=task_running,
             ),
             self._create_task_instance(
                 dag_id=dag.dag_id,
                 task_id="task_234",
                 state="success",
             ),
         ]
@@ -174,18 +179,19 @@
             "reason": "succeeded" if success else "task failed",
         }
         return dag_context
 
     def _test_upload_task_result(
             self,
             success: bool,
+            task_running: bool,
             mock_client_upload_result
     ):
-        dag_context = self._create_dag_context(success)
-        state = "success" if success else "failed"
+        dag_context = self._create_dag_context(success, task_running)
+        state = "running" if task_running else "success" if success else "failed"
         exception_message: str = "task failed" if not success else None
         if not success:
             dag_context["exception"] = Exception(exception_message)
         dag: DAG = dag_context["dag"]
         dag_run: DagRun = dag_context["dag_run"]
         task_instances: List[TaskInstance] = dag_run.get_task_instances()
         task_instance = task_instances[0]
@@ -201,15 +207,15 @@
             "success": success,
             "env": self._get_graphql_env(),
             "state": state,
             "log_url": f"http://airflow.com/{dag.dag_id}/{task_instance.task_id}/log",
             "execution_date": task_instance.execution_date.isoformat(),
             'start_date': task_instance.start_date.isoformat(),
             'end_date': task_instance.end_date.isoformat(),
-            'duration': task_instance.duration,
+            'duration': task_instance.duration or 0,
             'attempt_number': task_instance.prev_attempted_tries,
             "payload": EqVariable("payload"),
         }
         if exception_message and not success:
             expected_graphql_payload["exception_message"] = exception_message
 
         mock_client_upload_result.assert_called()
@@ -223,36 +229,36 @@
                 "success": success,
                 "task": self._get_dag_task_instance_result(task_instance, exception_message),
                 "event_type": "task",
             }
         )
 
     @staticmethod
-    def _create_task_instance(dag_id: str, task_id: str, state: str) -> TaskInstance:
+    def _create_task_instance(dag_id: str, task_id: str, state: str, running: bool = False) -> TaskInstance:
         task_instance = create_autospec(TaskInstance)
         task_instance.task_id = task_id
         task_instance.state = state
         task_instance.log_url = f"http://airflow.com/{dag_id}/{task_instance.task_id}/log"
         task_instance.prev_attempted_tries = 0
-        task_instance.duration = 10.5
+        task_instance.duration = 10.5 if not running else None
         task_instance.execution_date = datetime.now(tz=pytz.UTC) - timedelta(seconds=10)
         task_instance.start_date = datetime.now(tz=pytz.UTC) - timedelta(seconds=9)
         task_instance.end_date = datetime.now(tz=pytz.UTC)
         task_instance.max_tries = 3
         task_instance.try_number = 1
         return task_instance
 
     @staticmethod
     def _get_dag_task_instance_result(task_instance: TaskInstance, exception_message: Optional[str] = None) -> Dict:
         return {
             "task_id": task_instance.task_id,
             "state": task_instance.state,
             "log_url": task_instance.log_url,
             "prev_attempted_tries": task_instance.prev_attempted_tries,
-            "duration": task_instance.duration,
+            "duration": task_instance.duration or 0,
             "execution_date": task_instance.execution_date.isoformat(),
             "start_date": task_instance.start_date.isoformat(),
             "end_date": task_instance.end_date.isoformat(),
             "next_retry_datetime": None,
             "max_tries": task_instance.max_tries,
             "try_number": task_instance.try_number,
             "exception_message": exception_message,
```

### Comparing `airflow_mcd-0.0.8/tests/hooks/test_session_hook.py` & `airflow_mcd-0.1.0/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/tests/operators/test_base_op.py` & `airflow_mcd-0.1.0/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.0.8/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.1.0/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*


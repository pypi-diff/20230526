# Comparing `tmp/SpiffWorkflow-1.2.1.tar.gz` & `tmp/SpiffWorkflow-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpiffWorkflow-1.2.1.tar", last modified: Wed Oct 19 14:19:02 2022, max compression
+gzip compressed data, was "SpiffWorkflow-2.0.0rc0.tar", last modified: Fri May 26 14:05:01 2023, max compression
```

## Comparing `SpiffWorkflow-1.2.1.tar` & `SpiffWorkflow-2.0.0rc0.tar`

### file list

```diff
@@ -1,177 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     7641 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     6539 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5789 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.699230 SpiffWorkflow-1.2.1/SpiffWorkflow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.699230 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/
--rw-r--r--   0 runner    (1001) docker     (121)    12024 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/FeelLikeScriptEngine.py
--rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/PythonScriptEngine.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.699230 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/
--rw-r--r--   0 runner    (1001) docker     (121)    11075 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/BpmnParser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4633 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/ProcessParser.py
--rw-r--r--   0 runner    (1001) docker     (121)    11547 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/TaskParser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/ValidationException.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10538 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/event_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/node_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7136 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/task_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.699230 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/
--rw-r--r--   0 runner    (1001) docker     (121)     7895 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/BpmnSerializer.py
--rw-r--r--   0 runner    (1001) docker     (121)    19468 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/CompactWorkflowSerializer.py
--rw-r--r--   0 runner    (1001) docker     (121)    20727 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/Packager.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14249 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/bpmn_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)    11469 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     4323 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     9901 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/task_spec_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/version_migration.py
--rw-r--r--   0 runner    (1001) docker     (121)    13967 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     9976 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/workflow_spec_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/
--rw-r--r--   0 runner    (1001) docker     (121)     6279 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/BpmnProcessSpec.py
--rw-r--r--   0 runner    (1001) docker     (121)     7805 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/BpmnSpecMixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ExclusiveGateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/InclusiveGateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ManualTask.py
--rw-r--r--   0 runner    (1001) docker     (121)    21712 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/MultiInstanceTask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/NoneTask.py
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ParallelGateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ScriptTask.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ServiceTask.py
--rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/SubWorkflowTask.py
--rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/UnstructuredJoin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/UserTask.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/EndEvent.py
--rw-r--r--   0 runner    (1001) docker     (121)     5605 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/IntermediateEvent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/StartEvent.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14723 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/event_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/event_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    11123 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/parser/
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/parser/CamundaParser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/parser/UserTaskParser.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/parser/business_rule_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/parser/event_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/serializer/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/serializer/task_spec_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/specs/
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/specs/UserTask.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/specs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/specs/events/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/specs/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/camunda/specs/events/event_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.703230 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/engine/
--rw-r--r--   0 runner    (1001) docker     (121)     4739 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/engine/DMNEngine.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.707230 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/parser/
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/parser/BpmnDmnParser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7396 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/parser/DMNParser.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.707230 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/serializer/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3563 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/serializer/task_spec_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.707230 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/specs/
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/specs/BusinessRuleTask.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5503 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/specs/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2696 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10569 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.707230 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    28325 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     3679 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/dotv.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/json.py
--rw-r--r--   0 runner    (1001) docker     (121)    13813 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/prettyxml.py
--rw-r--r--   0 runner    (1001) docker     (121)    32297 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.707230 SpiffWorkflow-1.2.1/SpiffWorkflow/signavio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/signavio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.707230 SpiffWorkflow-1.2.1/SpiffWorkflow/signavio/parser/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/signavio/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/signavio/parser/bpmn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/signavio/parser/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/AcquireMutex.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Cancel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/CancelTask.py
--rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Celery.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Choose.py
--rw-r--r--   0 runner    (1001) docker     (121)     3714 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ExclusiveChoice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3040 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Execute.py
--rw-r--r--   0 runner    (1001) docker     (121)     2582 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Gate.py
--rw-r--r--   0 runner    (1001) docker     (121)    11935 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Join.py
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/LoopResetTask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Merge.py
--rw-r--r--   0 runner    (1001) docker     (121)     5361 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/MultiChoice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3968 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/MultiInstance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ReleaseMutex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/StartTask.py
--rw-r--r--   0 runner    (1001) docker     (121)     5870 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/SubWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ThreadMerge.py
--rw-r--r--   0 runner    (1001) docker     (121)     5209 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ThreadSplit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ThreadStart.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     3802 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Trigger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6469 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/WorkflowSpec.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18676 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/specs/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/parser/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/parser/event_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/parser/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     7072 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/parser/task_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/serializer/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5695 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/serializer/task_spec_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/events/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/events/event_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/events/event_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/manual_task.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/none_task.py
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/script_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/service_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/spiff_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/subworkflow_task.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/specs/user_task.py
--rw-r--r--   0 runner    (1001) docker     (121)    27777 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/SpiffWorkflow/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/util/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/util/deep_merge.py
--rw-r--r--   0 runner    (1001) docker     (121)     8885 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/util/event.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/util/impl.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/util/levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/util/weakmethod.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    14829 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/SpiffWorkflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 14:19:02.699230 SpiffWorkflow-1.2.1/SpiffWorkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6539 2022-10-19 14:19:02.000000 SpiffWorkflow-1.2.1/SpiffWorkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5584 2022-10-19 14:19:02.000000 SpiffWorkflow-1.2.1/SpiffWorkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 14:19:02.000000 SpiffWorkflow-1.2.1/SpiffWorkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-19 14:19:02.000000 SpiffWorkflow-1.2.1/SpiffWorkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-19 14:19:02.000000 SpiffWorkflow-1.2.1/SpiffWorkflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 14:19:02.711230 SpiffWorkflow-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-10-19 14:18:48.000000 SpiffWorkflow-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/FeelLikeScriptEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/PythonScriptEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/PythonScriptEngineEnvironment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/BpmnParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/ProcessParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/TaskParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/ValidationException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/node_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/BPMN20.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/BPMNDI.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/DC.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/DI.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    60913 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/Semantic.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/spec_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/task_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.632638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/event_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.632638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.632638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/process_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.632638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/bpmn_process_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/bpmn_task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/event_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/bpmn_spec_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/end_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/event_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/intermediate_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/start_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/exclusive_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/inclusive_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/manual_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/multiinstance_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/none_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/parallel_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/script_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/service_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/subworkflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/unstructured_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/user_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/CamundaParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/event_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/business_rule_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/event_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/multiinstance_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/user_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/engine/DMNEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/BpmnDmnParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/DMNParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.640638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DC.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    20095 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    22615 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN12.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN13.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMNDI12.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMNDI13.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.640638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.640638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/business_rule_task_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.640638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/dotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/prettyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29876 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/AcquireMutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/CancelTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Choose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ExclusiveChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/MultiChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/MultiInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ReleaseMutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/StartTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/SubWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadStart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/WorkflowSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/event_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/event_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/mixins/service_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/spiff_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/deep_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/weakmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 14:04:51.000000 SpiffWorkflow-2.0.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-26 14:04:51.000000 SpiffWorkflow-2.0.0rc0/setup.py
```

### Comparing `SpiffWorkflow-1.2.1/COPYING` & `SpiffWorkflow-2.0.0rc0/COPYING`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-1.2.1/PKG-INFO` & `SpiffWorkflow-2.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiffWorkflow
-Version: 1.2.1
+Version: 2.0.0rc0
 Summary: A workflow framework and BPMN/DMN Processor
 Home-page: https://github.com/sartography/SpiffWorkflow
 Author: Sartography
 Author-email: dan@sartography.com
 License: lGPLv2
 Keywords: spiff workflow bpmn engine
 Classifier: Development Status :: 4 - Beta
@@ -88,15 +88,15 @@
 ## Tests
 ```
 cd tests/SpiffWorkflow
 coverage run --source=SpiffWorkflow -m unittest discover -v . "*Test.py"
 ```
 
 ## Support
-You can find us on Discord at https://discord.gg/zDEBEnrF
+You can find us on Discord at https://discord.gg/BYHcc7PpUC
 
 Commercial support for SpiffWorkflow is available from
 [Sartography](https://sartography.com)
 
 ## Contribute
 Pull Requests are and always will be welcome!
```

### Comparing `SpiffWorkflow-1.2.1/README.md` & `SpiffWorkflow-2.0.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 ## Tests
 ```
 cd tests/SpiffWorkflow
 coverage run --source=SpiffWorkflow -m unittest discover -v . "*Test.py"
 ```
 
 ## Support
-You can find us on Discord at https://discord.gg/zDEBEnrF
+You can find us on Discord at https://discord.gg/BYHcc7PpUC
 
 Commercial support for SpiffWorkflow is available from
 [Sartography](https://sartography.com)
 
 ## Contribute
 Pull Requests are and always will be welcome!
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/FeelLikeScriptEngine.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/FeelLikeScriptEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf-8 -*-
-
-import re
-import datetime
-import operator
-from datetime import timedelta
-from decimal import Decimal
-from .PythonScriptEngine import PythonScriptEngine
-
-# Copyright (C) 2020 Kelly McDonald
+# Copyright (C) 2020 Kelly McDonald, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
+import re
+import datetime
+import operator
+from datetime import timedelta
+from decimal import Decimal
+from .PythonScriptEngine import PythonScriptEngine
+
 
 def feelConvertTime(datestr,parsestr):
     return datetime.datetime.strptime(datestr,parsestr)
 
 class FeelInterval():
     def __init__(self, begin, end, leftOpen=False, rightOpen=False):
         # pesky thing with python floats and Decimal comparison
@@ -164,15 +164,15 @@
 
     NB:
     Months are defined as 30 days currently - as I am dreading getting into
     Date arithmetic edge cases.
 
     """
     if input[0] != 'P':
-        raise Exception("Oh Crap!")
+        raise Exception("ISO Duration format must begin with the letter P")
     input = input[1:]
     days, time = input.split("T")
     lookups = [("Y",days,timedelta(days=365)),
                ("M", days, timedelta(days=30)),
                ("W", days, timedelta(days=7)),
                ("D", days, timedelta(days=1)),
                ("H", time, timedelta(seconds=60*60)),
@@ -235,15 +235,15 @@
          #               somedict.keys()  - because that is actually in the tests.
          # however, it would be fixed by doing:
          #              x contains( this.dotdict.item )
 
          ('true','True'),
          ('false','False')
     ]
-         
+
 externalFuncs = {
     'feelConvertTime':feelConvertTime,
     'FeelInterval':FeelInterval,
     'FeelNot':FeelNot,
     'Decimal':Decimal,
     'feelConcatenate': feelConcatenate,
     'feelAppend': feelAppend,
@@ -262,16 +262,16 @@
     operations that are done within both BPMN and BMN. Eventually it will also
     serve as a base for FEEL expressions as well
 
     If you are uncomfortable with the use of eval() and exec, then you should
     provide a specialised subclass that parses and executes the scripts /
     expressions in a mini-language of your own.
     """
-    def __init__(self):
-        super().__init__()
+    def __init__(self, environment=None):
+        super().__init__(environment=environment)
 
     def validate(self, expression):
         super().validate(self.patch_expression(expression))
 
     def patch_expression(self, invalid_python, lhs=''):
         if invalid_python is None:
             return None
@@ -302,12 +302,12 @@
     def execute(self, task, script, data, external_methods=None):
         """
         Execute the script, within the context of the specified task
         """
         if external_methods is None:
             external_methods = {}
         external_methods.update(externalFuncs)
-        super(PythonScriptEngine).execute(task, script, external_methods)
+        super().execute(task, script, external_methods)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/manual_task.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,28 @@
-# -*- coding: utf-8 -*-
 # Copyright (C) 2012 Matthew Hampton
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
+from SpiffWorkflow.specs.base import TaskSpec
+
+
+class ManualTask(TaskSpec):
+    """Task Spec for a bpmn:manualTask node."""
+
+    def __init__(self, wf_spec, bpmn_id, **kwargs):
+        super().__init__(wf_spec, bpmn_id, **kwargs)
+        self.manual = True
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/BpmnParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/BpmnParser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,179 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2012 Matthew Hampton
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
 import glob
+import os
 
 from lxml import etree
+from lxml.etree import LxmlError
 
-from SpiffWorkflow.bpmn.specs.events.event_definitions import NoneEventDefinition
+from SpiffWorkflow.bpmn.specs.bpmn_process_spec import BpmnProcessSpec
+from SpiffWorkflow.bpmn.specs.defaults import (
+    UserTask,
+    ManualTask,
+    NoneTask,
+    ScriptTask,
+    ServiceTask,
+    CallActivity,
+    SubWorkflowTask,
+    TransactionSubprocess,
+    InclusiveGateway,
+    ExclusiveGateway,
+    ParallelGateway,
+    StartEvent,
+    EndEvent,
+    IntermediateCatchEvent,
+    IntermediateThrowEvent,
+    SendTask,
+    ReceiveTask,
+    BoundaryEvent,
+    EventBasedGateway
+)
+from SpiffWorkflow.bpmn.specs.event_definitions import NoneEventDefinition, TimerEventDefinition
+from SpiffWorkflow.bpmn.specs.mixins.subworkflow_task import SubWorkflowTask as SubWorkflowTaskMixin
+from SpiffWorkflow.bpmn.specs.mixins.events.start_event import StartEvent as StartEventMixin
 
 from .ValidationException import ValidationException
-from ..specs.BpmnProcessSpec import BpmnProcessSpec
-from ..specs.events import StartEvent, EndEvent, BoundaryEvent, IntermediateCatchEvent, IntermediateThrowEvent
-from ..specs.events import SendTask, ReceiveTask
-from ..specs.SubWorkflowTask import CallActivity, SubWorkflowTask, TransactionSubprocess
-from ..specs.ExclusiveGateway import ExclusiveGateway
-from ..specs.InclusiveGateway import InclusiveGateway
-from ..specs.ManualTask import ManualTask
-from ..specs.NoneTask import NoneTask
-from ..specs.ParallelGateway import ParallelGateway
-from ..specs.ScriptTask import ScriptTask
-from ..specs.ServiceTask import ServiceTask
-from ..specs.UserTask import UserTask
 from .ProcessParser import ProcessParser
+from .node_parser import DEFAULT_NSMAP
+from .spec_description import SPEC_DESCRIPTIONS
 from .util import full_tag, xpath_eval, first
-from .task_parsers import (UserTaskParser, NoneTaskParser, ManualTaskParser,
-                           ExclusiveGatewayParser, ParallelGatewayParser, InclusiveGatewayParser,
-                           CallActivityParser, ScriptTaskParser, SubWorkflowParser,
-                           ServiceTaskParser)
-from .event_parsers import (StartEventParser, EndEventParser, BoundaryEventParser,
-                           IntermediateCatchEventParser, IntermediateThrowEventParser,
-                           SendTaskParser, ReceiveTaskParser)
-
+from .TaskParser import TaskParser
+from .task_parsers import (
+    GatewayParser,
+    ConditionalGatewayParser,
+    CallActivityParser,
+    ScriptTaskParser,
+    SubWorkflowParser,
+)
+from .event_parsers import (
+    EventBasedGatewayParser,
+    StartEventParser, EndEventParser,
+    BoundaryEventParser,
+    IntermediateCatchEventParser,
+    IntermediateThrowEventParser,
+    SendTaskParser,
+    ReceiveTaskParser
+)
+
+
+XSD_PATH = os.path.join(os.path.dirname(__file__), 'schema', 'BPMN20.xsd')
+
+class BpmnValidator:
+
+    def __init__(self, xsd_path=XSD_PATH, imports=None):
+        with open(xsd_path) as xsd:
+            schema = etree.parse(xsd)
+        if imports is not None:
+            for ns, fn in imports.items():
+                elem = etree.Element(
+                    '{http://www.w3.org/2001/XMLSchema}import',
+                    namespace=ns,
+                    schemaLocation=fn
+                )
+                schema.getroot().insert(0, elem)
+        self.validator = etree.XMLSchema(schema)
+
+    def validate(self, bpmn, filename=None):
+        try:
+            self.validator.assertValid(bpmn)
+        except ValidationException as ve:
+            ve.file_name = filename
+            ve.line_number = self.validator.error_log.last_error.line
+        except LxmlError as le:
+            last_error = self.validator.error_log.last_error
+            raise ValidationException(last_error.message, file_name=filename,
+                                      line_number=last_error.line)
 
 class BpmnParser(object):
     """
     The BpmnParser class is a pluggable base class that manages the parsing of
     a set of BPMN files. It is intended that this class will be overriden by an
     application that implements a BPMN engine.
 
     Extension points: OVERRIDE_PARSER_CLASSES provides a map from full BPMN tag
     name to a TaskParser and Task class. PROCESS_PARSER_CLASS provides a
-    subclass of ProcessParser
+    subclass of ProcessParser. DATA_STORE_CLASSES provides a mapping of names to
+    subclasses of BpmnDataStoreSpecification that provide a data store
+    implementation.
     """
 
     PARSER_CLASSES = {
         full_tag('startEvent'): (StartEventParser, StartEvent),
         full_tag('endEvent'): (EndEventParser, EndEvent),
-        full_tag('userTask'): (UserTaskParser, UserTask),
-        full_tag('task'): (NoneTaskParser, NoneTask),
-        full_tag('subProcess'): (SubWorkflowParser, CallActivity),
-        full_tag('manualTask'): (ManualTaskParser, ManualTask),
-        full_tag('exclusiveGateway'): (ExclusiveGatewayParser, ExclusiveGateway),
-        full_tag('parallelGateway'): (ParallelGatewayParser, ParallelGateway),
-        full_tag('inclusiveGateway'): (InclusiveGatewayParser, InclusiveGateway),
+        full_tag('userTask'): (TaskParser, UserTask),
+        full_tag('task'): (TaskParser, NoneTask),
+        full_tag('subProcess'): (SubWorkflowParser, SubWorkflowTask),
+        full_tag('manualTask'): (TaskParser, ManualTask),
+        full_tag('exclusiveGateway'): (ConditionalGatewayParser, ExclusiveGateway),
+        full_tag('parallelGateway'): (GatewayParser, ParallelGateway),
+        full_tag('inclusiveGateway'): (ConditionalGatewayParser, InclusiveGateway),
         full_tag('callActivity'): (CallActivityParser, CallActivity),
         full_tag('transaction'): (SubWorkflowParser, TransactionSubprocess),
         full_tag('scriptTask'): (ScriptTaskParser, ScriptTask),
-        full_tag('serviceTask'): (ServiceTaskParser, ServiceTask),
+        full_tag('serviceTask'): (TaskParser, ServiceTask),
         full_tag('intermediateCatchEvent'): (IntermediateCatchEventParser, IntermediateCatchEvent),
         full_tag('intermediateThrowEvent'): (IntermediateThrowEventParser, IntermediateThrowEvent),
         full_tag('boundaryEvent'): (BoundaryEventParser, BoundaryEvent),
         full_tag('receiveTask'): (ReceiveTaskParser, ReceiveTask),
         full_tag('sendTask'): (SendTaskParser, SendTask),
+        full_tag('eventBasedGateway'): (EventBasedGatewayParser, EventBasedGateway),
     }
 
     OVERRIDE_PARSER_CLASSES = {}
 
     PROCESS_PARSER_CLASS = ProcessParser
 
-    def __init__(self):
+    DATA_STORE_CLASSES = {}
+
+    def __init__(self, namespaces=None, validator=None, spec_descriptions=SPEC_DESCRIPTIONS):
         """
         Constructor.
         """
+        self.namespaces = namespaces or DEFAULT_NSMAP
+        self.validator = validator
+        self.spec_descriptions = spec_descriptions
         self.process_parsers = {}
-        self.process_parsers_by_name = {}
         self.collaborations = {}
         self.process_dependencies = set()
-        self.dmn_dependencies = set()
+        self.messages = {}
+        self.correlations = {}
+        self.data_stores = {}
 
     def _get_parser_class(self, tag):
         if tag in self.OVERRIDE_PARSER_CLASSES:
             return self.OVERRIDE_PARSER_CLASSES[tag]
         elif tag in self.PARSER_CLASSES:
             return self.PARSER_CLASSES[tag]
         return None, None
 
-    def get_process_parser(self, process_id_or_name):
+    def get_process_parser(self, process_id):
         """
         Returns the ProcessParser for the given process ID or name. It matches
         by name first.
         """
-        if process_id_or_name in self.process_parsers_by_name:
-            return self.process_parsers_by_name[process_id_or_name]
-        elif process_id_or_name in self.process_parsers:
-            return self.process_parsers[process_id_or_name]
+        if process_id in self.process_parsers:
+            return self.process_parsers[process_id]
 
     def get_process_ids(self):
         """Returns a list of process IDs"""
         return list(self.process_parsers.keys())
 
     def add_bpmn_file(self, filename):
         """
@@ -128,105 +189,158 @@
         self.add_bpmn_files(glob.glob(g))
 
     def add_bpmn_files(self, filenames):
         """
         Add all filenames in the given list to the parser's set.
         """
         for filename in filenames:
-            f = open(filename, 'r')
-            try:
-                self.add_bpmn_xml(etree.parse(f), filename=filename)
-            finally:
-                f.close()
+            with open(filename, 'r') as f:
+                self.add_bpmn_io(f, filename)
+
+    def add_bpmn_io(self, file_like_object, filename=None):
+        """
+        Add the given BPMN file like object to the parser's set. 
+        """
+        self.add_bpmn_xml(etree.parse(file_like_object), filename)
+
+    def add_bpmn_str(self, bpmn_str, filename=None):
+        """
+        Add the given BPMN string to the parser's set. 
+        """
+        self.add_bpmn_xml(etree.fromstring(bpmn_str), filename)
 
     def add_bpmn_xml(self, bpmn, filename=None):
         """
         Add the given lxml representation of the BPMN file to the parser's set.
 
         :param svg: Optionally, provide the text data for the SVG of the BPMN
           file
         :param filename: Optionally, provide the source filename.
         """
-        xpath = xpath_eval(bpmn)
-        # do a check on our bpmn to ensure that no id appears twice
-        # this *should* be taken care of by our modeler - so this test
-        # should never fail.
-        ids = [x for x in xpath('.//bpmn:*[@id]')]
-        foundids = {}
-        for node in ids:
-            id = node.get('id')
-            if foundids.get(id,None) is not None:
-                raise ValidationException(
-                    'The bpmn document should have no repeating ids but (%s) repeats'%id,
-                    node=node,
-                    filename=filename)
-            else:
-                foundids[id] = 1
-
-        for process in xpath('.//bpmn:process'):
-            self.create_parser(process, xpath, filename)
+        if self.validator:
+            self.validator.validate(bpmn, filename)
 
-        self._find_dependencies(xpath)
+        # we need to parse the data stores before _add_process since it creates
+        # the parser instances, which need to know about the data stores to
+        # resolve data references.
+        self._add_data_stores(bpmn)
+
+        self._add_processes(bpmn, filename)
+        self._add_collaborations(bpmn)
+        self._add_messages(bpmn)
+        self._add_correlations(bpmn)
+
+    def _add_processes(self, bpmn, filename=None):
+        for process in bpmn.xpath('.//bpmn:process', namespaces=self.namespaces):
+            self._find_dependencies(process)
+            self.create_parser(process, filename)
 
-        collaboration = first(xpath('.//bpmn:collaboration'))
+    def _add_collaborations(self, bpmn):
+        collaboration = first(bpmn.xpath('.//bpmn:collaboration', namespaces=self.namespaces))
         if collaboration is not None:
             collaboration_xpath = xpath_eval(collaboration)
             name = collaboration.get('id')
             self.collaborations[name] = [ participant.get('processRef') for participant in collaboration_xpath('.//bpmn:participant') ]
 
-    def _find_dependencies(self, xpath):
-        """Locate all calls to external BPMN and DMN files, and store their
-        ids in our list of dependencies"""
-        for call_activity in xpath('.//bpmn:callActivity'):
+    def _add_messages(self, bpmn):
+        for message in bpmn.xpath('.//bpmn:message', namespaces=self.namespaces):
+            if message.attrib.get("id") is None:
+                raise ValidationException(
+                    "Message identifier is missing from bpmn xml"
+                )
+            self.messages[message.attrib.get("id")] = message.attrib.get("name")
+
+    def _add_correlations(self, bpmn):
+        for correlation in bpmn.xpath('.//bpmn:correlationProperty', namespaces=self.namespaces):
+            correlation_identifier = correlation.attrib.get("id")
+            if correlation_identifier is None:
+                raise ValidationException("Correlation identifier is missing from bpmn xml")
+            correlation_property_retrieval_expressions = correlation.xpath(
+                ".//bpmn:correlationPropertyRetrievalExpression", namespaces = self.namespaces)
+            if not correlation_property_retrieval_expressions:
+                raise ValidationException(
+                    f"Correlation is missing correlation property retrieval expressions: {correlation_identifier}"
+                )
+            retrieval_expressions = []
+            for cpre in correlation_property_retrieval_expressions:
+                message_model_identifier = cpre.attrib.get("messageRef")
+                if message_model_identifier is None:
+                    raise ValidationException(
+                        f"Message identifier is missing from correlation property: {correlation_identifier}"
+                    )
+                children = cpre.getchildren()
+                expression = children[0].text if len(children) > 0 else None
+                retrieval_expressions.append({"messageRef": message_model_identifier,
+                                             "expression": expression})
+            self.correlations[correlation_identifier] = {
+                "name": correlation.attrib.get("name"),
+                "retrieval_expressions": retrieval_expressions
+            }
+
+    def _add_data_stores(self, bpmn):
+        for data_store in bpmn.xpath('.//bpmn:dataStore', namespaces=self.namespaces):
+            data_store_id = data_store.attrib.get("id")
+            if data_store_id is None:
+                raise ValidationException(
+                    "Data Store identifier is missing from bpmn xml"
+                )
+            data_store_name = data_store.attrib.get("name")
+            if data_store_name is None:
+                raise ValidationException(
+                    "Data Store name is missing from bpmn xml"
+                )
+            if data_store_name not in self.DATA_STORE_CLASSES:
+                raise ValidationException(
+                    f"Data Store with name {data_store_name} has no implementation"
+                )
+            data_store_spec = self.DATA_STORE_CLASSES[data_store_name](
+                data_store_id,
+                data_store_name,
+                data_store.attrib.get('capacity'),
+                data_store.attrib.get('isUnlimited'))
+            self.data_stores[data_store_id] = data_store_spec
+
+    def _find_dependencies(self, process):
+        """Locate all calls to external BPMN, and store their ids in our list of dependencies"""
+        for call_activity in process.xpath('.//bpmn:callActivity', namespaces=self.namespaces):
             self.process_dependencies.add(call_activity.get('calledElement'))
-        parser_cls, cls = self._get_parser_class(full_tag('businessRuleTask'))
-        if parser_cls:
-            for business_rule in xpath('.//bpmn:businessRuleTask'):
-                self.dmn_dependencies.add(parser_cls.get_decision_ref(business_rule))
-
-
-    def create_parser(self, node, doc_xpath, filename=None, lane=None):
-        parser = self.PROCESS_PARSER_CLASS(self, node, filename=filename, doc_xpath=doc_xpath, lane=lane)
-        if parser.get_id() in self.process_parsers:
-            raise ValidationException('Duplicate process ID', node=node, filename=filename)
-        if parser.get_name() in self.process_parsers_by_name:
-            raise ValidationException('Duplicate process name', node=node, filename=filename)
-        self.process_parsers[parser.get_id()] = parser
-        self.process_parsers_by_name[parser.get_name()] = parser
 
-    def get_dependencies(self):
-        return self.process_dependencies.union(self.dmn_dependencies)
+    def create_parser(self, node, filename=None, lane=None):
+        parser = self.PROCESS_PARSER_CLASS(self, node, self.namespaces, self.data_stores, filename=filename, lane=lane)
+        if parser.bpmn_id in self.process_parsers:
+            raise ValidationException(f'Duplicate process ID: {parser.bpmn_id}', node=node, file_name=filename)
+        self.process_parsers[parser.bpmn_id] = parser
 
     def get_process_dependencies(self):
         return self.process_dependencies
 
-    def get_dmn_dependencies(self):
-        return self.dmn_dependencies
-
-    def get_spec(self, process_id_or_name):
+    def get_spec(self, process_id, required=True):
         """
         Parses the required subset of the BPMN files, in order to provide an
         instance of BpmnProcessSpec (i.e. WorkflowSpec)
         for the given process ID or name. The Name is matched first.
         """
-        parser = self.get_process_parser(process_id_or_name)
-        if parser is None:
+        parser = self.get_process_parser(process_id)
+        if required and parser is None:
             raise ValidationException(
-                f"The process '{process_id_or_name}' was not found. "
+                f"The process '{process_id}' was not found. "
                 f"Did you mean one of the following: "
                 f"{', '.join(self.get_process_ids())}?")
-        return parser.get_spec()
+        elif parser is not None:
+            return parser.get_spec()
 
-    def get_subprocess_specs(self, name, specs=None):
+    def get_subprocess_specs(self, name, specs=None, require_call_activity_specs=True):
         used = specs or {}
         wf_spec = self.get_spec(name)
         for task_spec in wf_spec.task_specs.values():
-            if isinstance(task_spec, SubWorkflowTask) and task_spec.spec not in used:
-                used[task_spec.spec] = self.get_spec(task_spec.spec)
-                self.get_subprocess_specs(task_spec.spec, used)
+            if isinstance(task_spec, SubWorkflowTaskMixin) and task_spec.spec not in used:
+                subprocess_spec = self.get_spec(task_spec.spec, required=require_call_activity_specs)
+                used[task_spec.spec] = subprocess_spec
+                if subprocess_spec is not None:
+                    self.get_subprocess_specs(task_spec.spec, used)
         return used
 
     def find_all_specs(self):
         # This is a little convoluted, but we might add more processes as we generate
         # the dictionary if something refers to another subprocess that we haven't seen.
         processes = dict((id, self.get_spec(id)) for id in self.get_process_ids())
         while processes.keys() != self.process_parsers.keys():
@@ -234,20 +348,28 @@
                 processes[process_id] = self.get_spec(process_id)
         return processes
 
     def get_collaboration(self, name):
         self.find_all_specs()
         spec = BpmnProcessSpec(name)
         subprocesses = {}
-        start = StartEvent(spec, 'Start Collaboration', NoneEventDefinition())
+        participant_type = self._get_parser_class(full_tag('callActivity'))[1]
+        start_type = self._get_parser_class(full_tag('startEvent'))[1]
+        end_type = self._get_parser_class(full_tag('endEvent'))[1]
+        start = start_type(spec, 'Start Collaboration', NoneEventDefinition())
         spec.start.connect(start)
-        end = EndEvent(spec, 'End Collaboration', NoneEventDefinition())
+        end = end_type(spec, 'End Collaboration', NoneEventDefinition())
         end.connect(spec.end)
         for process in self.collaborations[name]:
             process_parser = self.get_process_parser(process)
             if process_parser and process_parser.process_executable:
-                participant = CallActivity(spec, process, process)
-                start.connect(participant)
-                participant.connect(end)
-                subprocesses[process] = self.get_spec(process)
+                sp_spec = self.get_spec(process)
+                subprocesses[process] = sp_spec
                 subprocesses.update(self.get_subprocess_specs(process))
+                if len([s for s in sp_spec.task_specs.values() if 
+                        isinstance(s, StartEventMixin) and 
+                        isinstance(s.event_definition, (NoneEventDefinition, TimerEventDefinition))
+                ]):
+                    participant = participant_type(spec, process, process)
+                    start.connect(participant)
+                    participant.connect(end)
         return spec, subprocesses
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/TaskParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/TaskParser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,247 +1,266 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
-import sys
-import traceback
-from .ValidationException import ValidationException
-from ..specs.NoneTask import NoneTask
-from ..specs.ScriptTask import ScriptTask
-from ..specs.UserTask import UserTask
-from ..specs.events import _BoundaryEventParent, CancelEventDefinition
-from ..specs.MultiInstanceTask import getDynamicMIClass
-from ..specs.SubWorkflowTask import CallActivity, TransactionSubprocess, SubWorkflowTask
-from ..specs.ExclusiveGateway import ExclusiveGateway
-from ...dmn.specs.BusinessRuleTask import BusinessRuleTask
-from ...operators import Attrib, PathAttrib
-from .util import one, first
-from .node_parser import NodeParser
-
-STANDARDLOOPCOUNT = '25'
+from SpiffWorkflow.bpmn.specs.mixins.subworkflow_task import TransactionSubprocess
+from SpiffWorkflow.bpmn.specs.mixins.exclusive_gateway import ExclusiveGateway
+from SpiffWorkflow.bpmn.specs.mixins.inclusive_gateway import InclusiveGateway
+from SpiffWorkflow.bpmn.specs.defaults import (
+    StandardLoopTask,
+    SequentialMultiInstanceTask,
+    ParallelMultiInstanceTask
+)
+from SpiffWorkflow.bpmn.specs.control import _BoundaryEventParent
+from SpiffWorkflow.bpmn.specs.event_definitions import CancelEventDefinition
+from SpiffWorkflow.bpmn.specs.data_spec import TaskDataReference
 
-CAMUNDA_MODEL_NS = 'http://camunda.org/schema/1.0/bpmn'
+from .util import one
+from .node_parser import NodeParser
+from .ValidationException import ValidationException
 
 
 class TaskParser(NodeParser):
     """
     This class parses a single BPMN task node, and returns the Task Spec for
     that node.
 
     It also results in the recursive parsing of connected tasks, connecting all
     outgoing transitions, once the child tasks have all been parsed.
     """
 
-    def __init__(self, process_parser, spec_class, node, lane=None):
+    # I hate myself for this.  I wanted to at least relegate it to the top-level
+    # parser where the rest of the similar nonsense is, but it's inaccessible here.
+    STANDARD_LOOP_CLASS = StandardLoopTask
+    PARALLEL_MI_CLASS = ParallelMultiInstanceTask
+    SEQUENTIAL_MI_CLASS = SequentialMultiInstanceTask
+
+    def __init__(self, process_parser, spec_class, node, nsmap=None, lane=None):
         """
         Constructor.
 
         :param process_parser: the owning process parser instance
         :param spec_class: the type of spec that should be created. This allows
           a subclass of BpmnParser to provide a specialised spec class, without
           extending the TaskParser.
         :param node: the XML node for this task
         """
-        super().__init__(node, process_parser.filename, process_parser.doc_xpath, lane)
+        super().__init__(node, nsmap, filename=process_parser.filename, lane=lane)
         self.process_parser = process_parser
         self.spec_class = spec_class
         self.spec = self.process_parser.spec
 
-    def _set_multiinstance_attributes(self, is_sequential, expanded, loop_count,
-                                      loop_task=False, element_var=None, collection=None, completion_condition=None):
-        # This should be replaced with its own task parser (though I'm not sure how feasible this is given
-        # the current parser achitecture).  We should also consider separate classes for loop vs
-        # multiinstance because having all these optional attributes is a nightmare
-
-        if not isinstance(self.task, (NoneTask, UserTask, BusinessRuleTask, ScriptTask, CallActivity, SubWorkflowTask)):
-            raise ValidationException(
-                f'Unsupported MultiInstance Task: {self.task.__class__}',
-                node=self.node,
-                filename=self.filename)
-
-        self.task.loopTask = loop_task
-        self.task.isSequential = is_sequential
-        self.task.expanded = expanded
-        # make dot notation compatible with bmpmn path notation.
-        self.task.times = PathAttrib(loop_count.replace('.', '/')) if loop_count.find('.') > 0 else Attrib(loop_count)
-        self.task.elementVar = element_var
-        self.task.collection = collection
-        self.task.completioncondition = completion_condition
-
-        self.task.prevtaskclass = self.task.__module__ + "." + self.task.__class__.__name__
-        newtaskclass = getDynamicMIClass(self.get_id(),self.task.__class__)
-        self.task.__class__ = newtaskclass
-
-    def _detect_multiinstance(self):
-
-        multiinstance_element = first(self.xpath('./bpmn:multiInstanceLoopCharacteristics'))
-        if multiinstance_element is not None:
-            is_sequential = multiinstance_element.get('isSequential') == 'true'
-
-            element_var_text = multiinstance_element.attrib.get('{' + CAMUNDA_MODEL_NS + '}elementVariable')
-            collection_text = multiinstance_element.attrib.get('{' + CAMUNDA_MODEL_NS + '}collection')
-
-            loop_cardinality = first(self.xpath('./bpmn:multiInstanceLoopCharacteristics/bpmn:loopCardinality'))
-            if loop_cardinality is not None:
-                loop_count = loop_cardinality.text
-            elif collection_text is not None:
-                loop_count = collection_text
+    def _copy_task_attrs(self, original):
+
+        self.task.inputs = original.inputs
+        self.task.outputs = original.outputs
+        self.task.io_specification = original.io_specification
+        self.task.data_input_associations = original.data_input_associations
+        self.task.data_output_associations = original.data_output_associations
+        self.task.description = original.description
+
+        original.inputs = [self.task]
+        original.outputs = []
+        original.io_specification = None
+        original.data_input_associations = []
+        original.data_output_associations = []
+        original.name = f'{original.name} [child]'
+        self.task.task_spec = original.name
+        self.spec.task_specs[original.name] = original
+
+    def _add_loop_task(self, loop_characteristics):
+
+        maximum = loop_characteristics.attrib.get('loopMaximum')
+        if maximum is not None:
+            maximum = int(maximum)
+        condition = self.xpath('./bpmn:standardLoopCharacteristics/bpmn:loopCondition')
+        condition = condition[0].text if len(condition) > 0 else None
+        test_before = loop_characteristics.get('testBefore', 'false') == 'true'
+        if maximum is None and condition is None:
+            self.raise_validation_exception('A loopMaximum or loopCondition must be specified for Loop Tasks')
+
+        original = self.spec.task_specs.pop(self.task.name)
+        self.task = self.STANDARD_LOOP_CLASS(self.spec, original.name, '', maximum, condition, test_before)
+        self._copy_task_attrs(original)
+
+    def _add_multiinstance_task(self, loop_characteristics):
+        
+        sequential = loop_characteristics.get('isSequential') == 'true'
+        prefix = 'bpmn:multiInstanceLoopCharacteristics'
+        cardinality = self.xpath(f'./{prefix}/bpmn:loopCardinality')
+        loop_input = self.xpath(f'./{prefix}/bpmn:loopDataInputRef')
+        if len(cardinality) == 0 and len(loop_input) == 0:
+            self.raise_validation_exception("A multiinstance task must specify a cardinality or a loop input data reference")
+        elif len(cardinality) > 0 and len(loop_input) > 0:
+            self.raise_validation_exception("A multiinstance task must specify exactly one of cardinality or loop input data reference")
+        cardinality = cardinality[0].text if len(cardinality) > 0 else None
+
+        loop_input = loop_input[0].text if len(loop_input) > 0 else None
+        if loop_input is not None:
+            if self.task.io_specification is not None:
+                try:
+                    loop_input = [v for v in self.task.io_specification.data_inputs if v.name == loop_input][0]
+                except:
+                    self.raise_validation_exception('The loop input data reference is missing from the IO specification')
             else:
-                loop_count = '1'
+                loop_input = TaskDataReference(loop_input)
 
-            if collection_text is not None:
-                collection = PathAttrib(collection_text.replace('.', '/')) if collection_text.find('.') > 0 else Attrib(collection_text)
+        input_item = self.xpath(f'./{prefix}/bpmn:inputDataItem')
+        input_item = self.create_data_spec(input_item[0], TaskDataReference) if len(input_item) > 0 else None
+
+        loop_output = self.xpath(f'./{prefix}/bpmn:loopDataOutputRef')
+        loop_output = loop_output[0].text if len(loop_output) > 0 else None
+        if loop_output is not None:
+            if self.task.io_specification is not None:
+                try:
+                    refs = set(self.task.io_specification.data_inputs + self.task.io_specification.data_outputs)
+                    loop_output = [v for v in refs if v.name == loop_output][0]
+                except:
+                    self.raise_validation_exception('The loop output data reference is missing from the IO specification')
             else:
-                collection = None
+                loop_output = TaskDataReference(loop_output)
+
+        output_item = self.xpath(f'./{prefix}/bpmn:outputDataItem')
+        output_item = self.create_data_spec(output_item[0], TaskDataReference) if len(output_item) > 0 else None
 
-            completion_condition = first(self.xpath('./bpmn:multiInstanceLoopCharacteristics/bpmn:completionCondition'))
-            if completion_condition is not None:
-                completion_condition = completion_condition.text
-
-            self._set_multiinstance_attributes(is_sequential, 1, loop_count,
-                                               element_var=element_var_text,
-                                               collection=collection,
-                                               completion_condition=completion_condition)
+        condition = self.xpath(f'./{prefix}/bpmn:completionCondition')
+        condition = condition[0].text if len(condition) > 0 else None
 
-        elif len(self.xpath('./bpmn:standardLoopCharacteristics')) > 0:
-            self._set_multiinstance_attributes(True, 25, STANDARDLOOPCOUNT, loop_task=True)
+        original = self.spec.task_specs.pop(self.task.name)
+        params = {
+            'task_spec': '', 
+            'cardinality': cardinality, 
+            'data_input': loop_input,
+            'data_output':loop_output,
+            'input_item': input_item,
+            'output_item': output_item,
+            'condition': condition,
+        }
+        if sequential:
+            self.task = self.SEQUENTIAL_MI_CLASS(self.spec, original.name, **params)
+        else:
+            self.task = self.PARALLEL_MI_CLASS(self.spec, original.name, **params)
+        self._copy_task_attrs(original)
+
+    def _add_boundary_event(self, children):
+
+        parent = _BoundaryEventParent(
+            self.spec, '%s.BoundaryEventParent' % self.bpmn_id,
+            self.task, lane=self.task.lane)
+        self.process_parser.parsed_nodes[self.node.get('id')] = parent
+        parent.connect(self.task)
+        for event in children:
+            child = self.process_parser.parse_node(event)
+            if isinstance(child.event_definition, CancelEventDefinition) \
+              and not isinstance(self.task, TransactionSubprocess):
+                self.raise_validation_exception('Cancel Events may only be used with transactions')
+            parent.connect(child)
+        return parent
 
     def parse_node(self):
         """
         Parse this node, and all children, returning the connected task spec.
         """
         try:
             self.task = self.create_task()
             # Why do we just set random attributes willy nilly everywhere in the code????
             # And we still pass around a gigantic kwargs dict whenever we create anything!
             self.task.extensions = self.parse_extensions()
-            self.task.documentation = self.parse_documentation()
-            # And now I have to add more of the same crappy thing.
-            self.task.data_input_associations = self.parse_incoming_data_references()
-            self.task.data_output_associations = self.parse_outgoing_data_references()
 
-            self._detect_multiinstance()
+            io_spec = self.xpath('./bpmn:ioSpecification')
+            if len(io_spec) > 0:
+                self.task.io_specification = self.parse_io_spec()
+
+            loop_characteristics = self.xpath('./bpmn:standardLoopCharacteristics')
+            if len(loop_characteristics) > 0:
+                self._add_loop_task(loop_characteristics[0])
+
+            mi_loop_characteristics = self.xpath('./bpmn:multiInstanceLoopCharacteristics')
+            if len(mi_loop_characteristics) > 0:
+                self._add_multiinstance_task(mi_loop_characteristics[0])
 
-            boundary_event_nodes = self.doc_xpath('.//bpmn:boundaryEvent[@attachedToRef="%s"]' % self.get_id())
+            boundary_event_nodes = self.doc_xpath('.//bpmn:boundaryEvent[@attachedToRef="%s"]' % self.bpmn_id)
             if boundary_event_nodes:
-                parent_task = _BoundaryEventParent(
-                    self.spec, '%s.BoundaryEventParent' % self.get_id(),
-                    self.task, lane=self.task.lane)
-                self.process_parser.parsed_nodes[
-                    self.node.get('id')] = parent_task
-                parent_task.connect_outgoing(
-                    self.task, '%s.FromBoundaryEventParent' % self.get_id(),
-                    None, None)
-                for boundary_event in boundary_event_nodes:
-                    b = self.process_parser.parse_node(boundary_event)
-                    if isinstance(b.event_definition, CancelEventDefinition) \
-                      and not isinstance(self.task, TransactionSubprocess):
-                        raise ValidationException(
-                            'Cancel Events may only be used with transactions',
-                            node=self.node,
-                            filename=self.filename)
-                    parent_task.connect_outgoing(
-                        b,
-                        '%s.FromBoundaryEventParent' % boundary_event.get(
-                            'id'),
-                        None, None)
+                parent = self._add_boundary_event(boundary_event_nodes)
             else:
-                self.process_parser.parsed_nodes[
-                    self.node.get('id')] = self.task
+                self.process_parser.parsed_nodes[self.node.get('id')] = self.task
 
             children = []
-            outgoing = self.doc_xpath('.//bpmn:sequenceFlow[@sourceRef="%s"]' % self.get_id())
+            outgoing = self.doc_xpath('.//bpmn:sequenceFlow[@sourceRef="%s"]' % self.bpmn_id)
             if len(outgoing) > 1 and not self.handles_multiple_outgoing():
-                raise ValidationException(
-                    'Multiple outgoing flows are not supported for '
-                    'tasks of type',
-                    node=self.node,
-                    filename=self.filename)
+                self.raise_validation_exception('Multiple outgoing flows are not supported for tasks of type')
             for sequence_flow in outgoing:
                 target_ref = sequence_flow.get('targetRef')
                 try:
                     target_node = one(self.doc_xpath('.//bpmn:*[@id="%s"]'% target_ref))
                 except:
-                    raise ValidationException(
-                        'When looking for a task spec, we found two items, '
-                        'perhaps a form has the same ID? (%s)' % target_ref,
-                        node=self.node,
-                        filename=self.filename)
+                    self.raise_validation_exception('When looking for a task spec, we found two items, '
+                        'perhaps a form has the same ID? (%s)' % target_ref)
 
                 c = self.process_parser.parse_node(target_node)
-                position = c.position
+                position = self.get_position(target_node)
                 children.append((position, c, target_node, sequence_flow))
 
             if children:
                 # Sort children by their y coordinate.
+                # Why??  Isn't the point of parallel tasks that they can be executed in any order (or simultaneously)?
+                # And what if they're arranged horizontally?
                 children = sorted(children, key=lambda tup: float(tup[0]["y"]))
 
                 default_outgoing = self.node.get('default')
-                if not default_outgoing:
-                    if len(children) == 1 or not isinstance(self.task, ExclusiveGateway):
-                        (position, c, target_node, sequence_flow) = children[0]
+                if len(children) == 1 and isinstance(self.task, (ExclusiveGateway, InclusiveGateway)):
+                    (position, c, target_node, sequence_flow) = children[0]
+                    if self.parse_condition(sequence_flow) is None:
                         default_outgoing = sequence_flow.get('id')
 
                 for (position, c, target_node, sequence_flow) in children:
-                    self.connect_outgoing(
-                        c, target_node, sequence_flow,
-                        sequence_flow.get('id') == default_outgoing)
-
-            return parent_task if boundary_event_nodes else self.task
-        except ValidationException:
-            raise
+                    self.connect_outgoing(c, sequence_flow, sequence_flow.get('id') == default_outgoing)
+
+            return parent if boundary_event_nodes else self.task
+        except ValidationException as ve:
+            raise ve
         except Exception as ex:
-            exc_info = sys.exc_info()
-            tb = "".join(traceback.format_exception(
-                exc_info[0], exc_info[1], exc_info[2]))
-            raise ValidationException("%r" % (ex), node=self.node, filename=self.filename)
+            raise ValidationException("%r" % (ex), node=self.node, file_name=self.filename)
 
     def get_task_spec_name(self, target_ref=None):
         """
         Returns a unique task spec name for this task (or the targeted one)
         """
-        return target_ref or self.get_id()
+        return target_ref or self.bpmn_id
 
     def create_task(self):
         """
         Create an instance of the task appropriately. A subclass can override
         this method to get extra information from the node.
         """
-        return self.spec_class(self.spec, self.get_task_spec_name(),
-                               lane=self.lane,
-                               description=self.node.get('name', None),
-                               position=self.position)
+        return self.spec_class(self.spec, self.bpmn_id, **self.bpmn_attributes)
 
-    def connect_outgoing(self, outgoing_task, outgoing_task_node,
-                         sequence_flow_node, is_default):
+    def connect_outgoing(self, outgoing_task, sequence_flow_node, is_default):
         """
         Connects this task to the indicating outgoing task, with the details in
         the sequence flow. A subclass can override this method to get extra
         information from the node.
         """
-        self.task.connect_outgoing(
-            outgoing_task, sequence_flow_node.get('id'),
-            sequence_flow_node.get(
-                'name', None),
-            self.parse_documentation(sequence_flow_node))
+        self.task.connect(outgoing_task)
 
     def handles_multiple_outgoing(self):
         """
         A subclass should override this method if the task supports multiple
         outgoing sequence flows.
         """
         return False
+
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/impl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,26 @@
-# -*- coding: utf-8 -*-
-# Copyright (C) 2012 Matthew Hampton
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
+import sys
+
+
+def get_class(full_class_name):
+    parts = full_class_name.rsplit('.', 1)
+    module_name = parts[0]
+    class_name = parts[1]
+    __import__(module_name)
+    return getattr(sys.modules[module_name], class_name)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/parser/util.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# -*- coding: utf-8 -*-
 # Copyright (C) 2012 Matthew Hampton
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# -*- coding: utf-8 -*-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2023 Sartography
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
-from .workflow import BpmnWorkflowSerializer
-from .bpmn_converters import BpmnDataConverter
+from SpiffWorkflow.exceptions import WorkflowException
+
+class VersionMigrationError(WorkflowException):
+    pass
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/bpmn_converters.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/workflow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,345 +1,311 @@
-from functools import partial
-
+# Copyright (C) 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3.0 of the License, or (at your option) any later version.
+#
+# SpiffWorkflow is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
+
+import json
+import gzip
+from copy import deepcopy
 from uuid import UUID
-from datetime import datetime, timedelta
-
-from SpiffWorkflow.bpmn.specs.BpmnProcessSpec import BpmnDataSpecification
-
-from .dictionary import DictionaryConverter
 
-from ..specs.events import SignalEventDefinition, MessageEventDefinition, NoneEventDefinition
-from ..specs.events import TimerEventDefinition, CycleTimerEventDefinition, TerminateEventDefinition
-from ..specs.events import ErrorEventDefinition, EscalationEventDefinition, CancelEventDefinition
-from ..specs.events.event_definitions import CorrelationProperty, NamedEventDefinition
+from SpiffWorkflow.task import Task
+from SpiffWorkflow.bpmn.workflow import BpmnMessage, BpmnWorkflow
+from SpiffWorkflow.bpmn.specs.mixins.subworkflow_task import SubWorkflowTask
+
+from .migration.version_migration import MIGRATIONS
+from .helpers.registry import DefaultRegistry
+from .helpers.dictionary import DictionaryConverter
+
+from .process_spec import BpmnProcessSpecConverter
+from .data_spec import BpmnDataObjectConverter, TaskDataReferenceConverter, IOSpecificationConverter
+from .task_spec import DEFAULT_TASK_SPEC_CONVERTER_CLASSES
+from .event_definition import DEFAULT_EVENT_CONVERTERS
+
+DEFAULT_SPEC_CONFIG = {
+    'process': BpmnProcessSpecConverter,
+    'data_specs': [IOSpecificationConverter, BpmnDataObjectConverter, TaskDataReferenceConverter],
+    'task_specs': DEFAULT_TASK_SPEC_CONVERTER_CLASSES,
+    'event_definitions': DEFAULT_EVENT_CONVERTERS,
+}
 
-from ..specs.BpmnSpecMixin import BpmnSpecMixin, SequenceFlow
-from ...operators import Attrib, PathAttrib
 
-
-class BpmnDataConverter(DictionaryConverter):
+class BpmnWorkflowSerializer:
     """
-    The default converter for task and workflow data.  It allows some commonly used python objects
-    to be converted to a form that can be serialized with JSOM
+    This class implements a customizable BPMN Workflow serializer, based on a Workflow Spec Converter
+    and a Data Converter.
 
-    It also serves as a simple example for anyone who needs custom data serialization.  If you have
-    custom objects or python objects not included here in your workflow/task data, then you should
-    replace or extend this with one that can handle the contents of your workflow.
-    """
-    def __init__(self):
+    The goal is to provide modular serialization capabilities.
 
-        super().__init__()
-        self.register(UUID, lambda v: { 'value': str(v) }, lambda v: UUID(v['value']))
-        self.register(datetime, lambda v:  { 'value': v.isoformat() }, lambda v: datetime.fromisoformat(v['value']))
-        self.register(timedelta, lambda v: { 'days': v.days, 'seconds': v.seconds }, lambda v: timedelta(**v))
-
-    def convert(self, obj):
-        self.clean(obj)
-        return super().convert(obj)
-
-    def clean(self, obj):
-        # This removes functions and other callables from task data.
-        # By default we don't want to serialize these
-        if isinstance(obj, dict):
-            items = [ (k, v) for k, v in obj.items() ]
-            for key, value in items:
-                if callable(value):
-                    del obj[key]
-
-class BpmnDataSpecificationConverter:
+    You'll need to configure a Workflow Spec Converter with converters for any task, data, or event types
+    present in your workflows.
 
-    @staticmethod
-    def to_dict(data_spec):
-        return { 'name': data_spec.name, 'description': data_spec.description }
+    If you have implemented any custom specs, you'll need to write a converter to handle them and
+    replace the converter from the default confiuration with your own.
 
-    @staticmethod
-    def from_dict(dct):
-        return BpmnDataSpecification(**dct)
+    If your workflow contains non-JSON-serializable objects, you'll need to extend or replace the
+    default data converter with one that will handle them.  This converter needs to implement
+    `convert` and `restore` methods.
 
+    Serialization occurs in two phases: the first is to convert everything in the workflow to a
+    dictionary containing only JSON-serializable objects and the second is dumping to JSON.
 
-
-class BpmnTaskSpecConverter(DictionaryConverter):
-    """
-    This the base Task Spec Converter.
-
-    It contains methods for parsing generic and BPMN task spec attributes.
-
-    If you have extended any of the the BPMN tasks with custom functionality, you'll need to
-    implement a converter for those task spec types.  You'll need to implement the `to_dict` and
-    `from_dict` methods on any inheriting classes.
-
-    The default task spec converters are in `task_converters`; the `camunda` and `dmn`
-    serialization packages contain other examples.
+    This means that you can call the `workflow_to_dict` or `workflow_from_dict` methods separately from
+    conversion to JSON for further manipulation of the state, or selective serialization of only certain
+    parts of the workflow more conveniently.  You can of course call methods from the Workflow Spec and
+    Data Converters via the `spec_converter` and `data_converter` attributes as well to bypass the
+    overhead of converting or restoring the entire thing.
     """
 
-    def __init__(self, spec_class, data_converter, typename=None):
-        """The default task spec converter.  This will generally be registered with a workflow
-        spec converter.
-
-        Task specs can contain arbitrary data, though none of the default BPMN tasks do.  We
-        may remove this functionality in the future.  Therefore, the data_converter can be
-        `None`; if this is the case, task spec attributes that can contain arbitrary data will be
-        ignored.
-
-        :param spec_class: the class defining the task type
-        :param data_converter: a converter for custom data (can be None)
-        :param typename: an optional typename for the object registration
-        """
-        super().__init__()
-        self.spec_class = spec_class
-        self.data_converter = data_converter
-        self.typename = typename if typename is not None else spec_class.__name__
-
-        event_definitions = [ NoneEventDefinition, CancelEventDefinition, TerminateEventDefinition,
-            SignalEventDefinition, MessageEventDefinition, ErrorEventDefinition, EscalationEventDefinition,
-            TimerEventDefinition, CycleTimerEventDefinition ]
-
-        for event_definition in event_definitions:
-            self.register(
-                event_definition,
-                self.event_definition_to_dict,
-                partial(self.event_defintion_from_dict, event_definition)
-            )
-
-        self.register(SequenceFlow, self.sequence_flow_to_dict, self.sequence_flow_from_dict)
-        self.register(Attrib, self.attrib_to_dict, partial(self.attrib_from_dict, Attrib))
-        self.register(PathAttrib, self.attrib_to_dict, partial(self.attrib_from_dict, PathAttrib))
-        self.register(BpmnDataSpecification, BpmnDataSpecificationConverter.to_dict, BpmnDataSpecificationConverter.from_dict)
+    # This is the default version set on the workflow, it can be overwritten
+    # using the configure_workflow_spec_converter.
+    VERSION = "1.2"
+    VERSION_KEY = "serializer_version"
+    DEFAULT_JSON_ENCODER_CLS = None
+    DEFAULT_JSON_DECODER_CLS = None
 
-    def to_dict(self, spec):
-        """
-        The convert method that will be called when a Task Spec Converter is registered with a
-        Workflow Spec Converter.
+    @staticmethod
+    def configure_workflow_spec_converter(spec_config=None, registry=None):
         """
-        raise NotImplementedError
+        This method can be used to create a spec converter that uses custom specs.
 
-    def from_dict(self, dct):
-        """
-        The restore method that will be called when a Task Spec Converter is registered with a
-        Workflow Spec Converter.
+        The task specs may contain arbitrary data, though none of the default task specs use it.  We don't
+        recommend that you do this, as we may disallow it in the future.  However, if you have task spec data,
+        then you'll also need to make sure it can be serialized.
+
+        The workflow spec serializer is based on the `DictionaryConverter` in the `helpers` package.  You can
+        create one of your own, add custom data serializtion to that and pass that in as the `registry`.  The
+        conversion classes in the spec_config will be added this "registry" and any classes with entries there
+        will be serialized/deserialized.
+
+        See the documentation for `helpers.spec.BpmnSpecConverter` for more information about what's going
+        on here.
+
+        :param spec_config: a dictionary specifying how to save and restore any classes used by the spec
+        :param registry: a `DictionaryConverter` with conversions for custom data (if applicable)
+        """
+        config = spec_config or DEFAULT_SPEC_CONFIG
+        spec_converter = registry or DictionaryConverter()
+        config['process'](spec_converter)
+        for cls in config['data_specs'] + config['task_specs'] + config['event_definitions']:
+            cls(spec_converter)
+        return spec_converter
+
+    def __init__(self, spec_converter=None, data_converter=None, wf_class=None, version=VERSION,
+                 json_encoder_cls=DEFAULT_JSON_ENCODER_CLS, json_decoder_cls=DEFAULT_JSON_DECODER_CLS):
+        """Intializes a Workflow Serializer with the given Workflow, Task and Data Converters.
+
+        :param spec_converter: the workflow spec converter
+        :param data_converter: the data converter
+        :param wf_class: the workflow class
+        :param json_encoder_cls: JSON encoder class to be used for dumps/dump operations
+        :param json_decoder_cls: JSON decoder class to be used for loads/load operations
         """
-        raise NotImplementedError
+        super().__init__()
+        self.spec_converter = spec_converter if spec_converter is not None else self.configure_workflow_spec_converter()
+        self.data_converter = data_converter if data_converter is not None else DefaultRegistry()
+        self.wf_class = wf_class if wf_class is not None else BpmnWorkflow
+        self.json_encoder_cls = json_encoder_cls
+        self.json_decoder_cls = json_decoder_cls
+        self.VERSION = version
 
-    def get_default_attributes(self, spec):
-        """Extracts the default Spiff attributes from a task spec.
+    def serialize_json(self, workflow, use_gzip=False):
+        """Serialize the dictionary representation of the workflow to JSON.
 
-        :param spec: the task spec to be converted
+        :param workflow: the workflow to serialize
 
         Returns:
-            a dictionary of standard task spec attributes
+            a JSON dump of the dictionary representation
         """
-        dct = {
-            'id': spec.id,
-            'name': spec.name,
-            'description': spec.description,
-            'manual': spec.manual,
-            'internal': spec.internal,
-            'lookahead': spec.lookahead,
-            'inputs': [task.name for task in spec.inputs],
-            'outputs': [task.name for task in spec.outputs],
-        }
-        # This stuff is also all defined in the base task spec, but can contain data, so we need
-        # our data serializer.  I think we should try to get this stuff out of the base task spec.
-        if self.data_converter is not None:
-            dct['data'] = self.data_converter.convert(spec.data)
-            dct['defines'] = self.data_converter.convert(spec.defines)
-            dct['pre_assign'] = self.data_converter.convert(spec.pre_assign)
-            dct['post_assign'] = self.data_converter.convert(spec.post_assign)
-
+        dct = self.workflow_to_dict(workflow)
+        dct[self.VERSION_KEY] = self.VERSION
+        json_str = json.dumps(dct, cls=self.json_encoder_cls)
+        return gzip.compress(json_str.encode('utf-8')) if use_gzip else json_str
+
+    def __get_dict(self, serialization, use_gzip=False):
+        if isinstance(serialization, dict):
+            dct = serialization
+        elif use_gzip:
+            dct = json.loads(gzip.decompress(serialization), cls=self.json_decoder_cls)
+        else:
+            dct = json.loads(serialization, cls=self.json_decoder_cls)
         return dct
 
-    def get_bpmn_attributes(self, spec):
-        """Extracts the attributes added by the `BpmnSpecMixin` class.
+    def deserialize_json(self, serialization, use_gzip=False):
+        dct = self.__get_dict(serialization, use_gzip)
+        return self.workflow_from_dict(dct)
+
+    def get_version(self, serialization, use_gzip=False):
+        try:
+            dct = self.__get_dict(serialization, use_gzip)
+            if self.VERSION_KEY in dct:
+                return dct[self.VERSION_KEY]
+        except:  # Don't bail out trying to get a version, just return none.
+            return None
 
-        :param spec: the task spec to be converted
+    def workflow_to_dict(self, workflow):
+        """Return a JSON-serializable dictionary representation of the workflow.
 
-        Returns:
-            a dictionary of BPMN task spec attributes
-        """
-        return {
-            'lane': spec.lane,
-            'documentation': spec.documentation,
-            'loopTask': spec.loopTask,
-            'position': spec.position,
-            'outgoing_sequence_flows': dict(
-                (k, self.convert(v)) for k, v in spec.outgoing_sequence_flows.items()
-            ),
-            'outgoing_sequence_flows_by_id': dict(
-                (k, self.convert(v)) for k, v in spec.outgoing_sequence_flows_by_id.items()
-            ),
-            'data_input_associations': [ self.convert(obj) for obj in spec.data_input_associations ],
-            'data_output_associations': [ self.convert(obj) for obj in spec.data_output_associations ],
-        }
-
-    def get_join_attributes(self, spec):
-        """Extracts attributes for task specs that inherit from `Join`.
-
-        :param spec: the task spec to be converted
+        :param workflow: the workflow
 
         Returns:
-            a dictionary of `Join` task spec attributes
+            a dictionary representation of the workflow
         """
-        return {
-            'split_task': spec.split_task,
-            'threshold': spec.threshold,
-            'cancel': spec.cancel_remaining,
-        }
-
-    def get_subworkflow_attributes(self, spec):
-        """Extracts attributes for task specs that inherit from `SubWorkflowTask`.
+        # These properties are applicable to top level & subprocesses
+        dct = self.process_to_dict(workflow)
+        # These are only used at the top-level
+        dct['spec'] = self.spec_converter.convert(workflow.spec)
+        dct['subprocess_specs'] = dict(
+            (name, self.spec_converter.convert(spec)) for name, spec in workflow.subprocess_specs.items()
+        )
+        dct['subprocesses'] = dict(
+            (str(task_id), self.process_to_dict(sp)) for task_id, sp in workflow.subprocesses.items()
+        )
+        dct['bpmn_messages'] = [self.message_to_dict(msg) for msg in workflow.bpmn_messages]
 
-        :param spec: the task spec to be converted
-
-        Returns:
-            a dictionary of subworkflow task spec attributes
-        """
-        return {'spec': spec.spec}
+        dct['correlations'] = workflow.correlations
+        return dct
 
-    def task_spec_from_dict(self, dct):
-        """
-        Creates a task spec based on the supplied dictionary.  It handles setting the default
-        task spec attributes as well as attributes added by `BpmnSpecMixin`.
+    def workflow_from_dict(self, dct):
+        """Create a workflow based on a dictionary representation.
 
-        :param dct: the dictionary to create the task spec from
+        :param dct: the dictionary representation
 
         Returns:
-            a restored task spec
+            a BPMN Workflow object
         """
-        internal = dct.pop('internal')
-        inputs = dct.pop('inputs')
-        outputs = dct.pop('outputs')
-
-        spec = self.spec_class(**dct)
-        spec.internal = internal
-        spec.inputs = inputs
-        spec.outputs = outputs
-        spec.id = dct['id']
-
-        if self.data_converter is not None:
-            spec.data = self.data_converter.restore(dct.get('data', {}))
-            spec.defines = self.data_converter.restore(dct.get('defines', {}))
-            spec.pre_assign = self.data_converter.restore(dct.get('pre_assign', {}))
-            spec.post_assign = self.data_converter.restore(dct.get('post_assign', {}))
-
-        if isinstance(spec, BpmnSpecMixin):
-            spec.documentation = dct.pop('documentation', None)
-            spec.lane = dct.pop('lane', None)
-            spec.loopTask = dct.pop('loopTask', False)
-            spec.outgoing_sequence_flows = self.restore(dct.pop('outgoing_sequence_flows', {}))
-            spec.outgoing_sequence_flows_by_id = self.restore(dct.pop('outgoing_sequence_flows_by_id', {}))
-            spec.data_input_associations = self.restore(dct.pop('data_input_associations', []))
-            spec.data_output_associations = self.restore(dct.pop('data_output_associations', []))
+        dct_copy = deepcopy(dct)
 
-        return spec
+        # Upgrade serialized version if necessary
+        if self.VERSION_KEY in dct_copy:
+            version = dct_copy.pop(self.VERSION_KEY)
+            if version in MIGRATIONS:
+                dct_copy = MIGRATIONS[version](dct_copy)
 
-    def event_definition_to_dict(self, event_definition):
-        """
-        Converts an BPMN event definition to a dict.  It will not typically be called directly,
-        but via `convert` and will convert any event type supported by Spiff.
+        # Restore the top level spec and the subprocess specs
+        spec = self.spec_converter.restore(dct_copy.pop('spec'))
+        subprocess_specs = dct_copy.pop('subprocess_specs', {})
+        for name, wf_dct in subprocess_specs.items():
+            subprocess_specs[name] = self.spec_converter.restore(wf_dct)
 
-        :param event_definition: the event_definition to be converted.
+        # Create the top-level workflow
+        workflow = self.wf_class(spec, subprocess_specs, deserializing=True)
 
-        Returns:
-            a dictionary representation of an event definition
-        """
-        dct = {'internal': event_definition.internal, 'external': event_definition.external}
-
-        if isinstance(event_definition, NamedEventDefinition):
-            dct['name'] = event_definition.name
-        if isinstance(event_definition, MessageEventDefinition):
-            dct['correlation_properties'] = [prop.__dict__ for prop in event_definition.correlation_properties]
-        if isinstance(event_definition, TimerEventDefinition):
-            dct['label'] = event_definition.label
-            dct['dateTime'] = event_definition.dateTime
-        if isinstance(event_definition, CycleTimerEventDefinition):
-            dct['label'] = event_definition.label
-            dct['cycle_definition'] = event_definition.cycle_definition
-        if isinstance(event_definition, ErrorEventDefinition):
-            dct['error_code'] = event_definition.error_code
-        if isinstance(event_definition, EscalationEventDefinition):
-            dct['escalation_code'] = event_definition.escalation_code
+        # Restore any unretrieve messages
+        workflow.bpmn_messages = [ self.message_from_dict(msg) for msg in dct.get('bpmn_messages', []) ]
 
-        return dct
+        workflow.correlations = dct_copy.pop('correlations', {})
 
-    def event_defintion_from_dict(self, definition_class, dct):
-        """Restores an event definition.  It will not typically be called directly, but via
-        `restore` and will restore any BPMN event type supporred by Spiff.
+        # Restore the remainder of the workflow
+        workflow.data = self.data_converter.restore(dct_copy.pop('data'))
+        workflow.success = dct_copy.pop('success')
+        workflow.task_tree = self.task_tree_from_dict(dct_copy, dct_copy.pop('root'), None, workflow)
 
-        :param definition_class: the class that will be used to create the object
-        :param dct: the event definition attributes
+        return workflow
 
-        Returns:
-            an `EventDefinition` object
-        """
-        internal, external = dct.pop('internal'), dct.pop('external')
-        if 'correlation_properties' in dct:
-            dct['correlation_properties'] = [CorrelationProperty(**prop) for prop in dct['correlation_properties']]
-        event_definition = definition_class(**dct)
-        event_definition.internal = internal
-        event_definition.external = external
-        return event_definition
-
-    def sequence_flow_to_dict(self, flow):
+    def task_to_dict(self, task):
         return {
-            'id': flow.id,
-            'name': flow.name,
-            'documentation': flow.documentation,
-            'target_task_spec': flow.target_task_spec.name
+            'id': str(task.id),
+            'parent': str(task.parent.id) if task.parent is not None else None,
+            'children': [ str(child.id) for child in task.children ],
+            'last_state_change': task.last_state_change,
+            'state': task.state,
+            'task_spec': task.task_spec.name,
+            'triggered': task.triggered,
+            'workflow_name': task.workflow.name,
+            'internal_data': self.data_converter.convert(task.internal_data),
+            'data': self.data_converter.convert(task.data),
         }
 
-    def sequence_flow_from_dict(self, dct):
-        return SequenceFlow(**dct)
-
-    def attrib_to_dict(self, attrib):
-        return { 'name': attrib.name }
-
-    def attrib_from_dict(self, attrib_class, dct):
-        return attrib_class(dct['name'])
+    def task_from_dict(self, dct, workflow, task_spec, parent):
 
+        task = Task(workflow, task_spec, parent, dct['state'])
+        task.id = UUID(dct['id'])
+        task.last_state_change = dct['last_state_change']
+        task.triggered = dct['triggered']
+        task.internal_data = self.data_converter.restore(dct['internal_data'])
+        task.data = self.data_converter.restore(dct['data'])
+        return task
+
+    def task_tree_to_dict(self, root):
+
+        tasks = { }
+        def add_task(task):
+            dct = self.task_to_dict(task)
+            tasks[dct['id']] = dct
+            for child in task.children:
+                add_task(child)
+
+        add_task(root)
+        return tasks
+
+    def task_tree_from_dict(self, process_dct, task_id, parent_task, process, top_level_workflow=None, top_level_dct=None):
+
+        top = top_level_workflow or process
+        top_dct = top_level_dct or process_dct
+
+        task_dict = process_dct['tasks'][task_id]
+        task_spec = process.spec.task_specs[task_dict['task_spec']]
+        task = self.task_from_dict(task_dict, process, task_spec, parent_task)
+        if task_id == process_dct['last_task']:
+            process.last_task = task
+
+        if isinstance(task_spec, SubWorkflowTask) and task_id in top_dct.get('subprocesses', {}):
+            subprocess_spec = top.subprocess_specs[task_spec.spec]
+            subprocess = self.wf_class(subprocess_spec, {}, name=task_spec.name, parent=process, deserializing=True)
+            subprocess_dct = top_dct['subprocesses'].get(task_id, {})
+            subprocess.spec.data_objects.update(process.spec.data_objects)
+            if len(subprocess.spec.data_objects) > 0:
+                subprocess.data = process.data
+            else:
+                subprocess.data = self.data_converter.restore(subprocess_dct.pop('data'))
+            subprocess.success = subprocess_dct.pop('success')
+            subprocess.task_tree = self.task_tree_from_dict(subprocess_dct, subprocess_dct.pop('root'), None, subprocess, top, top_dct)
+            subprocess.completed_event.connect(task_spec._on_subworkflow_completed, task)
+            top_level_workflow.subprocesses[task.id] = subprocess
+
+        for child_task_id in task_dict['children']:
+            if child_task_id in process_dct['tasks']:
+                child = process_dct['tasks'][child_task_id]
+                self.task_tree_from_dict(process_dct, child_task_id, task, process, top, top_dct)
+            else:
+                raise ValueError(f"Task {task_id} ({task_spec.name}) has child {child_task_id}, but no such task exists")
 
-class BpmnWorkflowSpecConverter(DictionaryConverter):
-    """
-    This is the base converter for a BPMN workflow spec.
-
-    It will register converters for the task spec types contained in the workflow, as well as
-    the workflow spec class itself.
-
-    This class can be extended if you implement a custom workflow spec type.  See the converter
-    in `workflow_spec_converter` for an example.
-    """
+        return task
 
-    def __init__(self, spec_class, task_spec_converters, data_converter=None):
-        """
-        Converter for a BPMN workflow spec class.
-
-        The `to_dict` and `from_dict` methods of the given task spec converter classes will
-        be registered, so that they can be restored automatically.
-
-        The data_converter applied to task *spec* data, not task data, and may be `None`.  See
-        `BpmnTaskSpecConverter` for more discussion.
-
-        :param spec_class: the workflow spec class
-        :param task_spec_converters: a list of `BpmnTaskSpecConverter` classes
-        :param data_converter: an optional data converter
-        """
-        super().__init__()
-        self.spec_class = spec_class
-        self.data_converter = data_converter
-
-        self.register(spec_class, self.to_dict, self.from_dict)
-        for converter in task_spec_converters:
-            self.register(converter.spec_class, converter.to_dict, converter.from_dict, converter.typename)
-        self.register(BpmnDataSpecification, BpmnDataSpecificationConverter.to_dict, BpmnDataSpecificationConverter.from_dict)
+    def process_to_dict(self, process):
+        return {
+            'data': self.data_converter.convert(process.data),
+            'last_task': str(process.last_task.id) if process.last_task is not None else None,
+            'success': process.success,
+            'tasks': self.task_tree_to_dict(process.task_tree),
+            'root': str(process.task_tree.id),
+        }
 
-    def to_dict(self, spec):
-        """
-        The convert method that will be called when a Workflow Spec Converter is registered with a
-        Workflow Converter.
-        """
-        raise NotImplementedError
+    def message_to_dict(self, message):
+        dct = {
+            'correlations': dict([ (k, self.data_converter.convert(v)) for k, v in message.correlations.items() ]),
+            'name': message.name,
+            'payload': self.spec_converter.convert(message.payload),
+        }
+        return dct
 
-    def from_dict(self, dct):
-        """
-        The restore method that will be called when a Workflow Spec Converter is registered with a
-        Workflow Converter.
-        """
-        raise NotImplementedError
+    def message_from_dict(self, dct):
+        return BpmnMessage(
+            dict([ (k, self.data_converter.restore(v)) for k, v in dct['correlations'].items() ]),
+            dct['name'],
+            self.spec_converter.restore(dct['payload'])
+        )
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/serializer/task_spec_converters.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/task_spec.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,310 +1,326 @@
-from uuid import UUID
-
-from .bpmn_converters import BpmnTaskSpecConverter
-
-from ...specs import StartTask
-from ...specs.Simple import Simple
-from ...specs.LoopResetTask import LoopResetTask
-
-from ..specs.BpmnProcessSpec import _EndJoin
-from ..specs.BpmnSpecMixin import _BpmnCondition
-
-from ..specs.NoneTask import NoneTask
-from ..specs.UserTask import UserTask
-from ..specs.ManualTask import ManualTask
-from ..specs.ScriptTask import ScriptTask
-from ..specs.SubWorkflowTask import CallActivity, TransactionSubprocess
-
-from ..specs.ExclusiveGateway import ExclusiveGateway
-from ..specs.InclusiveGateway import InclusiveGateway
-from ..specs.ParallelGateway import ParallelGateway
-
-from ..specs.events import StartEvent, EndEvent, BoundaryEvent, IntermediateCatchEvent, IntermediateThrowEvent
-from ..specs.events.IntermediateEvent import _BoundaryEventParent, SendTask, ReceiveTask
-
-from ..workflow import BpmnWorkflow
-
-
-class SimpleTaskConverter(BpmnTaskSpecConverter):
-
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(Simple, data_converter, typename)
+# Copyright (C) 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3.0 of the License, or (at your option) any later version.
+#
+# SpiffWorkflow is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
+
+from SpiffWorkflow.bpmn.specs.control import BpmnStartTask, _EndJoin, _BoundaryEventParent, SimpleBpmnTask
+from SpiffWorkflow.bpmn.specs.bpmn_task_spec import _BpmnCondition
+from SpiffWorkflow.bpmn.specs.defaults import (
+    UserTask,
+    ManualTask,
+    NoneTask,
+    ScriptTask,
+    ExclusiveGateway,
+    InclusiveGateway,
+    ParallelGateway,
+    StandardLoopTask,
+    SequentialMultiInstanceTask,
+    ParallelMultiInstanceTask,
+    CallActivity,
+    TransactionSubprocess,
+    SubWorkflowTask,
+    StartEvent,
+    EndEvent,
+    IntermediateCatchEvent,
+    IntermediateThrowEvent,
+    BoundaryEvent,
+    EventBasedGateway,
+    SendTask,
+    ReceiveTask,
+)
+
+from .helpers.spec import TaskSpecConverter
+
+
+class BpmnTaskSpecConverter(TaskSpecConverter):
 
     def to_dict(self, spec):
         dct = self.get_default_attributes(spec)
         return dct
 
     def from_dict(self, dct):
         return self.task_spec_from_dict(dct)
 
 
-class StartTaskConverter(BpmnTaskSpecConverter):
-
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(StartTask, data_converter, typename)
-
-    def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        return dct
-
-    def from_dict(self, dct):
-        return self.task_spec_from_dict(dct)
+class SimpleBpmnTaskConverter(BpmnTaskSpecConverter):
+    def __init__(self, registry):
+        super().__init__(SimpleBpmnTask, registry)
+
+class BpmnStartTaskConverter(BpmnTaskSpecConverter):
+    def __init__(self, registry):
+        super().__init__(BpmnStartTask, registry)
 
-class LoopResetTaskConverter(BpmnTaskSpecConverter):
+class EndJoinConverter(BpmnTaskSpecConverter):
+    def __init__(self, registry):
+        super().__init__(_EndJoin, registry)
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(LoopResetTask, data_converter, typename)
 
-    def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        # Maybe I should add this to the base task converter, but I'm trying to keep it free of
-        # anything but task related conversions
-        dct['destination_id'] = str(spec.destination_id)
-        dct['destination_spec_name'] = spec.destination_spec_name
-        return dct
 
-    def from_dict(self, dct):
-        spec = self.task_spec_from_dict(dct)
-        spec.destination_id = UUID(spec.destination_id)
-        return spec
+class NoneTaskConverter(BpmnTaskSpecConverter):
+    def __init__(self, registry):
+        super().__init__(NoneTask, registry)
 
-class EndJoinConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(_EndJoin, data_converter, typename)
+class UserTaskConverter(BpmnTaskSpecConverter):
+    def __init__(self, registry):
+        super().__init__(UserTask, registry)
 
-    def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        return dct
 
-    def from_dict(self, dct):
-        return self.task_spec_from_dict(dct)
+class ManualTaskConverter(BpmnTaskSpecConverter):
+    def __init__(self, registry):
+        super().__init__(ManualTask, registry)
 
 
-class NoneTaskConverter(BpmnTaskSpecConverter):
+class ScriptTaskConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(NoneTask, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(ScriptTask, registry)
 
     def to_dict(self, spec):
         dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
+        dct['script'] = spec.script
         return dct
 
-    def from_dict(self, dct):
-        return self.task_spec_from_dict(dct)
-
 
-class UserTaskConverter(BpmnTaskSpecConverter):
+class StandardLoopTaskConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(UserTask, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(StandardLoopTask, registry)
 
     def to_dict(self, spec):
         dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
+        dct.update(self.get_standard_loop_attributes(spec))
         return dct
 
-    def from_dict(self, dct):
-        return self.task_spec_from_dict(dct)
-
-
-class ManualTaskConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(ManualTask, data_converter, typename)
+class MultiInstanceTaskConverter(BpmnTaskSpecConverter):
 
     def to_dict(self, spec):
         dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
+        dct['task_spec'] = spec.task_spec
+        dct['cardinality'] = spec.cardinality
+        dct['data_input'] = self.registry.convert(spec.data_input)
+        dct['data_output'] = self.registry.convert(spec.data_output)
+        dct['input_item'] = self.registry.convert(spec.input_item)
+        dct['output_item'] = self.registry.convert(spec.output_item)
+        dct['condition'] = spec.condition
         return dct
 
     def from_dict(self, dct):
+        dct['data_input'] = self.registry.restore(dct['data_input'])
+        dct['data_output'] = self.registry.restore(dct['data_output'])
+        dct['input_item'] = self.registry.restore(dct['input_item'])
+        dct['output_item'] = self.registry.restore(dct['output_item'])
         return self.task_spec_from_dict(dct)
 
 
-class ScriptTaskConverter(BpmnTaskSpecConverter):
+class ParallelMultiInstanceTaskConverter(MultiInstanceTaskConverter):
+    def __init__(self, registry):
+        super().__init__(ParallelMultiInstanceTask, registry)
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(ScriptTask, data_converter, typename)
+class SequentialMultiInstanceTaskConverter(MultiInstanceTaskConverter):
+    def __init__(self, registry):
+        super().__init__(SequentialMultiInstanceTask, registry)
 
-    def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
-        dct['script'] = spec.script
-        return dct
 
-    def from_dict(self, dct):
-        return self.task_spec_from_dict(dct)
-
-
-class CallActivityTaskConverter(BpmnTaskSpecConverter):
+class BoundaryEventParentConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(CallActivity, data_converter, typename)
-        self.wf_class = BpmnWorkflow
+    def __init__(self, registry):
+        super().__init__(_BoundaryEventParent, registry)
 
     def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
-        dct.update(self.get_subworkflow_attributes(spec))
+        dct = super().to_dict(spec)
+        dct['main_child_task_spec'] = spec.main_child_task_spec.name
         return dct
 
-    def from_dict(self, dct):
-        dct['subworkflow_spec'] = dct.pop('spec')
-        return self.task_spec_from_dict(dct)
-
 
-class TransactionSubprocessTaskConverter(BpmnTaskSpecConverter):
+class SubWorkflowConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(TransactionSubprocess, data_converter, typename)
-        self.wf_class = BpmnWorkflow
+    def __init__(self, cls, registry):
+        super().__init__(cls, registry)
 
     def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
+        dct = super().to_dict(spec)
         dct.update(self.get_subworkflow_attributes(spec))
         return dct
 
     def from_dict(self, dct):
         dct['subworkflow_spec'] = dct.pop('spec')
         return self.task_spec_from_dict(dct)
 
+class SubprocessTaskConverter(SubWorkflowConverter):
+    def __init__(self, registry):
+        super().__init__(SubWorkflowTask, registry)
+
+class CallActivityTaskConverter(SubWorkflowConverter):
+    def __init__(self, registry):
+        super().__init__(CallActivity, registry)
 
-class ExclusiveGatewayConverter(BpmnTaskSpecConverter):
+class TransactionSubprocessTaskConverter(SubWorkflowConverter):
+    def __init__(self, registry):
+        super().__init__(TransactionSubprocess, registry)
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(ExclusiveGateway, data_converter, typename)
+
+class ConditionalGatewayConverter(BpmnTaskSpecConverter):
 
     def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
-        dct['default_task_spec'] = spec.default_task_spec
+        dct = super().to_dict(spec)
         dct['cond_task_specs'] = [ self.bpmn_condition_to_dict(cond) for cond in spec.cond_task_specs ]
         dct['choice'] = spec.choice
         return dct
 
     def from_dict(self, dct):
         conditions = dct.pop('cond_task_specs')
-        default_task_spec = dct.pop('default_task_spec')
         spec = self.task_spec_from_dict(dct)
         spec.cond_task_specs = [ self.bpmn_condition_from_dict(cond) for cond in conditions ]
-        spec.default_task_spec = default_task_spec
         return spec
 
     def bpmn_condition_from_dict(self, dct):
-        return (_BpmnCondition(dct['condition']), dct['task_spec'])
+        return (_BpmnCondition(dct['condition']) if dct['condition'] is not None else None, dct['task_spec'])
 
     def bpmn_condition_to_dict(self, condition):
-
         expr, task_spec = condition
         return {
-            'condition': expr.args[0],
+            'condition': expr.args[0] if expr is not None else None,
             'task_spec': task_spec
         }
 
-class InclusiveGatewayConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(InclusiveGateway, data_converter, typename)
+class ExclusiveGatewayConverter(ConditionalGatewayConverter):
+
+    def __init__(self, registry):
+        super().__init__(ExclusiveGateway, registry)
 
     def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
-        dct.update(self.get_join_attributes(spec))
+        dct = super().to_dict(spec)
+        dct['default_task_spec'] = spec.default_task_spec
         return dct
 
     def from_dict(self, dct):
-        return self.task_spec_from_dict(dct)
+        default_task_spec = dct.pop('default_task_spec')
+        spec = super().from_dict(dct)
+        spec.default_task_spec = default_task_spec
+        return spec
+
+
+class InclusiveGatewayConverter(ConditionalGatewayConverter):
+    def __init__(self, registry):
+        super().__init__(InclusiveGateway, registry)
 
 
 class ParallelGatewayConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(ParallelGateway, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(ParallelGateway, registry)
 
     def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
+        dct = super().to_dict(spec)
         dct.update(self.get_join_attributes(spec))
         return dct
 
     def from_dict(self, dct):
         return self.task_spec_from_dict(dct)
 
 
 class EventConverter(BpmnTaskSpecConverter):
 
-    def __init__(self, spec_class, data_converter, typename):
-        super().__init__(spec_class, data_converter, typename)
+    def __init__(self, spec_class, registry):
+        super().__init__(spec_class, registry)
 
     def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
-        dct['event_definition'] = self.convert(spec.event_definition)
+        dct = super().to_dict(spec)
+        dct['event_definition'] = self.registry.convert(spec.event_definition)
         return dct
 
     def from_dict(self, dct):
-        dct['event_definition'] = self.restore(dct['event_definition'])
+        dct['event_definition'] = self.registry.restore(dct['event_definition'])
         return self.task_spec_from_dict(dct)
 
 
 class StartEventConverter(EventConverter):
-
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(StartEvent, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(StartEvent, registry)
 
 
 class EndEventConverter(EventConverter):
-
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(EndEvent, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(EndEvent, registry)
 
 
 class IntermediateCatchEventConverter(EventConverter):
-
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(IntermediateCatchEvent, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(IntermediateCatchEvent, registry)
 
 
 class ReceiveTaskConverter(EventConverter):
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(ReceiveTask, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(ReceiveTask, registry)
 
 
 class IntermediateThrowEventConverter(EventConverter):
-
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(IntermediateThrowEvent, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(IntermediateThrowEvent, registry)
 
 
 class SendTaskConverter(EventConverter):
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(SendTask, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(SendTask, registry)
 
 
 class BoundaryEventConverter(EventConverter):
 
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(BoundaryEvent, data_converter, typename)
+    def __init__(self, registry):
+        super().__init__(BoundaryEvent, registry)
 
     def to_dict(self, spec):
         dct = super().to_dict(spec)
         dct['cancel_activity'] = spec.cancel_activity
         return dct
 
 
-class BoundaryEventParentConverter(BpmnTaskSpecConverter):
-
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(_BoundaryEventParent, data_converter, typename)
-
-    def to_dict(self, spec):
-        dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
-        dct['main_child_task_spec'] = spec.main_child_task_spec.name
-        return dct
-
-    def from_dict(self, dct):
-        return self.task_spec_from_dict(dct)
+class EventBasedGatewayConverter(EventConverter):
+    def __init__(self, registry):
+        super().__init__(EventBasedGateway, registry)
+
+
+DEFAULT_TASK_SPEC_CONVERTER_CLASSES = [
+    SimpleBpmnTaskConverter,
+    BpmnStartTaskConverter,
+    EndJoinConverter,
+    NoneTaskConverter,
+    UserTaskConverter,
+    ManualTaskConverter,
+    ScriptTaskConverter,
+    StandardLoopTaskConverter,
+    ParallelMultiInstanceTaskConverter,
+    SequentialMultiInstanceTaskConverter,
+    SubprocessTaskConverter,
+    CallActivityTaskConverter,
+    TransactionSubprocessTaskConverter,
+    StartEventConverter,
+    EndEventConverter, 
+    SendTaskConverter,
+    ReceiveTaskConverter,
+    IntermediateCatchEventConverter,
+    IntermediateThrowEventConverter,
+    EventBasedGatewayConverter,
+    BoundaryEventConverter,
+    BoundaryEventParentConverter,
+    ParallelGatewayConverter,
+    ExclusiveGatewayConverter,
+    InclusiveGatewayConverter,
+]
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/BpmnProcessSpec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/WorkflowSpec.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,185 +1,170 @@
-# -*- coding: utf-8 -*-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
-from copy import deepcopy
-import logging
-
-from SpiffWorkflow.bpmn.exceptions import WorkflowDataException
-from ...task import TaskState
-from .UnstructuredJoin import UnstructuredJoin
-from ...specs.Simple import Simple
-from ...specs.WorkflowSpec import WorkflowSpec
-
-
-data_log = logging.getLogger('spiff.data')
-
-class _EndJoin(UnstructuredJoin):
-
-    def _check_threshold_unstructured(self, my_task, force=False):
-        # Look at the tree to find all ready and waiting tasks (excluding
-        # ourself). The EndJoin waits for everyone!
-        waiting_tasks = []
-        for task in my_task.workflow.get_tasks(TaskState.READY | TaskState.WAITING):
-            if task.thread_id != my_task.thread_id:
-                continue
-            if task.task_spec == my_task.task_spec:
-                continue
-
-            is_mine = False
-            w = task.workflow
-            if w == my_task.workflow:
-                is_mine = True
-            while w and w.outer_workflow != w:
-                w = w.outer_workflow
-                if w == my_task.workflow:
-                    is_mine = True
-            if is_mine:
-                waiting_tasks.append(task)
-
-        return force or len(waiting_tasks) == 0, waiting_tasks
-
-    def _on_complete_hook(self, my_task):
-        super(_EndJoin, self)._on_complete_hook(my_task)
-        my_task.workflow.data.update(my_task.data)
-
-    def serialize(self, serializer):
-        return serializer.serialize_join(self)
-
-    @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_join(wf_spec, s_state, _EndJoin)
-
-
-class BpmnDataSpecification:
+from ..specs.StartTask import StartTask
 
-    def __init__(self, name, description=None):
-        """
-        :param name: the name of the task (the BPMN ID)
-        :param description: the task description (the BPMN name)
-        """
-        self.name = name
-        self.description = description or name
-        # In the future, we can add schemas defining the objects here.
-
-    def get(self, my_task):
-        """Copy a value form the workflow data to the task data."""
-        if self.name not in my_task.workflow.data:
-            message = f"Workflow variable {self.name} not found"
-            raise WorkflowDataException(my_task, data_input=self, message=message)
-        my_task.data[self.name] = deepcopy(my_task.workflow.data[self.name])
-
-    def set(self, my_task):
-        """Copy a value from the task data to the workflow data"""
-        if self.name not in my_task.data:
-            message = f"Task variable {self.name} not found"
-            raise WorkflowDataException(my_task, data_output=self, message=message)
-        my_task.workflow.data[self.name] = deepcopy(my_task.data[self.name])
-        del my_task.data[self.name]
-        data_log.info(f'Set workflow variable {self.name}', extra=my_task.log_info())
-
-    def copy(self, source, destination, data_input=False, data_output=False):
-        """Copy a value from one task to another."""
-        if self.name not in source.data:
-            message = f"Unable to copy {self.name}"
-            raise WorkflowDataException(
-                source, 
-                data_input=self if data_input else None,
-                data_output=self if data_output else None,
-                message=message
-            )
-        destination.data[self.name] = deepcopy(source.data[self.name])
 
+class WorkflowSpec(object):
 
-class BpmnProcessSpec(WorkflowSpec):
     """
-    This class represents the specification of a BPMN process workflow. This
-    specialises the standard Spiff WorkflowSpec class with a few extra methods
-    and attributes.
+    This class represents the specification of a workflow.
     """
 
-    def __init__(self, name=None, description=None, filename=None, svg=None):
+    def __init__(self, name=None, filename=None, nostart=False):
         """
         Constructor.
-
-        :param svg: This provides the SVG representation of the workflow as an
-        LXML node. (optional)
-        """
-        super(BpmnProcessSpec, self).__init__(name=name, filename=filename)
-        self.end = _EndJoin(self, '%s.EndJoin' % (self.name))
-        end = Simple(self, 'End')
-        end.follow(self.end)
-        self.svg = svg
-        self.description = description
-        self.data_inputs = []
-        self.data_outputs = []
-        self.data_objects = {}
-        self.correlation_keys = {}
-
-    def get_all_lanes(self):
         """
-        Returns a set of the distinct lane names used in the process (including
-        called activities)
+        self.name = name or ''
+        self.description = ''
+        self.file = filename
+        self.task_specs = dict()
+        self.start = None
+        if not nostart:
+            self.start = StartTask(self)
+
+    def _add_notify(self, task_spec):
+        """
+        Called by a task spec when it was added into the workflow.
+        """
+        if task_spec.name in self.task_specs:
+            raise KeyError('Duplicate task spec name: ' + task_spec.name)
+        self.task_specs[task_spec.name] = task_spec
+
+    def get_task_spec_from_name(self, name):
+        """
+        Returns the task with the given name.
+
+        :type  name: str
+        :param name: The name of the task spec.
+        :rtype:  TaskSpec
+        :returns: The task spec with the given name.
+        """
+        return self.task_specs.get(name)
+
+    def validate(self):
+        """Checks integrity of workflow and reports any problems with it.
+
+        Detects:
+        - loops (tasks that wait on each other in a loop)
+        :returns: empty list if valid, a list of errors if not
+        """
+        results = []
+        from ..specs.Join import Join
+
+        def recursive_find_loop(task, history):
+            current = history[:]
+            current.append(task)
+            if isinstance(task, Join):
+                if task in history:
+                    msg = "Found loop with '%s': %s then '%s' again" % (
+                        task.name, '->'.join([p.name for p in history]),
+                        task.name)
+                    raise Exception(msg)
+                for predecessor in task.inputs:
+                    recursive_find_loop(predecessor, current)
+
+            for parent in task.inputs:
+                recursive_find_loop(parent, current)
+
+        for task_id, task in list(self.task_specs.items()):
+            # Check for cyclic waits
+            try:
+                recursive_find_loop(task, [])
+            except Exception as exc:
+                results.append(exc.__str__())
+
+            # Check for disconnected tasks
+            if not task.inputs and task.name not in ['Start', 'Root']:
+                if task.outputs:
+                    results.append(f"Task '{task.name}' is disconnected (no inputs)")
+                else:
+                    results.append(f"Task '{task.name}' is not being used")
+
+
+        return results
+
+    def serialize(self, serializer, **kwargs):
+        """
+        Serializes the instance using the provided serializer.
+
+        :type  serializer: :class:`SpiffWorkflow.serializer.base.Serializer`
+        :param serializer: The serializer to use.
+        :type  kwargs: dict
+        :param kwargs: Passed to the serializer.
+        :rtype:  object
+        :returns: The serialized object.
         """
+        return serializer.serialize_workflow_spec(self, **kwargs)
 
-        done = set()
-        lanes = set()
-
-        def recursive_find(task_spec):
-            if task_spec in done:
-                return
-
-            done.add(task_spec)
-
-            if hasattr(task_spec, 'lane') and task_spec.lane:
-                lanes.add(task_spec.lane)
-
-            if hasattr(task_spec, 'spec'):
-                recursive_find(task_spec.spec.start)
-
-            for t in task_spec.outputs:
-                recursive_find(t)
-
-        recursive_find(self.start)
-
-        return lanes
-
-    def get_specs_depth_first(self):
+    @classmethod
+    def deserialize(cls, serializer, s_state, **kwargs):
         """
-        Get the specs for all processes (including called ones), in depth first
-        order.
+        Deserializes a WorkflowSpec instance using the provided serializer.
+
+        :type  serializer: :class:`SpiffWorkflow.serializer.base.Serializer`
+        :param serializer: The serializer to use.
+        :type  s_state: object
+        :param s_state: The serialized workflow specification object.
+        :type  kwargs: dict
+        :param kwargs: Passed to the serializer.
+        :rtype:  WorkflowSpec
+        :returns: The resulting instance.
         """
 
+        return serializer.deserialize_workflow_spec(s_state, **kwargs)
+
+    def get_dump(self, verbose=False):
         done = set()
-        specs = [self]
 
-        def recursive_find(task_spec):
+        def recursive_dump(task_spec, indent):
             if task_spec in done:
-                return
-
+                return '[shown earlier] %s (%s:%s)' % (
+                    task_spec.name,
+                    task_spec.__class__.__name__,
+                    hex(id(task_spec))
+                ) + '\n'
             done.add(task_spec)
+            dump = '%s (%s:%s)' % (
+                task_spec.name,
+                task_spec.__class__.__name__,
+                hex(id(task_spec))
+            ) + '\n'
+            if verbose:
+                if task_spec.inputs:
+                    dump += indent + \
+                        '- IN: ' + \
+                        ','.join(['%s (%s)' % (t.name, hex(id(t))) for t in task_spec.inputs]) + \
+                        '\n'
+                if task_spec.outputs:
+                    dump += indent + \
+                        '- OUT: ' + \
+                        ','.join(['%s (%s)' % (t.name, hex(id(t))) for t in task_spec.outputs]) + \
+                        '\n'
+            # sub_specs = ([task_spec.spec.start] if hasattr(task_spec, 'spec') else []) + task_spec.outputs
+            for i, t in enumerate(task_spec.outputs):
+                dump += indent + \
+                    '   --> ' + \
+                    recursive_dump(t, indent + ('   |   ' if i + 1 < len(task_spec.outputs) else '       '))
+            return dump
 
-            if hasattr(task_spec, 'spec'):
-                specs.append(task_spec.spec)
-                recursive_find(task_spec.spec.start)
-
-            for t in task_spec.outputs:
-                recursive_find(t)
-
-        recursive_find(self.start)
+        dump = recursive_dump(self.start, '')
+        return dump
 
-        return specs
+    def dump(self):
+        print(self.get_dump())
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ExclusiveGateway.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/StartTask.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2007 Samuel Abels
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from ...exceptions import WorkflowException
-
-from .BpmnSpecMixin import BpmnSpecMixin
-from ...specs import TaskSpec
-from ...specs.ExclusiveChoice import ExclusiveChoice
+from ..exceptions import WorkflowException
+from .base import TaskSpec
 
 
-class ExclusiveGateway(ExclusiveChoice, BpmnSpecMixin):
+class StartTask(TaskSpec):
 
     """
-    Task Spec for a bpmn:exclusiveGateway node.
+    This class implements the task the is placed at the beginning
+    of each workflow. The task has no inputs and at least one output.
+    If more than one output is connected, the task does an implicit
+    parallel split.
     """
 
+    def __init__(self, wf_spec, name='Start', **kwargs):
+        """
+        Constructor. The name of this task is *always* 'Start'.
+
+        :type  wf_spec: WorkflowSpec
+        :param wf_spec: A reference to the workflow specification.
+        :type  kwargs: dict
+        :param kwargs: See :class:`SpiffWorkflow.specs.TaskSpec`.
+        """
+        TaskSpec.__init__(self, wf_spec, name, **kwargs)
+
+    def _connect_notify(self, task_spec):
+        """
+        Called by the previous task to let us know that it exists.
+        """
+        raise WorkflowException('StartTask can not have any inputs.', task_spec=self)
+
     def test(self):
         """
         Checks whether all required attributes are set. Throws an exception
         if an error was detected.
         """
-        # This has been overridden to allow a single default flow out (without a
-        # condition) - useful for the converging type
-        TaskSpec.test(self)
-#        if len(self.cond_task_specs) < 1:
-#            raise WorkflowException(self, 'At least one output required.')
-        for condition, name in self.cond_task_specs:
-            if name is None:
-                raise WorkflowException(self, 'Condition with no task spec.')
-            task_spec = self._wf_spec.get_task_spec_from_name(name)
-            if task_spec is None:
-                msg = 'Condition leads to non-existent task ' + repr(name)
-                raise WorkflowException(self, msg)
-            if condition is None:
-                continue
-
-    @property
-    def spec_type(self):
-        return 'Exclusive Gateway'
+        if len(self.inputs) != 0:
+            raise WorkflowException('StartTask with an input.', task_spec=self)
+        elif len(self.outputs) < 1:
+            raise WorkflowException('No output task connected.', task_spec=self)
 
     def serialize(self, serializer):
-        return serializer.serialize_exclusive_gateway(self)
-
+        return serializer.serialize_start_task(self)
 
     @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_exclusive_gateway(wf_spec, s_state)
+    def deserialize(cls, serializer, wf_spec, s_state):
+        return serializer.deserialize_start_task(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/InclusiveGateway.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/inclusive_gateway.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from collections import deque
 
-from ...task import TaskState
-from .UnstructuredJoin import UnstructuredJoin
+from SpiffWorkflow.bpmn.exceptions import WorkflowTaskException
+from SpiffWorkflow.task import TaskState
+from SpiffWorkflow.specs.MultiChoice import MultiChoice
+from .unstructured_join import UnstructuredJoin
 
 
-class InclusiveGateway(UnstructuredJoin):
+
+class InclusiveGateway(MultiChoice, UnstructuredJoin):
     """
     Task Spec for a bpmn:parallelGateway node. From the specification of BPMN
     (http://www.omg.org/spec/BPMN/2.0/PDF - document number:formal/2011-01-03):
 
     The Inclusive Gateway is activated if
      * At least one incoming Sequence Flow has at least one token and
      * For every directed path formed by sequence flow that
@@ -58,66 +60,60 @@
     If and only if none of the conditions evaluates to true, the token is
     passed on the default Sequence Flow.
 
     In case all conditions evaluate to false and a default flow has not been
     specified, the Inclusive Gateway throws an exception.
     """
 
-    @property
-    def spec_type(self):
-        return 'Inclusive Gateway'
+    def test(self):
+        MultiChoice.test(self)
+        UnstructuredJoin.test(self)
 
     def _check_threshold_unstructured(self, my_task, force=False):
 
-        # Look at the tree to find all ready and waiting tasks (excluding ones
-        # that are our completed inputs).
-        tasks = []
-        for task in my_task.workflow.get_tasks(TaskState.READY | TaskState.WAITING):
-            if task.thread_id != my_task.thread_id:
-                continue
-            if task.workflow != my_task.workflow:
-                continue
-            if task.task_spec == my_task.task_spec:
-                continue
-            tasks.append(task)
-
-        inputs_with_tokens, waiting_tasks = self._get_inputs_with_tokens(
-            my_task)
-        inputs_without_tokens = [
-            i for i in self.inputs if i not in inputs_with_tokens]
-
-        waiting_tasks = []
-        for task in tasks:
-            if (self._has_directed_path_to(
-                    task, self,
-                    without_using_sequence_flow_from=inputs_with_tokens) and
-                not self._has_directed_path_to(
-                    task, self,
-                    without_using_sequence_flow_from=inputs_without_tokens)):
-                waiting_tasks.append(task)
-
-        return force or len(waiting_tasks) == 0, waiting_tasks
-
-    def _has_directed_path_to(self, task, task_spec,
-                              without_using_sequence_flow_from=None):
-        q = deque()
-        done = set()
-
-        without_using_sequence_flow_from = set(
-            without_using_sequence_flow_from or [])
-
-        q.append(task.task_spec)
-        while q:
-            n = q.popleft()
-            if n == task_spec:
-                return True
-            for child in n.outputs:
-                if child not in done and not (
-                        n in without_using_sequence_flow_from and
-                        child == task_spec):
-                    done.add(child)
-                    q.append(child)
-        return False
-
-    @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_generic(wf_spec, s_state, InclusiveGateway)
+        completed_inputs, waiting_tasks = self._get_inputs_with_tokens(my_task)
+        uncompleted_inputs = [i for i in self.inputs if i not in completed_inputs]
+
+        # We only have to complete a task once for it to count, even if's on multiple paths
+        for task in waiting_tasks:
+            if task.task_spec in completed_inputs:
+                waiting_tasks.remove(task)
+
+        if force:
+            # If force is true, complete the task
+            complete = True
+        elif len(waiting_tasks) > 0:
+            # If we have waiting tasks, we're obviously not done
+            complete = False
+        else:
+            # Handle the case where there are paths from active tasks that must go through uncompleted inputs
+            tasks = my_task.workflow.get_tasks(TaskState.READY | TaskState.WAITING, workflow=my_task.workflow)
+            sources = [t.task_spec for t in tasks]
+
+            # This will go back through a task spec's ancestors and return the source, if applicable
+            def check(spec): 
+                for parent in spec.inputs:
+                    return parent if parent in sources else check(parent)
+
+            # If we can get to a completed input from this task, we don't have to wait for it
+            for spec in completed_inputs:
+                source = check(spec)
+                if source is not None:
+                    sources.remove(source)
+
+            # Now check the rest of the uncompleted inputs and see if they can be reached from any of the remaining tasks
+            unfinished_paths = []
+            for spec in uncompleted_inputs:
+                if check(spec) is not None:
+                    unfinished_paths.append(spec)
+                    break
+
+            complete = len(unfinished_paths) == 0
+
+        return complete, waiting_tasks
+
+    def _run_hook(self, my_task):
+        outputs = self._get_matching_outputs(my_task)
+        if len(outputs) == 0:
+            raise WorkflowTaskException(f'No conditions satisfied on gateway', task=my_task)
+        my_task._sync_children(outputs, TaskState.FUTURE)
+        return True
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ManualTask.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/service_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from ...bpmn.specs.BpmnSpecMixin import BpmnSpecMixin
-
-from ...specs import Simple
 
+from .script_task import ScriptEngineTask
 
-class ManualTask(Simple, BpmnSpecMixin):
 
-    @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_generic(wf_spec, s_state, ManualTask)
+class ServiceTask(ScriptEngineTask):
 
-    def is_engine_task(self):
-        return False
+    """
+    Task Spec for a bpmn:serviceTask node.
+    """
 
-    @property
-    def spec_type(self):
-        return 'Manual Task'
+    def __init__(self, wf_spec, bpmn_id, **kwargs):
+        super(ServiceTask, self).__init__(wf_spec, bpmn_id, **kwargs)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/NoneTask.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Simple.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2007 Samuel Abels
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from ...specs import Simple
-
-from ...bpmn.specs.BpmnSpecMixin import BpmnSpecMixin
 
+from .base import TaskSpec
 
-class NoneTask(Simple, BpmnSpecMixin):
 
-    def is_engine_task(self):
-        return False
+class Simple(TaskSpec):
 
-    @property
-    def spec_type(self):
-        return 'Task'
+    """
+    This class implements a task with one or more inputs and
+    any number of outputs.
+    If more than one input is connected, the task performs an implicit
+    multi merge.
+    If more than one output is connected, the task performs an implicit
+    parallel split.
+    """
+    def serialize(self, serializer):
+        return serializer.serialize_simple(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_generic(wf_spec, s_state, NoneTask)
+        return serializer.deserialize_simple(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ParallelGateway.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/parallel_gateway.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from .UnstructuredJoin import UnstructuredJoin
+
+from .unstructured_join import UnstructuredJoin
 
 
 class ParallelGateway(UnstructuredJoin):
     """
     Task Spec for a bpmn:parallelGateway node. From the specification of BPMN
     (http://www.omg.org/spec/BPMN/2.0/PDF - document number:formal/2011-01-03):
 
@@ -38,19 +39,8 @@
 
     Essentially, this means that we must wait until we have a completed parent
     task on each incoming sequence.
     """
 
     def _check_threshold_unstructured(self, my_task, force=False):
         completed_inputs, waiting_tasks = self._get_inputs_with_tokens(my_task)
-
-        # If the threshold was reached, get ready to fire.
-        return (force or len(completed_inputs) >= len(self.inputs),
-                waiting_tasks)
-
-    @property
-    def spec_type(self):
-        return 'Parallel Gateway'
-
-    @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_generic(wf_spec, s_state, ParallelGateway)
+        return force or len(completed_inputs) >= len(self.inputs), waiting_tasks
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/ScriptTask.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadStart.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,57 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2007 Samuel Abels
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
-from .BpmnSpecMixin import BpmnSpecMixin
-from ...task import TaskState
-from ...specs.Simple import Simple
-
-
-class ScriptEngineTask(Simple, BpmnSpecMixin):
-    """Task Spec for a bpmn:scriptTask node"""
-
-    def _execute(self, task):
-        """Please override for specific Implementations, see ScriptTask below for an example"""
-        pass
-
-    def _on_complete_hook(self, task):
-        try:
-            self._execute(task)
-            super(ScriptEngineTask, self)._on_complete_hook(task)
-        except Exception as exc:
-            task._set_state(TaskState.WAITING)
-            raise exc
+from .base import TaskSpec
+from SpiffWorkflow.task import TaskState
 
-    def serialize(self, serializer):
-        return serializer.serialize_script_task(self)
 
-    @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_script_task(wf_spec, s_state)
+class ThreadStart(TaskSpec):
 
+    """
+    This class implements the task the is placed at the beginning
+    of each thread. It is NOT supposed to be used! It is purely internal,
+    and used only by the ThreadSplit task.
+    The task has no inputs and at least one output.
+    If more than one output is connected, the task does an implicit
+    parallel split.
+    """
 
-class ScriptTask(ScriptEngineTask):
-
-    def __init__(self, wf_spec, name, script, **kwargs):
+    def __init__(self, wf_spec, name='ThreadStart', **kwargs):
         """
-        Constructor.
+        Constructor. The name of this task is *always* 'ThreadStart'.
 
-        :param script: the script that must be executed by the script engine.
+        :type  wf_spec: WorkflowSpec
+        :param wf_spec: A reference to the workflow specification.
+        :type  kwargs: dict
+        :param kwargs: See :class:`SpiffWorkflow.specs.TaskSpec`.
         """
-        super(ScriptTask, self).__init__(wf_spec, name, **kwargs)
-        self.script = script
+        TaskSpec.__init__(self, wf_spec, name, **kwargs)
+        self.internal = True
 
-    @property
-    def spec_type(self):
-        return 'Script Task'
+    def _run_hook(self, my_task):
+        my_task._assign_new_thread_id()
+        my_task._sync_children(self.outputs, TaskState.READY)
+        return True
 
-    def _execute(self, task):
-        task.workflow.script_engine.execute(task, self.script)
+    def serialize(self, serializer):
+        return serializer.serialize_thread_start(self)
 
+    @classmethod
+    def deserialize(self, serializer, wf_spec, s_state):
+        return serializer.deserialize_thread_start(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/UserTask.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/none_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
-from .BpmnSpecMixin import BpmnSpecMixin
-from ...specs.Simple import Simple
-
-
-class UserTask(Simple, BpmnSpecMixin):
+from SpiffWorkflow.specs.base import TaskSpec
 
-    """
-    Task Spec for a bpmn:userTask node.
-    """
 
-    def is_engine_task(self):
-        return False
+class NoneTask(TaskSpec):
+    """Task Spec for a bpmn:task node."""
 
-    @property
-    def spec_type(self):
-        return 'User Task'
+    def __init__(self, wf_spec, bpmn_id, **kwargs):
+        super().__init__(wf_spec, bpmn_id, **kwargs)
+        self.manual = True
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# -*- coding: utf-8 -*-
 # Copyright (C) 2012 Matthew Hampton
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/StartEvent.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/AcquireMutex.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,66 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2007 Samuel Abels
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
-from .event_types import CatchingEvent
-from ....task import TaskState
-
-
-class StartEvent(CatchingEvent):
-    """Task Spec for a bpmn:startEvent node with an optional event definition."""
+from ..task import TaskState
+from .base import TaskSpec
 
-    def __init__(self, wf_spec, name, event_definition, **kwargs):
-        super(StartEvent, self).__init__(wf_spec, name, event_definition, **kwargs)
 
-    @property
-    def spec_type(self):
-        return f'{self.event_definition.event_type} Start Event'
+class AcquireMutex(TaskSpec):
 
-    def catch(self, my_task, event_definition):
-
-        # We might need to revisit a start event after it completes or
-        # if it got cancelled so we'll still catch messages even if we're finished
-        if my_task.state == TaskState.COMPLETED or my_task.state == TaskState.CANCELLED:
-            my_task.set_children_future()
+    """
+    This class implements a task that acquires a mutex (lock), protecting
+    a section of the workflow from being accessed by other sections.
+    If more than one input is connected, the task performs an implicit
+    multi merge.
+    If more than one output is connected, the task performs an implicit
+    parallel split.
+    """
+
+    def __init__(self, wf_spec, name, mutex, **kwargs):
+        """
+        Constructor.
+
+        :type  wf_spec: WorkflowSpec
+        :param wf_spec: A reference to the workflow specification.
+        :type  name: str
+        :param name: The name of the task spec.
+        :type  mutex: str
+        :param mutex: The name of the mutex that should be acquired.
+        :type  kwargs: dict
+        :param kwargs: See :class:`SpiffWorkflow.specs.TaskSpec`.
+        """
+        assert mutex is not None
+        TaskSpec.__init__(self, wf_spec, name, **kwargs)
+        self.mutex = mutex
+
+    def _update_hook(self, my_task):
+        super()._update_hook(my_task)
+        mutex = my_task.workflow._get_mutex(self.mutex)
+        if mutex.testandset():
+            self.entered_event.emit(my_task.workflow, my_task)
+            return True
+        else:
             my_task._set_state(TaskState.WAITING)
 
-        super(StartEvent, self).catch(my_task, event_definition)
-
     def serialize(self, serializer):
-        return serializer.serialize_generic_event(self)
+        return serializer.serialize_acquire_mutex(self)
 
     @classmethod
-    def deserialize(cls, serializer, wf_spec, s_state):
-        return serializer.deserialize_generic_event(wf_spec, s_state, StartEvent)
-
+    def deserialize(self, serializer, wf_spec, s_state):
+        return serializer.deserialize_acquire_mutex(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/bpmn/specs/events/event_types.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/event_types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,94 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2012 Matthew Hampton
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+import time
+from SpiffWorkflow.task import TaskState
+from SpiffWorkflow.specs.base import TaskSpec
+from ...event_definitions import MessageEventDefinition, NoneEventDefinition, CycleTimerEventDefinition
 
-from .event_definitions import MessageEventDefinition, NoneEventDefinition
-from ..BpmnSpecMixin import BpmnSpecMixin
-from ....specs.Simple import Simple
-from ....task import TaskState
 
-class CatchingEvent(Simple, BpmnSpecMixin):
+class CatchingEvent(TaskSpec):
     """Base Task Spec for Catching Event nodes."""
 
-    def __init__(self, wf_spec, name, event_definition, **kwargs):
+    def __init__(self, wf_spec, bpmn_id, event_definition, **kwargs):
         """
         Constructor.
 
         :param event_definition: the EventDefinition that we must wait for.
         """
-        super(CatchingEvent, self).__init__(wf_spec, name, **kwargs)
+        super(CatchingEvent, self).__init__(wf_spec, bpmn_id, **kwargs)
         self.event_definition = event_definition
 
     def catches(self, my_task, event_definition, correlations=None):
         if self.event_definition == event_definition:
-            return all([ correlations.get(key) == my_task.workflow.correlations.get(key) for key in correlations ])
+            return all([correlations.get(key) == my_task.workflow.correlations.get(key) for key in correlations ])
         else:
             return False
 
     def catch(self, my_task, event_definition):
         """
         Catch is called by the workflow when the task has matched an event
         definition, at which point we can update our task's state.
         """
         self.event_definition.catch(my_task, event_definition)
-        self._update_hook(my_task)
+        my_task.last_update_time = time.time()
+        my_task._set_state(TaskState.WAITING)
 
     def _update_hook(self, my_task):
 
-        if my_task.state == TaskState.WAITING and self.event_definition.has_fired(my_task):
-            my_task._ready()
-        super(CatchingEvent, self)._update_hook(my_task)
-
-    def _on_ready(self, my_task):
-
+        super()._update_hook(my_task)
         # None events don't propogate, so as soon as we're ready, we fire our event
         if isinstance(self.event_definition, NoneEventDefinition):
             my_task._set_internal_data(event_fired=True)
 
-        # If we have not seen the event we're waiting for, enter the waiting state
-        if not self.event_definition.has_fired(my_task):
+        if self.event_definition.has_fired(my_task):
+            return True
+        elif isinstance(self.event_definition, CycleTimerEventDefinition):
+            if self.event_definition.cycle_complete(my_task):
+                for output in self.outputs:
+                    child = my_task._add_child(output, TaskState.READY)
+                    child.task_spec._predict(child, mask=TaskState.READY|TaskState.PREDICTED_MASK)
+                if my_task.state != TaskState.WAITING:
+                    my_task._set_state(TaskState.WAITING)
+        elif my_task.state != TaskState.WAITING:
             my_task._set_state(TaskState.WAITING)
-        super(CatchingEvent, self)._on_ready(my_task)
 
-    def _on_complete_hook(self, my_task):
+    def _run_hook(self, my_task):
 
         if isinstance(self.event_definition, MessageEventDefinition):
             self.event_definition.update_task_data(my_task)
         self.event_definition.reset(my_task)
-        super(CatchingEvent, self)._on_complete_hook(my_task)
+        return super(CatchingEvent, self)._run_hook(my_task)
 
-    def serialize(self, serializer):
-        return serializer.serialize_generic_event(self)
 
-    @classmethod
-    def deserialize(cls, serializer, wf_spec, s_state):
-        return serializer.deserialize_generic_event(wf_spec, s_state, cls)
-
-
-class ThrowingEvent(Simple, BpmnSpecMixin):
+class ThrowingEvent(TaskSpec):
     """Base Task Spec for Throwing Event nodes."""
 
-    def __init__(self, wf_spec, name, event_definition, **kwargs):
+    def __init__(self, wf_spec, bpmn_id, event_definition, **kwargs):
         """
         Constructor.
 
         :param event_definition: the EventDefinition to be thrown.
         """
-        super(ThrowingEvent, self).__init__(wf_spec, name, **kwargs)
+        super(ThrowingEvent, self).__init__(wf_spec, bpmn_id, **kwargs)
         self.event_definition = event_definition
 
-    def _on_complete_hook(self, my_task):
-        super(ThrowingEvent, self)._on_complete_hook(my_task)
+    def _run_hook(self, my_task):
+        super(ThrowingEvent, self)._run_hook(my_task)
         self.event_definition.throw(my_task)
-
-    def serialize(self, serializer):
-        return serializer.serialize_generic_event(self)
-
-    @classmethod
-    def deserialize(cls, serializer, wf_spec, s_state):
-        return serializer.deserialize_generic_event(wf_spec, s_state, cls)
+        return True
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/parser/DMNParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/DMNParser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,131 +1,161 @@
+# Copyright (C) 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3.0 of the License, or (at your option) any later version.
+#
+# SpiffWorkflow is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
+
 import ast
 
-from ...bpmn.parser.util import xpath_eval
+from SpiffWorkflow.bpmn.parser.node_parser import NodeParser, DEFAULT_NSMAP
+from SpiffWorkflow.bpmn.parser.ValidationException import ValidationException
 
-from ...dmn.specs.model import Decision, DecisionTable, InputEntry, \
-    OutputEntry, Input, Output, Rule
+from SpiffWorkflow.bpmn.parser.util import xpath_eval
 
+from SpiffWorkflow.dmn.specs.model import (
+    Decision,
+    DecisionTable,
+    InputEntry,
+    OutputEntry,
+    Input,
+    Output,
+    Rule,
+)
 
 def get_dmn_ns(node):
     """
     Returns the namespace definition for the current DMN
 
     :param node: the XML node for the DMN document
     """
+    nsmap = DEFAULT_NSMAP.copy()
     if 'http://www.omg.org/spec/DMN/20151101/dmn.xsd' in node.nsmap.values():
-        return 'http://www.omg.org/spec/DMN/20151101/dmn.xsd'
+        nsmap['dmn'] = 'http://www.omg.org/spec/DMN/20151101/dmn.xsd'
+    elif 'http://www.omg.org/spec/DMN/20180521/DI/' in node.nsmap.values():
+        nsmap['dmn'] = 'http://www.omg.org/spec/DMN/20180521/DI/'
     elif 'https://www.omg.org/spec/DMN/20191111/MODEL/' in node.nsmap.values():
-        return 'https://www.omg.org/spec/DMN/20191111/MODEL/'
-    return None
-
+        nsmap['dmn'] = 'https://www.omg.org/spec/DMN/20191111/MODEL/'
+    return nsmap
 
-class DMNParser(object):
+class DMNParser(NodeParser):
     """
     Please note this DMN Parser still needs a lot of work.  A few key areas
     that need to be addressed:
     1. it assumes that only one decision table exists within a decision
     2. it is not always name space aware (I fixed the top level, but could be
        cleaner all the way through.
     """
 
     DT_FORMAT = '%Y-%m-%dT%H:%M:%S'
 
-    def __init__(self, p, node, svg=None, filename=None, doc_xpath=None):
+    def __init__(self, p, node, nsmap, svg=None, filename=None):
         """
         Constructor.
 
         :param p: the owning BpmnParser instance
         :param node: the XML node for the DMN document
         :param svg: the SVG representation of this process as a string
           (optional)
         :param filename: the source BMN filename (optional)
         """
+        super().__init__(node, nsmap, filename=filename)
+
         self.parser = p
         self.node = node
         self.decision = None
         self.svg = svg
         self.filename = filename
-        self.doc_xpath = doc_xpath
-        self.dmn_ns = get_dmn_ns(self.node)
-        self.xpath = xpath_eval(self.node, {'dmn': self.dmn_ns})
 
     def parse(self):
         self.decision = self._parse_decision(self.node.findall('{*}decision'))
 
-    def get_id(self):
+    @property
+    def bpmn_id(self):
         """
         Returns the process ID
         """
         return self.node.findall('{*}decision[1]')[0].get('id')
 
     def get_name(self):
         """
         Returns the process name (or ID, if no name is included in the file)
         """
         return self.node.findall('{*}decision[1]')[0].get('name')
 
     def _parse_decision(self, root):
         decision_elements = list(root)
         if len(decision_elements) == 0:
-            raise Exception('No decisions found')
+            raise ValidationException('No decisions found', file_name=self.filename,
+                                      node=root)
 
         if len(decision_elements) > 1:
-            raise Exception('Multiple decisions found')
+            raise ValidationException('Multiple decision tables are not current supported.',
+                                      file_name=self.filename, node=root)
 
         decision_element = decision_elements[0]
-        assert decision_element.tag.endswith(
-            'decision'), 'Element %r is not of type "decision"' % (
-            decision_element.tag)
 
         decision = Decision(decision_element.attrib['id'],
                             decision_element.attrib.get('name', ''))
 
         # Parse decision tables
-        try:
-            self._parse_decision_tables(decision, decision_element)
-        except Exception as e:
-            raise Exception(
-                "Error in Decision '%s': %s" % (decision.name, str(e)))
+        self._parse_decision_tables(decision, decision_element)
 
         return decision
 
     def _parse_decision_tables(self, decision, decisionElement):
         for decision_table_element in decisionElement.findall('{*}decisionTable'):
+            name = decision_table_element.attrib.get('name', '')
+            hitPolicy = decision_table_element.attrib.get('hitPolicy', 'UNIQUE').upper()
             decision_table = DecisionTable(decision_table_element.attrib['id'],
-                                           decision_table_element.attrib.get(
-                                               'name', ''))
+                                           name, hitPolicy)
             decision.decisionTables.append(decision_table)
 
             # parse inputs
             self._parse_inputs_outputs(decision_table, decision_table_element)
 
     def _parse_inputs_outputs(self, decisionTable,
                               decisionTableElement):
+        rule_counter = 0
         for element in decisionTableElement:
             if element.tag.endswith('input'):
                 e_input = self._parse_input(element)
                 decisionTable.inputs.append(e_input)
             elif element.tag.endswith('output'):
                 output = self._parse_output(element)
                 decisionTable.outputs.append(output)
             elif element.tag.endswith('rule'):
-                rule = self._parse_rule(decisionTable, element)
+                rule_counter += 1
+                rule = self._parse_rule(decisionTable, element, rule_counter)
                 decisionTable.rules.append(rule)
             else:
-                raise Exception(
-                    'Unknown type in decision table: %r' % element.tag)
+                raise ValidationException(
+                    'Unknown type in decision table: %r' % element.tag,
+                    node=element, file_name=self.filename)
 
     def _parse_input(self, input_element):
         type_ref = None
-        xpath = xpath_eval(input_element, {'dmn': self.dmn_ns})
+        prefix = self.nsmap['dmn']
+        xpath = xpath_eval(input_element, {'dmn': prefix})
         expression = None
         for input_expression in xpath('dmn:inputExpression'):
             type_ref = input_expression.attrib.get('typeRef', '')
-            expression_node = input_expression.find('{' + self.dmn_ns + '}text')
+            expression_node = input_expression.find('{' + prefix + '}text')
             if expression_node is not None:
                 expression = expression_node.text
 
         return Input(input_element.attrib['id'],
                      input_element.attrib.get('label', ''),
                      input_element.attrib.get('name', ''),
                      expression,
@@ -134,17 +164,17 @@
     def _parse_output(self, outputElement):
         output = Output(outputElement.attrib['id'],
                         outputElement.attrib.get('label', ''),
                         outputElement.attrib.get('name', ''),
                         outputElement.attrib.get('typeRef', ''))
         return output
 
-    def _parse_rule(self, decisionTable, ruleElement):
+    def _parse_rule(self, decisionTable, ruleElement, rowNumber):
         rule = Rule(ruleElement.attrib['id'])
-
+        rule.row_number = rowNumber
         input_idx = 0
         output_idx = 0
         for child in ruleElement:
             # Load description
             if child.tag.endswith('description'):
                 rule.description = child.text
 
@@ -165,26 +195,26 @@
                                                                 output_idx)
                 rule.outputEntries.append(output_entry)
                 output_idx += 1
 
         return rule
 
     def _parse_input_output_element(self, decision_table, element, cls, idx):
-        input_or_output = (
-            decision_table.inputs if cls == InputEntry else decision_table.outputs if cls == OutputEntry else None)[
-            idx]
+        input_or_output = (decision_table.inputs if cls == InputEntry else decision_table.outputs)[idx]
         entry = cls(element.attrib['id'], input_or_output)
         for child in element:
             if child.tag.endswith('description'):
                 entry.description = child.text
             elif child.tag.endswith('text'):
                 entry.text = child.text
         if cls == InputEntry:
-            entry.lhs.append(entry.text)
+            # DMN renders 'no input specification' with '-'; assume this is intended if somebody has added '-'
+            entry.lhs.append(entry.text if entry.text != '-' else None)
         elif cls == OutputEntry:
             if entry.text and entry.text != '':
                 try:
                     ast.parse(entry.text)
                 except Exception as e:
-                    raise Exception(
-                        "Malformed Output Expression '%s'. %s " % (entry.text, str(e)))
+                    raise ValidationException(
+                        "Malformed Output Expression '%s'. %s " % (entry.text, str(e)),
+                        node=element, file_name=self.filename)
         return entry
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/dmn/serializer/task_spec_converters.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/task_spec.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,45 @@
-from ...bpmn.serializer.bpmn_converters import BpmnTaskSpecConverter
+# Copyright (C) 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3.0 of the License, or (at your option) any later version.
+#
+# SpiffWorkflow is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
 
-from ..specs.BusinessRuleTask import BusinessRuleTask
-from ..specs.model import DecisionTable, Rule
+from ...bpmn.serializer.helpers.spec import TaskSpecConverter
+
+from ..specs.model import DecisionTable, Rule, HitPolicy
 from ..specs.model import Input, InputEntry, Output, OutputEntry
 from ..engine.DMNEngine import DMNEngine
 
-class BusinessRuleTaskConverter(BpmnTaskSpecConverter):
-
-    def __init__(self, data_converter=None, typename=None):
-        super().__init__(BusinessRuleTask, data_converter, typename)
+class BaseBusinessRuleTaskConverter(TaskSpecConverter):
 
     def to_dict(self, spec):
         dct = self.get_default_attributes(spec)
-        dct.update(self.get_bpmn_attributes(spec))
         # We only ever use one decision table
         dct['decision_table'] = self.decision_table_to_dict(spec.dmnEngine.decision_table)
         return dct
 
     def decision_table_to_dict(self, table):
         return {
             'id': table.id,
             'name': table.name,
+            'hit_policy': table.hit_policy,
             'inputs': [val.__dict__ for val in table.inputs],
             'outputs': [val.__dict__ for val in table.outputs],
             'rules': [self.rule_to_dict(rule) for rule in table.rules],
         }
 
     def input_entry_to_dict(self, entry):
         return {
@@ -42,26 +57,28 @@
             'text': entry.text,
         }
         return dct
 
     def rule_to_dict(self, rule):
         return {
             'id': rule.id,
+            'row_number': rule.row_number,
             'description': rule.description,
             'input_entries': [self.input_entry_to_dict(entry) for entry in rule.inputEntries],
             'output_entries': [self.output_entry_to_dict(entry) for entry in rule.outputEntries],
         }
 
     def from_dict(self, dct):
         table = self.decision_table_from_dict(dct.pop('decision_table'))
         dct['dmnEngine'] = DMNEngine(table)
         return self.task_spec_from_dict(dct)
 
     def decision_table_from_dict(self, dct):
-        table = DecisionTable(dct['id'], dct['name'])
+        hit_policy = dct.get('hit_policy', HitPolicy.UNIQUE.value)
+        table = DecisionTable(dct['id'], dct['name'], hit_policy)
         table.inputs = [ Input(**val) for val in dct['inputs'] ]
         table.outputs = [ Output(**val) for val in dct['outputs'] ]
         table.rules = [ self.rule_from_dict(rule, table.inputs, table.outputs)
                         for rule in dct['rules'] ]
         return table
 
     def input_entry_from_dict(self, dct, inputs):
@@ -85,12 +102,13 @@
         entry.description = dct['description']
         entry.text = dct['text']
         return entry
 
     def rule_from_dict(self, dct, inputs, outputs):
         rule = Rule(dct['id'])
         rule.description = dct['description']
+        rule.row_number = dct.get('row_number', 0)
         rule.inputEntries = [self.input_entry_from_dict(entry, inputs)
                              for entry in dct['input_entries']]
         rule.outputEntries = [self.output_entry_from_dict(entry, outputs)
                               for entry in dct['output_entries']]
         return rule
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/exceptions.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ReleaseMutex.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,61 @@
-# -*- coding: utf-8 -*-
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
+from .base import TaskSpec
 
-class WorkflowException(Exception):
-    """
-    Base class for all SpiffWorkflow-generated exceptions.
-    """
 
-    def __init__(self, sender, error):
-        """
-        Standard exception class.
+class ReleaseMutex(TaskSpec):
 
-        :param sender: the task spec that threw the exception
-        :type sender: TaskSpec
-        :param error: a human readable error message
-        :type error: string
-        """
-        Exception.__init__(self, str(error))
-        # Points to the TaskSpec that generated the exception.
-        self.sender = sender
-
-    @staticmethod
-    def get_task_trace(task):
-        task_trace = [f"{task.task_spec.description} ({task.workflow.spec.file})"]
-        workflow = task.workflow
-        while workflow != workflow.outer_workflow:
-            caller = workflow.name
-            workflow = workflow.outer_workflow
-            task_trace.append(f"{workflow.spec.task_specs[caller].description} ({workflow.spec.file})")
-        return task_trace
-
-class WorkflowTaskException(WorkflowException):
-    """WorkflowException that provides task_trace information."""
+    """
+    This class implements a task that releases a mutex (lock), protecting
+    a section of the workflow from being accessed by other sections.
+    If more than one input is connected, the task performs an implicit
+    multi merge.
+    If more than one output is connected, the task performs an implicit
+    parallel split.
+    """
 
-    def __init__(self, task, error_msg, exception=None):
+    def __init__(self, wf_spec, name, mutex, **kwargs):
         """
-        Exception initialization.
+        Constructor.
 
-        :param task: the task that threw the exception
-        :type task: Task
-        :param error_msg: a human readable error message
-        :type error_msg: str
-        :param exception: an exception to wrap, if any
-        :type exception: Exception
+        :type  wf_spec: WorkflowSpec
+        :param wf_spec: A reference to the workflow specification.
+        :type  name: str
+        :param name: The name of the task spec.
+        :type  mutex: str
+        :param mutex: The name of the mutex that should be released.
+        :type  kwargs: dict
+        :param kwargs: See :class:`SpiffWorkflow.specs.TaskSpec`.
         """
-
-        self.exception = exception
-        self.task = task
-
-        # If encountered in a sub-workflow, this traces back up the stack
-        # so we can tell how we got to this paticular task, no matter how
-        # deeply nested in sub-workflows it is.  Takes the form of:
-        # task-description (file-name)
-        self.task_trace = self.get_task_trace(task)
-
-        super().__init__(task.task_spec, error_msg)
-
-
-class StorageException(Exception):
-    pass
+        assert mutex is not None
+        TaskSpec.__init__(self, wf_spec, name, **kwargs)
+        self.mutex = mutex
+
+    def _run_hook(self, my_task):
+        mutex = my_task.workflow._get_mutex(self.mutex)
+        mutex.unlock()
+        return True
+
+    def serialize(self, serializer):
+        return serializer.serialize_release_mutex(self)
+
+    @classmethod
+    def deserialize(self, serializer, wf_spec, s_state):
+        return serializer.deserialize_release_mutex(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/operators.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 import logging
 import re
 
 logger = logging.getLogger('spiff')
 
 
 class Term(object):
@@ -221,15 +222,15 @@
     def _get_values(self, task):
         values = []
         for arg in self.args:
             values.append(str(valueof(task, arg)))
         return values
 
     def _matches(self, task):
-        raise Exception("Abstract class, do not call")
+        raise NotImplementedError("Abstract class, do not call")
 
     def serialize(self, serializer):
         """
         Serializes the instance using the provided serializer.
 
         :type  serializer: :class:`SpiffWorkflow.serializer.base.Serializer`
         :param serializer: The serializer to use.
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/dict.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/dict.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,70 @@
-# -*- coding: utf-8 -*-
-
-
-import json
-from builtins import str
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
+import json
+
 import pickle
 from base64 import b64encode, b64decode
 from ..workflow import Workflow
 from ..util.impl import get_class
-from ..task import Task
-from ..operators import (Attrib, PathAttrib, Equal, NotEqual,
-                         Operator, GreaterThan, LessThan, Match)
-from ..specs import (Cancel, AcquireMutex, CancelTask, Celery, Choose,
-                     ExclusiveChoice, Execute, Gate, Join, MultiChoice,
-                     MultiInstance, ReleaseMutex, Simple, WorkflowSpec,
-                     TaskSpec, SubWorkflow, StartTask, ThreadMerge,
-                     ThreadSplit, ThreadStart, Merge, Trigger, LoopResetTask)
+from ..task import Task, TaskState
+from ..operators import Attrib, PathAttrib, Equal, NotEqual, Operator, GreaterThan, LessThan, Match
+from ..specs.base import TaskSpec
+from ..specs.AcquireMutex import AcquireMutex
+from ..specs.Cancel import Cancel
+from ..specs.CancelTask import CancelTask
+from ..specs.Choose import Choose
+from ..specs.ExclusiveChoice import ExclusiveChoice
+from ..specs.Execute import Execute
+from ..specs.Gate import Gate
+from ..specs.Join import Join
+from ..specs.Merge import Merge
+from ..specs.MultiChoice import MultiChoice
+from ..specs.MultiInstance import MultiInstance
+from ..specs.ReleaseMutex import ReleaseMutex
+from ..specs.Simple import Simple
+from ..specs.StartTask import StartTask
+from ..specs.SubWorkflow import SubWorkflow
+from ..specs.ThreadStart import ThreadStart
+from ..specs.ThreadMerge import ThreadMerge
+from ..specs.ThreadSplit import ThreadSplit
+from ..specs.Trigger import Trigger
+from ..specs.WorkflowSpec import WorkflowSpec
 from .base import Serializer
 from .exceptions import TaskNotSupportedError, MissingSpecError
 import warnings
 
 class DictionarySerializer(Serializer):
 
-    def __init__(self):
-        # When deserializing, this is a set of specs for sub-workflows.
-        # This prevents us from serializing a copy of the same spec many
-        # times, which can create very large files.
-        self.SPEC_STATES = {}
-
     def serialize_dict(self, thedict):
         return dict(
-            (str(k), b64encode(pickle.dumps(v,
-                                            protocol=pickle.HIGHEST_PROTOCOL)))
-            for k, v in list(thedict.items()))
+            (str(k), b64encode(pickle.dumps(v, protocol=pickle.HIGHEST_PROTOCOL)))
+            for k, v in list(thedict.items())
+        )
 
     def deserialize_dict(self, s_state):
-        return dict((k, pickle.loads(b64decode(v)))
-                    for k, v in list(s_state.items()))
+        return dict((k, pickle.loads(b64decode(v))) for k, v in list(s_state.items()))
 
     def serialize_list(self, thelist):
-        return [b64encode(pickle.dumps(v, protocol=pickle.HIGHEST_PROTOCOL))
-                for v in thelist]
+        return [b64encode(pickle.dumps(v, protocol=pickle.HIGHEST_PROTOCOL)) for v in thelist]
 
     def deserialize_list(self, s_state):
         return [pickle.loads(b64decode(v)) for v in s_state]
 
     def serialize_attrib(self, attrib):
         return attrib.name
 
@@ -129,58 +136,42 @@
         ret = arg_cls.deserialize(self, arg)
         if isinstance(ret,list):
             return arg_cls(*ret)
         else:
             return ret
 
     def serialize_task_spec(self, spec):
-        s_state = dict(id=spec.id,
-                       name=spec.name,
+        s_state = dict(name=spec.name,
                        description=spec.description,
                        manual=spec.manual,
-                       internal=spec.internal,
                        lookahead=spec.lookahead)
         module_name = spec.__class__.__module__
         s_state['class'] = module_name + '.' + spec.__class__.__name__
-        s_state['inputs'] = [t.id for t in spec.inputs]
-        s_state['outputs'] = [t.id for t in spec.outputs]
+        s_state['inputs'] = [t.name for t in spec.inputs]
+        s_state['outputs'] = [t.name for t in spec.outputs]
         s_state['data'] = self.serialize_dict(spec.data)
-        if hasattr(spec, 'position'):
-            s_state['position'] = self.serialize_dict(spec.position)
-
         s_state['defines'] = self.serialize_dict(spec.defines)
         s_state['pre_assign'] = self.serialize_list(spec.pre_assign)
         s_state['post_assign'] = self.serialize_list(spec.post_assign)
-        s_state['locks'] = spec.locks[:]
-
         # Note: Events are not serialized; this is documented in
         # the TaskSpec API docs.
-
         return s_state
 
     def deserialize_task_spec(self, wf_spec, s_state, spec):
-        spec.id = s_state.get('id', None)
         spec.description = s_state.get('description', '')
         spec.manual = s_state.get('manual', False)
-        spec.internal = s_state.get('internal', False)
         spec.lookahead = s_state.get('lookahead', 2)
-
         spec.data = self.deserialize_dict(s_state.get('data', {}))
-        if 'position' in s_state.keys():
-            spec.position = self.deserialize_dict(s_state.get('position', {}))
         spec.defines = self.deserialize_dict(s_state.get('defines', {}))
         spec.pre_assign = self.deserialize_list(s_state.get('pre_assign', []))
-        spec.post_assign = self.deserialize_list(
-            s_state.get('post_assign', []))
-        spec.locks = s_state.get('locks', [])[:]
+        spec.post_assign = self.deserialize_list(s_state.get('post_assign', []))
         # We can't restore inputs and outputs yet because they may not be
         # deserialized yet. So keep the names, and resolve them in the end.
         spec.inputs = s_state.get('inputs', [])[:]
         spec.outputs = s_state.get('outputs', [])[:]
-
         return spec
 
     def serialize_acquire_mutex(self, spec):
         s_state = self.serialize_task_spec(spec)
         s_state['mutex'] = spec.mutex
         return s_state
 
@@ -192,50 +183,29 @@
 
     def serialize_cancel(self, spec):
         s_state = self.serialize_task_spec(spec)
         s_state['cancel_successfully'] = spec.cancel_successfully
         return s_state
 
     def deserialize_cancel(self, wf_spec, s_state):
-        spec = Cancel(wf_spec, s_state['name'],
-                      success=s_state.get('cancel_successfully', False))
+        spec = Cancel(wf_spec, s_state['name'], success=s_state.get('cancel_successfully', False))
         self.deserialize_task_spec(wf_spec, s_state, spec=spec)
         return spec
 
     def serialize_cancel_task(self, spec):
         return self.serialize_trigger(spec)
 
     def deserialize_cancel_task(self, wf_spec, s_state):
         spec = CancelTask(wf_spec,
                           s_state['name'],
                           s_state['context'],
                           times=self.deserialize_arg(s_state['times']))
         self.deserialize_task_spec(wf_spec, s_state, spec=spec)
         return spec
 
-    def serialize_celery(self, spec):
-        args = self.serialize_list(spec.args)
-        kwargs = self.serialize_dict(spec.kwargs)
-        s_state = self.serialize_task_spec(spec)
-        s_state['call'] = spec.call
-        s_state['args'] = args
-        s_state['kwargs'] = kwargs
-        s_state['result_key'] = spec.result_key
-        return s_state
-
-    def deserialize_celery(self, wf_spec, s_state):
-        args = self.deserialize_list(s_state['args'])
-        kwargs = self.deserialize_dict(s_state.get('kwargs', {}))
-        spec = Celery(wf_spec, s_state['name'], s_state['call'],
-                      call_args=args,
-                      result_key=s_state['result_key'],
-                      **kwargs)
-        self.deserialize_task_spec(wf_spec, s_state, spec)
-        return spec
-
     def serialize_choose(self, spec):
         s_state = self.serialize_task_spec(spec)
         s_state['context'] = spec.context
         # despite the various documentation suggesting that choice ought to be
         # a collection of objects, here it is a collection of strings. The
         # handler in MultiChoice.py converts it to TaskSpecs. So instead of:
         # s_state['choice'] = [c.name for c in spec.choice]
@@ -279,40 +249,28 @@
         return s_state
 
     def deserialize_gate(self, wf_spec, s_state):
         spec = Gate(wf_spec, s_state['name'], s_state['context'])
         self.deserialize_task_spec(wf_spec, s_state, spec=spec)
         return spec
 
-    def serialize_loop_reset_task(self, spec):
-        s_state = self.serialize_task_spec(spec)
-        s_state['destination_id'] = spec.destination_id
-        s_state['destination_spec_name'] = spec.destination_spec_name
-        return s_state
-
-    def deserialize_loop_reset_task(self, wf_spec, s_state):
-        spec = LoopResetTask(wf_spec, s_state['name'], s_state['destination_id'],
-                             s_state['destination_spec_name'])
-        self.deserialize_task_spec(wf_spec, s_state, spec=spec)
-        return spec
-
     def serialize_join(self, spec):
         s_state = self.serialize_task_spec(spec)
         s_state['split_task'] = spec.split_task
         s_state['threshold'] = b64encode(
             pickle.dumps(spec.threshold, protocol=pickle.HIGHEST_PROTOCOL))
         s_state['cancel_remaining'] = spec.cancel_remaining
         return s_state
 
-    def deserialize_join(self, wf_spec, s_state, cls=Join):
+    def deserialize_join(self, wf_spec, s_state):
         if isinstance(s_state['threshold'],dict):
             byte_payload = s_state['threshold']['__bytes__']
         else:
             byte_payload = s_state['threshold']
-        spec = cls(wf_spec,
+        spec = Join(wf_spec,
                     s_state['name'],
                     split_task=s_state['split_task'],
                     threshold=pickle.loads(b64decode(byte_payload)),
                     cancel=s_state['cancel_remaining'])
         self.deserialize_task_spec(wf_spec, s_state, spec=spec)
         return spec
 
@@ -341,44 +299,33 @@
         self.deserialize_task_spec(wf_spec, s_state, spec=spec)
         return spec
 
     def serialize_multi_instance(self, spec):
         s_state = self.serialize_task_spec(spec)
         # here we need to add in all of the things that would get serialized
         # for other classes that the MultiInstance could be -
-        #
-
         if isinstance(spec, SubWorkflow):
             br_state = self.serialize_sub_workflow(spec)
             s_state['file'] = br_state['file']
             s_state['in_assign'] = br_state['in_assign']
             s_state['out_assign'] = br_state['out_assign']
-
         s_state['times'] = self.serialize_arg(spec.times)
-        s_state['prevtaskclass'] = spec.prevtaskclass
         return s_state
 
-    def deserialize_multi_instance(self, wf_spec, s_state, cls=None):
-        if cls == None:
-            cls = MultiInstance(wf_spec,
-                         s_state['name'],
-                         times=self.deserialize_arg(s_state['times']))
-        if isinstance(s_state['times'],list):
-            s_state['times'] = self.deserialize_arg(s_state['times'])
-            cls.times = s_state['times']
-        if isinstance(cls, SubWorkflow):
+    def deserialize_multi_instance(self, wf_spec, s_state):
+        spec = MultiInstance(wf_spec, s_state['name'], times=self.deserialize_arg(s_state['times']))
+        if isinstance(spec, SubWorkflow):
             if s_state.get('file'):
-                cls.file = self.deserialize_arg(s_state['file'])
+                spec.file = self.deserialize_arg(s_state['file'])
             else:
-                cls.file = None
-            cls.in_assign = self.deserialize_list(s_state['in_assign'])
-            cls.out_assign = self.deserialize_list(s_state['out_assign'])
-
-        self.deserialize_task_spec(wf_spec, s_state, spec=cls)
-        return cls
+                spec.file = None
+            spec.in_assign = self.deserialize_list(s_state['in_assign'])
+            spec.out_assign = self.deserialize_list(s_state['out_assign'])
+        self.deserialize_task_spec(wf_spec, s_state, spec=spec)
+        return spec
 
     def serialize_release_mutex(self, spec):
         s_state = self.serialize_task_spec(spec)
         s_state['mutex'] = spec.mutex
         return s_state
 
     def deserialize_release_mutex(self, wf_spec, s_state):
@@ -392,15 +339,14 @@
 
     def deserialize_simple(self, wf_spec, s_state):
         assert isinstance(wf_spec, WorkflowSpec)
         spec = Simple(wf_spec, s_state['name'])
         self.deserialize_task_spec(wf_spec, s_state, spec=spec)
         return spec
 
-
     def deserialize_generic(self, wf_spec, s_state,newclass):
         assert isinstance(wf_spec, WorkflowSpec)
         spec = newclass(wf_spec, s_state['name'])
         self.deserialize_task_spec(wf_spec, s_state, spec=spec)
         return spec
 
     def serialize_start_task(self, spec):
@@ -480,248 +426,147 @@
                        s_state['name'],
                        s_state['context'],
                        self.deserialize_arg(s_state['times']))
         self.deserialize_task_spec(wf_spec, s_state, spec=spec)
         return spec
 
     def serialize_workflow_spec(self, spec, **kwargs):
-        s_state = dict(name=spec.name,
-                       description=spec.description,
-                       file=spec.file)
-
-        if 'Root' not in spec.task_specs:
-            # This is to fix up the case when we
-            # load in a task spec and there is no root object.
-            # it causes problems when we deserialize and then re-serialize
-            # because the deserialize process adds a root.
-            root = Simple(spec, 'Root')
-            spec.task_specs['Root'] = root
-
-        mylist = [(k, v.serialize(self)) for k, v in list(spec.task_specs.items())]
-
-        # As we serialize back up, keep only one copy of any sub_workflow
-        s_state['sub_workflows'] = {}
-        for name, task in mylist:
-            if 'spec' in task:
-                spec = json.loads(task['spec'])
-                if 'sub_workflows' in spec:
-                    s_state['sub_workflows'].update(spec['sub_workflows'])
-                    del spec['sub_workflows']
-                if spec['name'] not in s_state['sub_workflows']:
-                    s_state['sub_workflows'][spec['name']] = json.dumps(spec)
-                task['spec_name'] = spec['name']
-                del task['spec']
-
-        if hasattr(spec,'end'):
-            s_state['end']=spec.end.id
-        s_state['task_specs'] = dict(mylist)
+        s_state = dict(name=spec.name, description=spec.description, file=spec.file)
+        s_state['task_specs'] = dict(
+            (k, v.serialize(self))
+            for k, v in list(spec.task_specs.items())
+        )
         return s_state
 
     def _deserialize_workflow_spec_task_spec(self, spec, task_spec, name):
-        task_spec.inputs = [spec.get_task_spec_from_id(t) for t in task_spec.inputs]
-        task_spec.outputs = [spec.get_task_spec_from_id(t) for t in task_spec.outputs]
-
-    def _prevtaskclass_bases(self, oldtask):
-        return (oldtask)
+        task_spec.inputs = [spec.get_task_spec_from_name(t) for t in task_spec.inputs]
+        task_spec.outputs = [spec.get_task_spec_from_name(t) for t in task_spec.outputs]
 
     def deserialize_workflow_spec(self, s_state, **kwargs):
         spec = WorkflowSpec(s_state['name'], filename=s_state['file'])
         spec.description = s_state['description']
+
         # Handle Start Task
         spec.start = None
-
-        # Store all sub-workflows so they can be referenced.
-        if 'sub_workflows' in s_state:
-            # Hate the whole json dumps thing, why do we do this?
-            self.SPEC_STATES.update(s_state['sub_workflows'])
-
         del spec.task_specs['Start']
         start_task_spec_state = s_state['task_specs']['Start']
-        start_task_spec = StartTask.deserialize(
-            self, spec, start_task_spec_state)
+        start_task_spec = StartTask.deserialize(self, spec, start_task_spec_state)
         spec.start = start_task_spec
+
         spec.task_specs['Start'] = start_task_spec
         for name, task_spec_state in list(s_state['task_specs'].items()):
             if name == 'Start':
                 continue
-            prevtask = task_spec_state.get('prevtaskclass', None)
-            if prevtask:
-                oldtask = get_class(prevtask)
-                task_spec_cls = type(task_spec_state['class'],
-                      self._prevtaskclass_bases(oldtask), {})
-            else:
-                task_spec_cls = get_class(task_spec_state['class'])
+            task_spec_cls = get_class(task_spec_state['class'])
             task_spec = task_spec_cls.deserialize(self, spec, task_spec_state)
             spec.task_specs[name] = task_spec
 
         for name, task_spec in list(spec.task_specs.items()):
             self._deserialize_workflow_spec_task_spec(spec, task_spec, name)
 
         if s_state.get('end', None):
-            spec.end = spec.get_task_spec_from_id(s_state['end'])
+            spec.end = spec.get_task_spec_from_name(s_state['end'])
 
         assert spec.start is spec.get_task_spec_from_name('Start')
         return spec
 
     def serialize_workflow(self, workflow, include_spec=True, **kwargs):
 
         assert isinstance(workflow, Workflow)
         s_state = dict()
         if include_spec:
-            s_state['wf_spec'] = self.serialize_workflow_spec(workflow.spec,
-                                                              **kwargs)
+            s_state['wf_spec'] = self.serialize_workflow_spec(workflow.spec, **kwargs)
 
-        # data
         s_state['data'] = self.serialize_dict(workflow.data)
-
-        # last_node
         value = workflow.last_task
         s_state['last_task'] = value.id if value is not None else None
-
-        # outer_workflow
-        # s_state['outer_workflow'] = workflow.outer_workflow.id
-
-        # success
         s_state['success'] = workflow.success
-
-        # task_tree
         s_state['task_tree'] = self.serialize_task(workflow.task_tree)
 
         return s_state
 
-    def deserialize_workflow(self, s_state, wf_class=Workflow,
-                             read_only=False, wf_spec=None, **kwargs):
+    def deserialize_workflow(self, s_state, wf_class=Workflow, **kwargs):
         """It is possible to override the workflow class, and specify a
         workflow_spec, otherwise the spec is assumed to be serialized in the
         s_state['wf_spec']"""
 
-        if wf_spec is None:
-            wf_spec = self.deserialize_workflow_spec(s_state['wf_spec'], **kwargs)
-        workflow = wf_class(wf_spec)
-
-        workflow.read_only = read_only
+        if isinstance(s_state['wf_spec'], str):
+            spec_dct = json.loads(s_state['wf_spec'])
+        else:
+            spec_dct = s_state['wf_spec']
+        reset_specs = [spec['name'] for spec in spec_dct['task_specs'].values() if spec['class'].endswith('LoopResetTask')]
+        for name in reset_specs:
+            s_state['wf_spec']['task_specs'].pop(name)
+        wf_spec = self.deserialize_workflow_spec(s_state['wf_spec'], **kwargs)
 
-        # data
+        workflow = wf_class(wf_spec)
         workflow.data = self.deserialize_dict(s_state['data'])
-
-        # outer_workflow
-        # workflow.outer_workflow =
-        # find_workflow_by_id(remap_workflow_id(s_state['outer_workflow']))
-
-        # success
         workflow.success = s_state['success']
-
-        # workflow
         workflow.spec = wf_spec
+        workflow.task_tree = self.deserialize_task(workflow, s_state['task_tree'], reset_specs)
 
-        # task_tree
-        workflow.task_tree = self.deserialize_task(
-            workflow, s_state['task_tree'])
-
-        # Re-connect parents
-        tasklist = list(workflow.get_tasks())
+        # Re-connect parents and update states if necessary
+        tasklist = workflow.get_tasks()
+        root = workflow.get_tasks_from_spec_name('Root')[0]
+        update_state = root.state != TaskState.COMPLETED
         for task in tasklist:
-            task.parent = workflow.get_task(task.parent,tasklist)
+            if task.parent is not None:
+                task.parent = workflow.get_task_from_id(task.parent, tasklist)
+            if update_state:
+                if task.state == 32:
+                    task.state = TaskState.COMPLETED
+                elif task.state == 64:
+                    task.state = TaskState.CANCELLED
 
-        # last_task
-        workflow.last_task = workflow.get_task(s_state['last_task'],tasklist)
-
-        # task_mapping
+        if workflow.last_task is not None:
+            workflow.last_task = workflow.get_task_from_id(s_state['last_task'],tasklist)
         workflow.update_task_mapping()
 
         return workflow
 
-
-    def serialize_task(self, task, skip_children=False, allow_subs=False):
-        """
-             :param allow_subs: Allows sub-serialization to take place, otherwise
-             assumes that the subworkflow is stored in internal data and raises an error.
-        """
-
+    def serialize_task(self, task, skip_children=False):
         assert isinstance(task, Task)
-
-        # Please note, the BPMN Serializer DOES allow sub-workflows.  This is
-        # for backwards compatibility and support of the original parsers.
-        if not allow_subs and isinstance(task.task_spec, SubWorkflow):
+        if isinstance(task.task_spec, SubWorkflow):
             raise TaskNotSupportedError(
                 "Subworkflow tasks cannot be serialized (due to their use of" +
                 " internal_data to store the subworkflow).")
-
         s_state = dict()
-
-        # id
         s_state['id'] = task.id
-
-        # workflow
         s_state['workflow_name'] = task.workflow.name
-
-        # parent
         s_state['parent'] = task.parent.id if task.parent is not None else None
-
-        # children
         if not skip_children:
-            s_state['children'] = [
-                self.serialize_task(child) for child in task.children]
-
-        # state
+            s_state['children'] = [self.serialize_task(child) for child in task.children]
         s_state['state'] = task.state
         s_state['triggered'] = task.triggered
-
-        # task_spec
         s_state['task_spec'] = task.task_spec.name
-
-        # last_state_change
         s_state['last_state_change'] = task.last_state_change
-
-        # data
         s_state['data'] = self.serialize_dict(task.data)
-
-        # internal_data
         s_state['internal_data'] = task.internal_data
-
         return s_state
 
-
-    def deserialize_task(self, workflow, s_state):
+    def deserialize_task(self, workflow, s_state, ignored_specs=None):
         assert isinstance(workflow, Workflow)
-        splits = s_state['task_spec'].split('_')
-        oldtaskname = s_state['task_spec']
-        task_spec = workflow.get_task_spec_from_name(oldtaskname)
+        old_spec_name = s_state['task_spec']
+        if old_spec_name in ignored_specs:
+            return None
+        task_spec = workflow.get_task_spec_from_name(old_spec_name)
         if task_spec is None:
-            raise MissingSpecError("Unknown task spec: " + oldtaskname)
+            raise MissingSpecError("Unknown task spec: " + old_spec_name)
         task = Task(workflow, task_spec)
 
-        if getattr(task_spec,'isSequential',False) and \
-            s_state['internal_data'].get('splits') is not None:
-            task.task_spec.expanded = s_state['internal_data']['splits']
-
-
-        # id
         task.id = s_state['id']
-
-        # parent
         # as the task_tree might not be complete yet
         # keep the ids so they can be processed at the end
         task.parent = s_state['parent']
-
-        # children
-        task.children = self._deserialize_task_children(task, s_state)
-
-        # state
+        task.children = self._deserialize_task_children(task, s_state, ignored_specs)
         task._state = s_state['state']
         task.triggered = s_state['triggered']
-
-        # last_state_change
         task.last_state_change = s_state['last_state_change']
-
-        # data
         task.data = self.deserialize_dict(s_state['data'])
-
-        # internal_data
         task.internal_data = s_state['internal_data']
         return task
 
-    def _deserialize_task_children(self, task, s_state):
+    def _deserialize_task_children(self, task, s_state, ignored_specs):
         """This may need to be overridden if you need to support
          deserialization of sub-workflows"""
-        return [self.deserialize_task(task.workflow, c)
-                         for c in s_state['children']]
+        children = [self.deserialize_task(task.workflow, c, ignored_specs) for c in s_state['children']]
+        return [c for c in children if c is not None]
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/dotv.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/dotv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# -*- coding: utf-8 -*-
-
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/json.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/json.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,59 @@
-# -*- coding: utf-8 -*-
-
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 import json
 import uuid
 from ..operators import Attrib
 from .dict import DictionarySerializer
 
 class JSONSerializer(DictionarySerializer):
 
     def serialize_workflow_spec(self, wf_spec, **kwargs):
-        thedict = super(JSONSerializer, self).serialize_workflow_spec(
-            wf_spec, **kwargs)
+        thedict = super(JSONSerializer, self).serialize_workflow_spec(wf_spec, **kwargs)
         return self._dumps(thedict)
 
     def deserialize_workflow_spec(self, s_state, **kwargs):
         thedict = self._loads(s_state)
-        return super(JSONSerializer, self).deserialize_workflow_spec(
-            thedict, **kwargs)
+        return super(JSONSerializer, self).deserialize_workflow_spec(thedict, **kwargs)
 
     def serialize_workflow(self, workflow, **kwargs):
-        thedict = super(JSONSerializer, self).serialize_workflow(
-            workflow, **kwargs)
+        thedict = super(JSONSerializer, self).serialize_workflow(workflow, **kwargs)
         return self._dumps(thedict)
 
     def deserialize_workflow(self, s_state, **kwargs):
         thedict = self._loads(s_state)
-        return super(JSONSerializer, self).deserialize_workflow(
-            thedict, **kwargs)
+        return super(JSONSerializer, self).deserialize_workflow(thedict, **kwargs)
 
     def _object_hook(self, dct):
         if '__uuid__' in dct:
             return uuid.UUID(dct['__uuid__'])
 
         if '__bytes__' in dct:
             return dct['__bytes__'].encode('ascii')
 
         if '__attrib__' in dct:
             return Attrib(dct['__attrib__'])
 
         return dct
 
-    def _jsonableHandler(self, obj):
-        if hasattr(obj, 'jsonable'):
-            return obj.jsonable()
-
-        raise 'Object of type %s with value of %s is not JSON serializable' % (
-            type(obj), repr(obj))
-
-
     def _default(self, obj):
         if isinstance(obj, uuid.UUID):
             return {'__uuid__': obj.hex}
 
         if isinstance(obj, bytes):
             return {'__bytes__': obj.decode('ascii')}
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/serializer/xml.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/xml.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# -*- coding: utf-8 -*-
-
-from builtins import str
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-import re
+
 import warnings
 from lxml import etree
 from lxml.etree import SubElement
 from ..workflow import Workflow
-from .. import specs, operators
 from ..task import Task, TaskStateNames
-from ..operators import (Attrib, Assign, PathAttrib, Equal, NotEqual,
-                         GreaterThan, LessThan, Match)
-from ..specs import (Cancel, AcquireMutex, CancelTask, Celery, Choose,
-                     ExclusiveChoice, Execute, Gate, Join, MultiChoice,
-                     MultiInstance, ReleaseMutex, Simple, WorkflowSpec,
-                     SubWorkflow, StartTask, ThreadMerge,
-                     ThreadSplit, ThreadStart, Merge, Trigger, LoopResetTask)
-from .base import Serializer
+from ..operators import (Attrib, Assign, PathAttrib, Equal, NotEqual, GreaterThan, LessThan, Match)
+from ..specs.AcquireMutex import AcquireMutex
+from ..specs.Cancel import Cancel
+from ..specs.CancelTask import CancelTask
+from ..specs.Choose import Choose
+from ..specs.ExclusiveChoice import ExclusiveChoice
+from ..specs.Execute import Execute
+from ..specs.Gate import Gate
+from ..specs.Join import Join
+from ..specs.Merge import Merge
+from ..specs.MultiChoice import MultiChoice
+from ..specs.MultiInstance import MultiInstance
+from ..specs.ReleaseMutex import ReleaseMutex
+from ..specs.Simple import Simple
+from ..specs.StartTask import StartTask
+from ..specs.SubWorkflow import SubWorkflow
+from ..specs.ThreadStart import ThreadStart
+from ..specs.ThreadMerge import ThreadMerge
+from ..specs.ThreadSplit import ThreadSplit
+from ..specs.Trigger import Trigger
+from ..specs.WorkflowSpec import WorkflowSpec
+from .base import Serializer, spec_map, op_map
 from .exceptions import TaskNotSupportedError
 
 # Create a list of tag names out of the spec names.
-_spec_map = dict()
-for name in dir(specs):
-    if name.startswith('_'):
-        continue
-    module = specs.__dict__[name]
-    name = re.sub(r'(.)([A-Z])', r'\1-\2', name).lower()
-    _spec_map[name] = module
-_spec_map['task'] = specs.Simple
-
-_op_map = {'equals':       operators.Equal,
-           'not-equals':   operators.NotEqual,
-           'less-than':    operators.LessThan,
-           'greater-than': operators.GreaterThan,
-           'matches':      operators.Match}
+_spec_map = spec_map()
+_op_map = op_map()
 
 
 class XmlSerializer(Serializer):
 
     def serialize_attrib(self, op):
         """
         Serializer for :meth:`SpiffWorkflow.operators.Attrib`.
@@ -282,23 +282,19 @@
         cls = _op_map[elem.tag]
         return cls.deserialize(self, elem)
 
     def serialize_task_spec(self, spec, elem):
         """
         Serializes common attributes of :meth:`SpiffWorkflow.specs.TaskSpec`.
         """
-        if spec.id is not None:
-            SubElement(elem, 'id').text = str(spec.id)
         SubElement(elem, 'name').text = spec.name
         if spec.description:
             SubElement(elem, 'description').text = spec.description
         if spec.manual:
             SubElement(elem, 'manual')
-        if spec.internal:
-            SubElement(elem, 'internal')
         SubElement(elem, 'lookahead').text = str(spec.lookahead)
         inputs = [t.name for t in spec.inputs]
         outputs = [t.name for t in spec.outputs]
         self.serialize_value_list(SubElement(elem, 'inputs'), inputs)
         self.serialize_value_list(SubElement(elem, 'outputs'), outputs)
         self.serialize_value_map(SubElement(elem, 'data'), spec.data)
         self.serialize_value_map(SubElement(elem, 'defines'), spec.defines)
@@ -311,19 +307,16 @@
         # the TaskSpec API docs.
 
         return elem
 
     def deserialize_task_spec(self, wf_spec, elem, spec_cls, **kwargs):
         name = elem.findtext('name')
         spec = spec_cls(wf_spec, name, **kwargs)
-        theid = elem.findtext('id')
-        spec.id = theid if theid is not None else None
         spec.description = elem.findtext('description', spec.description)
         spec.manual = elem.findtext('manual', spec.manual)
-        spec.internal = elem.find('internal') is not None
         spec.lookahead = int(elem.findtext('lookahead', spec.lookahead))
 
         data_elem = elem.find('data')
         if data_elem is not None:
             spec.data = self.deserialize_value_map(data_elem)
         defines_elem = elem.find('defines')
         if defines_elem is not None:
@@ -379,45 +372,14 @@
     def serialize_cancel_task(self, spec):
         elem = etree.Element('cancel-task')
         return self.serialize_trigger(spec, elem)
 
     def deserialize_cancel_task(self, wf_spec, elem, cls=CancelTask, **kwargs):
         return self.deserialize_trigger(wf_spec, elem, cls, **kwargs)
 
-    def serialize_celery(self, spec, elem=None):
-        if elem is None:
-            elem = etree.Element('celery')
-
-        SubElement(elem, 'call').text = spec.call
-        args_elem = SubElement(elem, 'args')
-        self.serialize_value_list(args_elem, spec.args)
-        kwargs_elem = SubElement(elem, 'kwargs')
-        self.serialize_value_map(kwargs_elem, spec.kwargs)
-        if spec.merge_results:
-            SubElement(elem, 'merge-results')
-        SubElement(elem, 'result-key').text = spec.result_key
-
-        return self.serialize_task_spec(spec, elem)
-
-    def deserialize_celery(self, wf_spec, elem, cls=Celery, **kwargs):
-        call = elem.findtext('call')
-        args = self.deserialize_value_list(elem.find('args'))
-        result_key = elem.findtext('call')
-        merge_results = elem.find('merge-results') is not None
-        spec = self.deserialize_task_spec(wf_spec,
-                                          elem,
-                                          cls,
-                                          call=call,
-                                          call_args=args,
-                                          result_key=result_key,
-                                          merge_results=merge_results,
-                                          **kwargs)
-        spec.kwargs = self.deserialize_value_map(elem.find('kwargs'))
-        return spec
-
     def serialize_choose(self, spec, elem=None):
         if elem is None:
             elem = etree.Element('choose')
         elem = self.serialize_task_spec(spec, elem)
         SubElement(elem, 'context').text = spec.context
         choice_elem = SubElement(elem, 'choice')
         self.serialize_value_list(choice_elem, spec.choice)
@@ -716,39 +678,25 @@
         # workflow.outer_workflow =
         # find_workflow_by_id(remap_workflow_id(elem['outer_workflow']))
 
         task_tree_elem = elem.find('task-tree')
         workflow.task_tree = self.deserialize_task(workflow, task_tree_elem[0])
 
         # Re-connect parents
-        for task in workflow.get_tasks():
-            task.parent = workflow.get_task(task.parent)
+        for task in workflow.get_tasks_iterator():
+            if task.parent is not None:
+                task.parent = workflow.get_task_from_id(task.parent)
 
         # last_task
         last_task = elem.findtext('last-task')
         if last_task is not None:
-            workflow.last_task = workflow.get_task(last_task)
+            workflow.last_task = workflow.get_task_from_id(last_task)
 
         return workflow
 
-    def serialize_loop_reset_task(self, spec):
-        elem = etree.Element('loop-reset-task')
-        SubElement(elem, 'destination_id').text = str(spec.destination_id)
-        SubElement(elem, 'destination_spec_name').text = str(spec.destination_spec_name)
-        return self.serialize_task_spec(spec, elem)
-
-    def deserialize_loop_reset_task(self, wf_spec, elem, cls=LoopResetTask, **kwargs):
-        destination_id = elem.findtext('destination_id')
-        destination_spec_name = elem.findtext('destination_spec_name')
-
-        task = self.deserialize_task_spec(wf_spec, elem, cls,
-                                          destination_id=destination_id,
-                                          destination_spec_name=destination_spec_name)
-        return task
-
     def serialize_task(self, task, skip_children=False):
         assert isinstance(task, Task)
 
         if isinstance(task.task_spec, SubWorkflow):
             raise TaskNotSupportedError(
                 "Subworkflow tasks cannot be serialized (due to their use of" +
                 " internal_data to store the subworkflow).")
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/AcquireMutex.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Execute.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,88 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
-# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,MA  02110-1301  USA
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
+
+import subprocess
+
 from ..task import TaskState
 from .base import TaskSpec
 
 
-class AcquireMutex(TaskSpec):
+class Execute(TaskSpec):
 
     """
-    This class implements a task that acquires a mutex (lock), protecting
-    a section of the workflow from being accessed by other sections.
-    If more than one input is connected, the task performs an implicit
-    multi merge.
-    If more than one output is connected, the task performs an implicit
-    parallel split.
+    This class executes an external process, goes into WAITING until the
+    process is complete, and returns the results of the execution.
+
+    Usage:
+
+    task = Execute(spec, 'Ping', args=["ping", "-t", "1", "127.0.0.1"])
+        ... when workflow complete
+    print workflow.get_task('Ping').results
     """
 
-    def __init__(self, wf_spec, name, mutex, **kwargs):
+    def __init__(self, wf_spec, name, args=None, **kwargs):
         """
         Constructor.
 
         :type  wf_spec: WorkflowSpec
         :param wf_spec: A reference to the workflow specification.
         :type  name: str
         :param name: The name of the task spec.
-        :type  mutex: str
-        :param mutex: The name of the mutex that should be acquired.
+        :type  args: list
+        :param args: args to pass to process (first arg is the command).
         :type  kwargs: dict
-        :param kwargs: See :class:`SpiffWorkflow.specs.TaskSpec`.
+        :param kwargs: kwargs to pass-through to TaskSpec initializer.
         """
-        assert mutex is not None
+        assert wf_spec is not None
+        assert name is not None
         TaskSpec.__init__(self, wf_spec, name, **kwargs)
-        self.mutex = mutex
+        self.args = args
+
+    def _start(self, my_task, force=False):
+        """Returns False when successfully fired, True otherwise"""
+        if (not hasattr(my_task, 'subprocess')) or my_task.subprocess is None:
+            my_task.subprocess = subprocess.Popen(self.args,
+                                                  stderr=subprocess.STDOUT,
+                                                  stdout=subprocess.PIPE)
+
+        if my_task.subprocess:
+            my_task.subprocess.poll()
+            if my_task.subprocess.returncode is None:
+                # Still waiting
+                return False
+            else:
+                results = my_task.subprocess.communicate()
+                my_task.results = results
+                return True
+        return False
 
     def _update_hook(self, my_task):
-        mutex = my_task.workflow._get_mutex(self.mutex)
-        if mutex.testandset():
-            self.entered_event.emit(my_task.workflow, my_task)
-            my_task._ready()
-            return
-        my_task._set_state(TaskState.WAITING)
+        super()._update_hook(my_task)
+        if not self._start(my_task):
+            my_task._set_state(TaskState.WAITING)
+        else:
+            return True
 
     def serialize(self, serializer):
-        return serializer.serialize_acquire_mutex(self)
+        return serializer.serialize_execute(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_acquire_mutex(wf_spec, s_state)
+        spec = serializer.deserialize_execute(wf_spec, s_state)
+        return spec
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Cancel.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Cancel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..exceptions import WorkflowException
 from .base import TaskSpec
 
 
 class Cancel(TaskSpec):
 
     """
@@ -49,19 +50,19 @@
     def test(self):
         """
         Checks whether all required attributes are set. Throws an exception
         if an error was detected.
         """
         TaskSpec.test(self)
         if len(self.outputs) > 0:
-            raise WorkflowException(self, 'Cancel with an output.')
+            raise WorkflowException('Cancel with an output.', task_spec=self)
 
-    def _on_complete_hook(self, my_task):
+    def _run_hook(self, my_task):
         my_task.workflow.cancel(self.cancel_successfully)
-        TaskSpec._on_complete_hook(self, my_task)
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_cancel(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_cancel(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/CancelTask.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/CancelTask.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from .base import TaskSpec
+
 from .Trigger import Trigger
 
 
 class CancelTask(Trigger):
 
     """
     This class implements a trigger that cancels another task (branch).
     If more than one input is connected, the task performs an implicit
     multi merge.
     If more than one output is connected, the task performs an implicit
     parallel split.
     """
 
-    def _on_complete_hook(self, my_task):
+    def _run_hook(self, my_task):
         for task_name in self.context:
             cancel_tasks = my_task.workflow.get_task_spec_from_name(task_name)
             for cancel_task in my_task._get_root()._find_any(cancel_tasks):
                 cancel_task.cancel()
-        TaskSpec._on_complete_hook(self, my_task)
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_cancel_task(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_cancel_task(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Choose.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Choose.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from .base import TaskSpec
 from .Trigger import Trigger
 
 
 class Choose(Trigger):
 
     """
@@ -51,26 +52,26 @@
         assert name is not None
         assert context is not None
         # HACK: inherit from TaskSpec (not Trigger) on purpose.
         TaskSpec.__init__(self, wf_spec, name, **kwargs)
         self.context = context
         self.choice = choice is not None and choice or []
 
-    def _on_complete_hook(self, my_task):
+    def _run_hook(self, my_task):
         context = my_task.workflow.get_task_spec_from_name(self.context)
         triggered = []
         for task in my_task.workflow.task_tree:
             if task.thread_id != my_task.thread_id:
                 continue
             if task.task_spec == context:
                 task.trigger(self.choice)
                 triggered.append(task)
         for task in triggered:
             context._predict(task)
-        TaskSpec._on_complete_hook(self, my_task)
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_choose(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_choose(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ExclusiveChoice.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ExclusiveChoice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..task import TaskState
 from ..exceptions import WorkflowException
 from .MultiChoice import MultiChoice
 
 
 class ExclusiveChoice(MultiChoice):
 
@@ -49,51 +50,38 @@
         Connects the task spec that is executed if no other condition
         matches.
 
         :type  task_spec: TaskSpec
         :param task_spec: The following task spec.
         """
         assert self.default_task_spec is None
-        self.outputs.append(task_spec)
         self.default_task_spec = task_spec.name
-        task_spec._connect_notify(self)
+        super().connect(task_spec)
 
     def test(self):
-        """
-        Checks whether all required attributes are set. Throws an exception
-        if an error was detected.
-        """
-        MultiChoice.test(self)
+        super().test()
         if self.default_task_spec is None:
-            raise WorkflowException(self, 'A default output is required.')
+            raise WorkflowException('A default output is required.', task_spec=self)
 
-    def _predict_hook(self, my_task):
-        # If the task's status is not predicted, we default to MAYBE
-        # for all it's outputs except the default choice, which is
-        # LIKELY.
-        # Otherwise, copy my own state to the children.
-        my_task._sync_children(self.outputs)
-        spec = self._wf_spec.get_task_spec_from_name(self.default_task_spec)
-        my_task._set_likely_task(spec)
+    def _run_hook(self, my_task):
 
-    def _on_complete_hook(self, my_task):
-        # Find the first matching condition.
         output = self._wf_spec.get_task_spec_from_name(self.default_task_spec)
         for condition, spec_name in self.cond_task_specs:
-            if condition is None or condition._matches(my_task):
+            if condition is not None and condition._matches(my_task):
                 output = self._wf_spec.get_task_spec_from_name(spec_name)
                 break
 
         if output is None:
-            raise WorkflowException(self,
-                f'No conditions satisfied for {my_task.task_spec.name}')
+            raise WorkflowException(f'No conditions satisfied for {my_task.task_spec.name}', task_spec=self)
 
         my_task._sync_children([output], TaskState.FUTURE)
         for child in my_task.children:
-            child.task_spec._update(child)
+            child.task_spec._predict(child, mask=TaskState.FUTURE|TaskState.PREDICTED_MASK)
+        
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_exclusive_choice(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_exclusive_choice(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Gate.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Gate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..task import TaskState
 from .base import TaskSpec
 
 
 class Gate(TaskSpec):
 
     """
@@ -48,23 +49,24 @@
         assert wf_spec is not None
         assert name is not None
         assert context is not None
         TaskSpec.__init__(self, wf_spec, name, **kwargs)
         self.context = context
 
     def _update_hook(self, my_task):
+        super()._update_hook(my_task)
         context_task = my_task.workflow.get_task_spec_from_name(self.context)
         root_task = my_task.workflow.task_tree
         for task in root_task._find_any(context_task):
             if task.thread_id != my_task.thread_id:
                 continue
             if not task._has_state(TaskState.COMPLETED):
                 my_task._set_state(TaskState.WAITING)
                 return
-        super(Gate, self)._update_hook(my_task)
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_gate(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_gate(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Join.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Join.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..task import Task, TaskState
 from ..exceptions import WorkflowException
 from .base import TaskSpec
 from ..operators import valueof
 
 
 class Join(TaskSpec):
@@ -116,63 +117,79 @@
                 continue
             # Merge found.
             if child.task_spec == self:
                 return True
             # If the task is predicted with less outputs than he has
             # children, that means the prediction may be incomplete (for
             # example, because a prediction is not yet possible at this time).
-            if not child._is_definite() \
-                    and len(child.task_spec.outputs) > len(child.children):
+            if child._is_predicted() and len(child.task_spec.outputs) > len(child.children):
                 return True
         return False
 
+    def _get_split_task(self, my_task):
+        # One Join spec may have multiple corresponding Task objects::
+        #
+        #     - Due to the MultiInstance pattern.
+        #     - Due to the ThreadSplit pattern.
+        #
+        # When using the MultiInstance pattern, we want to join across
+        # the resulting task instances. When using the ThreadSplit
+        # pattern, we only join within the same thread. (Both patterns
+        # may also be mixed.)
+        #
+        # We are looking for all task instances that must be joined.
+        # We limit our search by starting at the split point.
+        if self.split_task:
+            task_spec = my_task.workflow.get_task_spec_from_name(self.split_task)
+            split_task = my_task._find_ancestor(task_spec)
+        else:
+            split_task = my_task.workflow.task_tree
+        return split_task
+
     def _check_threshold_unstructured(self, my_task, force=False):
         # The default threshold is the number of inputs.
         threshold = valueof(my_task, self.threshold)
         if threshold is None:
             threshold = len(self.inputs)
 
         # Look at the tree to find all places where this task is used.
         tasks = []
-        for input in self.inputs:
-            tasks += my_task.workflow.task_mapping[my_task.thread_id][input]
+        for spec in self.inputs:
+            tasks.extend([ t for t in  my_task.workflow.task_tree._find_any(spec) if t.thread_id == my_task.thread_id ])
 
         # Look up which tasks have already completed.
         waiting_tasks = []
         completed = 0
         for task in tasks:
             if task.parent is None or task._has_state(TaskState.COMPLETED):
                 completed += 1
-            else:
+            elif not task._is_finished():
                 waiting_tasks.append(task)
 
         # If the threshold was reached, get ready to fire.
         return force or completed >= threshold, waiting_tasks
 
     def _check_threshold_structured(self, my_task, force=False):
         # Retrieve a list of all activated tasks from the associated
         # task that did the conditional parallel split.
         split_task = my_task._find_ancestor_from_name(self.split_task)
         if split_task is None:
             msg = 'Join with %s, which was not reached' % self.split_task
-            raise WorkflowException(self, msg)
+            raise WorkflowException(msg, task_spec=self)
         tasks = split_task.task_spec._get_activated_tasks(split_task, my_task)
 
         # The default threshold is the number of branches that were started.
         threshold = valueof(my_task, self.threshold)
         if threshold is None:
             threshold = len(tasks)
 
         # Look up which tasks have already completed.
         waiting_tasks = []
         completed = 0
         for task in tasks:
-            # Refresh path prediction.
-            task.task_spec._predict(task)
-
             if not self._branch_may_merge_at(task):
                 completed += 1
             elif self._branch_is_complete(task):
                 completed += 1
             else:
                 waiting_tasks.append(task)
 
@@ -181,116 +198,74 @@
 
     def _start(self, my_task, force=False):
         """
         Checks whether the preconditions for going to READY state are met.
         Returns True if the threshold was reached, False otherwise.
         Also returns the list of tasks that yet need to be completed.
         """
-        # If the threshold was already reached, there is nothing else to do.
-        if my_task._has_state(TaskState.COMPLETED):
-            return True, None
+        if my_task._is_finished():
+            return False, None
         if my_task._has_state(TaskState.READY):
             return True, None
 
         # Check whether we may fire.
         if self.split_task is None:
             return self._check_threshold_unstructured(my_task, force)
-        return self._check_threshold_structured(my_task, force)
+        else:
+            return self._check_threshold_structured(my_task, force)
 
     def _update_hook(self, my_task):
         # Check whether enough incoming branches have completed.
+        my_task._inherit_data()
         may_fire, waiting_tasks = self._start(my_task)
-        if not may_fire:
+        if may_fire:
+            # If this is a cancelling join, cancel all incoming branches except for the one that just completed.
+            if self.cancel_remaining:
+                for task in waiting_tasks:
+                    task.cancel()
+            # Update the state of our child objects.
+            self._do_join(my_task)
+            return True
+        elif not my_task._is_finished():
             my_task._set_state(TaskState.WAITING)
-            return
-
-        # If this is a cancelling join, cancel all incoming branches,
-        # except for the one that just completed.
-        if self.cancel_remaining:
-            for task in waiting_tasks:
-                task.cancel()
-
-        # We do NOT set the task state to COMPLETED, because in
-        # case all other incoming tasks get cancelled (or never reach
-        # the Join for other reasons, such as reaching a stub branch),
-        # we need to revisit it.
-        my_task._ready()
 
-        # Update the state of our child objects.
-        self._do_join(my_task)
-
-    def _do_join(self, my_task):
-        # One Join spec may have multiple corresponding Task objects::
-        #
-        #     - Due to the MultiInstance pattern.
-        #     - Due to the ThreadSplit pattern.
-        #
-        # When using the MultiInstance pattern, we want to join across
-        # the resulting task instances. When using the ThreadSplit
-        # pattern, we only join within the same thread. (Both patterns
-        # may also be mixed.)
-        #
-        # We are looking for all task instances that must be joined.
-        # We limit our search by starting at the split point.
-        if self.split_task:
-            split_task = my_task.workflow.get_task_spec_from_name(
-                self.split_task)
-            split_task = my_task._find_ancestor(split_task)
-        else:
-            split_task = my_task.workflow.task_tree
+    def _find_tasks(self, my_task):
 
+        split_task = self._get_split_task(my_task)
         # Identify all corresponding task instances within the thread.
-        # Also remember which of those instances was most recently changed,
-        # because we are making this one the instance that will
-        # continue the thread of control. In other words, we will continue
-        # to build the task tree underneath the most recently changed task.
-        last_changed = None
         thread_tasks = []
         for task in split_task._find_any(self):
             # Ignore tasks from other threads.
             if task.thread_id != my_task.thread_id:
                 continue
             # Ignore my outgoing branches.
             if self.split_task and task._is_descendant_of(my_task):
                 continue
-
             # We have found a matching instance.
             thread_tasks.append(task)
+        return thread_tasks
 
-            # Check whether the state of the instance was recently
-            # changed.
-            changed = task.parent.last_state_change
-            if last_changed is None \
-                    or changed > last_changed.parent.last_state_change:
-                last_changed = task
-
-        # Mark the identified task instances as COMPLETED. The exception
-        # is the most recently changed task, for which we assume READY.
-        # By setting the state to READY only, we allow for calling
-        # :class:`Task.complete()`, which leads to the task tree being
-        # (re)built underneath the node.
-        for task in thread_tasks:
-            if task == last_changed:
-                self.entered_event.emit(my_task.workflow, my_task)
-                task._ready()
-            else:
-                task._set_state(TaskState.COMPLETED)
-                task._drop_children()
-
+    def _do_join(self, my_task):
 
+        # Execution will continue from this task; mark others as cancelled
+        for task in self._find_tasks(my_task):
+            if task != my_task:
+                task._set_state(TaskState.CANCELLED)
+                task._drop_children()
 
     def _on_trigger(self, my_task):
         """
         May be called to fire the Join before the incoming branches are
         completed.
         """
-        for task in my_task.workflow.task_tree._find_any(self):
-            if task.thread_id != my_task.thread_id:
-                continue
-            self._do_join(task)
+        tasks = sorted(self._find_tasks(my_task), key=lambda t: t.last_state_change)
+        for task in tasks[:-1]:
+            task._set_state(TaskState.CANCELLED)
+            task._drop_children()
+        tasks[-1]._ready()
 
     def serialize(self, serializer):
         return serializer.serialize_join(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_join(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Merge.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Merge.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/MultiChoice.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/MultiChoice.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..task import TaskState
 from ..exceptions import WorkflowException
 from .base import TaskSpec
 
 
 class MultiChoice(TaskSpec):
 
@@ -66,80 +67,61 @@
     def test(self):
         """
         Checks whether all required attributes are set. Throws an exception
         if an error was detected.
         """
         TaskSpec.test(self)
         if len(self.cond_task_specs) < 1:
-            raise WorkflowException(self, 'At least one output required.')
+            raise WorkflowException('At least one output required.', task_spec=self)
         for condition, name in self.cond_task_specs:
             if name is None:
-                raise WorkflowException(self, 'Condition with no task spec.')
+                raise WorkflowException('Condition with no task spec.', task_spec=self)
             task_spec = self._wf_spec.get_task_spec_from_name(name)
             if task_spec is None:
                 msg = 'Condition leads to non-existent task ' + repr(name)
-                raise WorkflowException(self, msg)
+                raise WorkflowException(msg, task_spec=self)
             if condition is None:
                 continue
 
     def _on_trigger(self, my_task, choice):
         """
         Lets a caller narrow down the choice by using a Choose trigger.
         """
         self.choice = choice
         # The caller needs to make sure that predict() is called.
 
     def _predict_hook(self, my_task):
-        if self.choice:
-            outputs = [self._wf_spec.get_task_spec_from_name(o)
-                       for o in self.choice]
-        else:
-            outputs = self.outputs
-
-        # Default to MAYBE for all conditional outputs, default to LIKELY
-        # for unconditional ones. We can not default to FUTURE, because
-        # a call to trigger() may override the unconditional paths.
-        my_task._sync_children(outputs)
-        if not my_task._is_definite():
-            best_state = my_task.state
-        else:
-            best_state = TaskState.LIKELY
-
-        # Collect a list of all unconditional outputs.
-        outputs = []
+        conditional, unconditional = [], []
         for condition, output in self.cond_task_specs:
-            if condition is None:
-                outputs.append(self._wf_spec.get_task_spec_from_name(output))
-
-        for child in my_task.children:
-            if child._is_definite():
+            if self.choice is not None and output not in self.choice:
                 continue
-            if child.task_spec in outputs:
-                child._set_state(best_state)
+            if condition is None:
+                unconditional.append(self._wf_spec.get_task_spec_from_name(output))
+            else:
+                conditional.append(self._wf_spec.get_task_spec_from_name(output))
+        state = TaskState.MAYBE if my_task.state == TaskState.MAYBE else TaskState.LIKELY
+        my_task._sync_children(unconditional, state)
+        for spec in conditional:
+            my_task._add_child(spec, TaskState.MAYBE)
 
-    def _on_complete_hook(self, my_task):
-        """
-        Runs the task. Should not be called directly.
-        Returns True if completed, False otherwise.
-        """
-        # Find all matching conditions.
+    def _get_matching_outputs(self, my_task):
         outputs = []
         for condition, output in self.cond_task_specs:
             if self.choice is not None and output not in self.choice:
                 continue
-            if condition is None:
+            if condition is None or condition._matches(my_task):
                 outputs.append(self._wf_spec.get_task_spec_from_name(output))
-                continue
-            if not condition._matches(my_task):
-                continue
-            outputs.append(self._wf_spec.get_task_spec_from_name(output))
+        return outputs
 
-        my_task._sync_children(outputs, TaskState.FUTURE)
+    def _run_hook(self, my_task):
+        """Runs the task. Should not be called directly."""
+        my_task._sync_children(self._get_matching_outputs(my_task), TaskState.FUTURE)
         for child in my_task.children:
-            child.task_spec._update(child)
+            child.task_spec._predict(child, mask=TaskState.FUTURE|TaskState.PREDICTED_MASK)
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_multi_choice(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_multi_choice(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/MultiInstance.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/MultiInstance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# -*- coding: utf-8 -*-
-
-from builtins import range
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..task import TaskState
 from .base import TaskSpec
 from ..operators import valueof
 
 
 class MultiInstance(TaskSpec):
 
@@ -47,15 +47,14 @@
         :type  kwargs: dict
         :param kwargs: See :class:`SpiffWorkflow.specs.TaskSpec`.
         """
         if times is None:
             raise ValueError('times argument is required')
         TaskSpec.__init__(self, wf_spec, name, **kwargs)
         self.times = times
-        self.prevtaskclass = None
 
     def _find_my_task(self, task):
         for thetask in task.workflow.task_tree:
             if thetask.thread_id != task.thread_id:
                 continue
             if thetask.task_spec == self:
                 return thetask
@@ -71,43 +70,32 @@
         if my_task._has_state(TaskState.COMPLETED):
             state = TaskState.READY
         else:
             state = TaskState.FUTURE
         for output in self.outputs:
             new_task = my_task._add_child(output, state)
             new_task.triggered = True
-            output._predict(new_task)
+            output._predict(new_task, mask=TaskState.FUTURE|TaskState.READY|TaskState.PREDICTED_MASK)
 
     def _get_predicted_outputs(self, my_task):
         split_n = int(valueof(my_task, self.times, 1))
-
-        # Predict the outputs.
-        outputs = []
-        for i in range(split_n):
-            outputs += self.outputs
-        return outputs
+        return self.outputs * split_n
 
     def _predict_hook(self, my_task):
-        split_n = int(valueof(my_task, self.times, 1))
-        my_task._set_internal_data(splits=split_n)
-
-        # Create the outgoing tasks.
-        outputs = []
-        for i in range(split_n):
-            outputs += self.outputs
+        outputs = self._get_predicted_outputs(my_task)
         if my_task._is_definite():
             my_task._sync_children(outputs, TaskState.FUTURE)
         else:
             my_task._sync_children(outputs, TaskState.LIKELY)
 
-    def _on_complete_hook(self, my_task):
+    def _run_hook(self, my_task):
         outputs = self._get_predicted_outputs(my_task)
         my_task._sync_children(outputs, TaskState.FUTURE)
-        for child in my_task.children:
-            child.task_spec._update(child)
+        self._predict(my_task, mask=TaskState.FUTURE|TaskState.PREDICTED_MASK)
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_multi_instance(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_multi_instance(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ReleaseMutex.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/bpmn_process_spec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,50 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from .base import TaskSpec
 
+from SpiffWorkflow.specs.WorkflowSpec import WorkflowSpec
+from SpiffWorkflow.bpmn.specs.control import _EndJoin, BpmnStartTask, SimpleBpmnTask
 
-class ReleaseMutex(TaskSpec):
 
+class BpmnProcessSpec(WorkflowSpec):
     """
-    This class implements a task that releases a mutex (lock), protecting
-    a section of the workflow from being accessed by other sections.
-    If more than one input is connected, the task performs an implicit
-    multi merge.
-    If more than one output is connected, the task performs an implicit
-    parallel split.
+    This class represents the specification of a BPMN process workflow. This
+    specialises the standard Spiff WorkflowSpec class with a few extra methods
+    and attributes.
     """
 
-    def __init__(self, wf_spec, name, mutex, **kwargs):
+    def __init__(self, name=None, description=None, filename=None, svg=None):
         """
         Constructor.
 
-        :type  wf_spec: WorkflowSpec
-        :param wf_spec: A reference to the workflow specification.
-        :type  name: str
-        :param name: The name of the task spec.
-        :type  mutex: str
-        :param mutex: The name of the mutex that should be released.
-        :type  kwargs: dict
-        :param kwargs: See :class:`SpiffWorkflow.specs.TaskSpec`.
+        :param svg: This provides the SVG representation of the workflow as an
+        LXML node. (optional)
         """
-        assert mutex is not None
-        TaskSpec.__init__(self, wf_spec, name, **kwargs)
-        self.mutex = mutex
-
-    def _on_complete_hook(self, my_task):
-        mutex = my_task.workflow._get_mutex(self.mutex)
-        mutex.unlock()
-        TaskSpec._on_complete_hook(self, my_task)
-
-    def serialize(self, serializer):
-        return serializer.serialize_release_mutex(self)
-
-    @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_release_mutex(wf_spec, s_state)
+        super(BpmnProcessSpec, self).__init__(name=name, filename=filename, nostart=True)
+        # Add a root task to ensure all tasks in the workflow are bpmn tasks
+        # The serializer ignores this task
+        SimpleBpmnTask(self, 'Root')
+        self.start = BpmnStartTask(self, 'Start')
+        self.end = _EndJoin(self, '%s.EndJoin' % (self.name))
+        self.end.connect(SimpleBpmnTask(self, 'End'))
+        self.svg = svg
+        self.description = description
+        self.io_specification = None
+        self.data_objects = {}
+        self.data_stores = {}
+        self.correlation_keys = {}
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Simple.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/user_task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,27 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from .base import TaskSpec
-
-
-class Simple(TaskSpec):
 
-    """
-    This class implements a task with one or more inputs and
-    any number of outputs.
-    If more than one input is connected, the task performs an implicit
-    multi merge.
-    If more than one output is connected, the task performs an implicit
-    parallel split.
-    """
+from SpiffWorkflow.specs.base import TaskSpec
 
-    def serialize(self, serializer):
-        return serializer.serialize_simple(self)
+class UserTask(TaskSpec):
+    """Task Spec for a bpmn:userTask node."""
 
-    @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_simple(wf_spec, s_state)
+    def __init__(self, wf_spec, bpmn_id, **kwargs):
+        super().__init__(wf_spec, bpmn_id, **kwargs)
+        self.manual = True
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/SubWorkflow.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/SubWorkflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 import os
 
-from . import StartTask
+from lxml import etree
+
+from .StartTask import StartTask
 from .base import TaskSpec
 from ..task import TaskState
 from ..exceptions import WorkflowException
 from ..operators import valueof
 
 
 class SubWorkflow(TaskSpec):
@@ -68,84 +71,76 @@
         if file is not None:
             dirname = os.path.dirname(wf_spec.file)
             self.file = os.path.join(dirname, file)
 
     def test(self):
         TaskSpec.test(self)
         if self.file is not None and not os.path.exists(self.file):
-            raise WorkflowException(
-                self, 'File does not exist: %s' % self.file)
+            raise WorkflowException('File does not exist: %s' % self.file, task_spec=self)
 
     def _predict_hook(self, my_task):
+        # Modifying the task spec is a TERRIBLE idea, but if we don't do it, sync_children won't work
         outputs = [task.task_spec for task in my_task.children]
         for output in self.outputs:
             if output not in outputs:
                 outputs.insert(0, output)
         if my_task._is_definite():
-            my_task._sync_children(outputs, TaskState.FUTURE)
+            # This prevents errors with sync children
+            my_task._sync_children(outputs, TaskState.LIKELY)
         else:
             my_task._sync_children(outputs, my_task.state)
 
     def _create_subworkflow(self, my_task):
         from ..serializer.prettyxml import XmlSerializer
-        from ..specs import WorkflowSpec
+        from ..specs.WorkflowSpec import WorkflowSpec
         from ..workflow import Workflow
         file_name = valueof(my_task, self.file)
         serializer = XmlSerializer()
         with open(file_name) as fp:
-            xml = fp.read()
-        wf_spec = WorkflowSpec.deserialize(
-            serializer, xml, filename=file_name)
+            xml = etree.parse(fp).getroot()
+        wf_spec = WorkflowSpec.deserialize(serializer, xml, filename=file_name)
         outer_workflow = my_task.workflow.outer_workflow
-        return Workflow(wf_spec, parent=outer_workflow)
-
-    def _on_ready_before_hook(self, my_task):
-        subworkflow = self._create_subworkflow(my_task)
-        subworkflow.completed_event.connect(
-            self._on_subworkflow_completed, my_task)
-        self._integrate_subworkflow_tree(my_task, subworkflow)
-        my_task._set_internal_data(subworkflow=subworkflow)
-
-    def _integrate_subworkflow_tree(self, my_task, subworkflow):
-        # Integrate the tree of the subworkflow into the tree of this workflow.
+        subworkflow = Workflow(wf_spec, parent=outer_workflow)
         my_task._sync_children(self.outputs, TaskState.FUTURE)
-        for child in my_task.children:
-            child.task_spec._update(child)
-            child._inherit_data()
         for child in subworkflow.task_tree.children:
             my_task.children.insert(0, child)
             child.parent = my_task
+            child.state = TaskState.READY
+        subworkflow.completed_event.connect(self._on_subworkflow_completed, my_task)
+        my_task._set_internal_data(subworkflow=subworkflow)
+        my_task._set_state(TaskState.WAITING)
 
-    def _on_ready_hook(self, my_task):
+    def _run_hook(self, my_task):
         # Assign variables, if so requested.
         subworkflow = my_task._get_internal_data('subworkflow')
         for child in subworkflow.task_tree.children:
             for assignment in self.in_assign:
                 assignment.assign(my_task, child)
-
-        self._predict(my_task)
-        for child in subworkflow.task_tree.children:
             child.task_spec._update(child)
+        return True
+
+    def _update_hook(self, my_task):
+        super()._update_hook(my_task)
+        subworkflow = my_task._get_internal_data('subworkflow')
+        if subworkflow is None:
+            self._create_subworkflow(my_task)
+        elif subworkflow.is_completed():
+            my_task.complete()
 
     def _on_subworkflow_completed(self, subworkflow, my_task):
         # Assign variables, if so requested.
         for child in my_task.children:
             if not isinstance(child.task_spec, StartTask):
                 if subworkflow.last_task is not None:
                     child.data = subworkflow.last_task.data
                 for assignment in self.out_assign:
                     assignment.assign(subworkflow, child)
 
                 # Alright, abusing that hook is just evil but it works.
                 child.task_spec._update_hook(child)
 
-    def _on_complete_hook(self, my_task):
-        for child in my_task.children:
-            if isinstance(child.task_spec, StartTask):
-                child.task_spec._update(child)
-
     def serialize(self, serializer):
         return serializer.serialize_sub_workflow(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_sub_workflow(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ThreadMerge.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadMerge.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..task import TaskState
 from ..exceptions import WorkflowException
 from ..operators import valueof
-from ..specs import Join
+from ..specs.Join import Join
 
 
 class ThreadMerge(Join):
 
     """
     This class represents a task for synchronizing branches that were
     previously split using a a ThreadSplit.
@@ -58,16 +59,15 @@
         if my_task._has_state(TaskState.READY):
             return True
 
         # Retrieve a list of all activated tasks from the associated
         # task that did the conditional parallel split.
         split_task = my_task._find_ancestor_from_name(self.split_task)
         if split_task is None:
-            msg = 'Join with %s, which was not reached' % self.split_task
-            raise WorkflowException(self, msg)
+            raise WorkflowException(f'Join with %s, which was not reached {self.split_task}', task_spec=self)
         tasks = split_task.task_spec._get_activated_threads(split_task)
 
         # The default threshold is the number of threads that were started.
         threshold = valueof(my_task, self.threshold)
         if threshold is None:
             threshold = len(tasks)
 
@@ -95,20 +95,21 @@
         # We do NOT set the task state to COMPLETED, because in
         # case all other incoming tasks get cancelled (or never reach
         # the ThreadMerge for other reasons, such as reaching a stub branch),
         # we need to revisit it.
         return False
 
     def _update_hook(self, my_task):
+
+        my_task._inherit_data()
         if not self._start(my_task):
             my_task._set_state(TaskState.WAITING)
             return
 
-        split_task_spec = my_task.workflow.get_task_spec_from_name(
-            self.split_task)
+        split_task_spec = my_task.workflow.get_task_spec_from_name(self.split_task)
         split_task = my_task._find_ancestor(split_task_spec)
 
         # Find the inbound task that was completed last.
         last_changed = None
         tasks = []
         for task in split_task._find_any(self):
             if self.split_task and task._is_descendant_of(my_task):
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ThreadSplit.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadSplit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# -*- coding: utf-8 -*-
-
-from builtins import range
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..task import TaskState
 from .base import TaskSpec
 from .ThreadStart import ThreadStart
 from ..operators import valueof
 
 
 class ThreadSplit(TaskSpec):
@@ -104,41 +104,33 @@
         May be called after execute() was already completed to create an
         additional outbound task.
         """
         for output in self.outputs:
             new_task = my_task.add_child(output, TaskState.READY)
             new_task.triggered = True
 
-    def _predict_hook(self, my_task):
+    def _get_predicted_outputs(self, my_task):
         split_n = int(valueof(my_task, self.times))
+        return [self.thread_starter] * split_n
 
+    def _predict_hook(self, my_task):
         # if we were created with thread_starter suppressed, connect it now.
         if self.thread_starter is None:
             self.thread_starter = self.outputs[0]
 
-        # Predict the outputs.
-        outputs = []
-        for i in range(split_n):
-            outputs.append(self.thread_starter)
+        outputs = self._get_predicted_outputs(my_task)
         if my_task._is_definite():
             my_task._sync_children(outputs, TaskState.FUTURE)
         else:
             my_task._sync_children(outputs, TaskState.LIKELY)
 
-    def _on_complete_hook(self, my_task):
-        # Split, and remember the number of splits in the context data.
-        split_n = int(valueof(my_task, self.times))
-
-        # Create the outgoing tasks.
-        outputs = []
-        for i in range(split_n):
-            outputs.append(self.thread_starter)
+    def _run_hook(self, my_task):
+        outputs = self._get_predicted_outputs(my_task)
         my_task._sync_children(outputs, TaskState.FUTURE)
-        for child in my_task.children:
-            child.task_spec._update(child)
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_thread_split(self)
 
     @classmethod
     def deserialize(self, serializer, wf_spec, s_state):
         return serializer.deserialize_thread_split(wf_spec, s_state)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/ThreadStart.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/script_task.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,46 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-from .base import TaskSpec
 
+from SpiffWorkflow.specs.base import TaskSpec
+
+
+class ScriptEngineTask(TaskSpec):
+    """Task Spec for a bpmn:scriptTask node"""
+
+    def _execute(self, task):
+        """Please override for specific Implementations, see ScriptTask below for an example"""
+        pass
+
+    def _run_hook(self, task):
+        return self._execute(task)
 
-class ThreadStart(TaskSpec):
 
-    """
-    This class implements the task the is placed at the beginning
-    of each thread. It is NOT supposed to be used! It is purely internal,
-    and used only by the ThreadSplit task.
-    The task has no inputs and at least one output.
-    If more than one output is connected, the task does an implicit
-    parallel split.
-    """
+class ScriptTask(ScriptEngineTask):
 
-    def __init__(self, wf_spec, name='ThreadStart', **kwargs):
+    def __init__(self, wf_spec, bpmn_id, script, **kwargs):
         """
-        Constructor. The name of this task is *always* 'ThreadStart'.
+        Constructor.
 
-        :type  wf_spec: WorkflowSpec
-        :param wf_spec: A reference to the workflow specification.
-        :type  kwargs: dict
-        :param kwargs: See :class:`SpiffWorkflow.specs.TaskSpec`.
+        :param script: the script that must be executed by the script engine.
         """
-        TaskSpec.__init__(self, wf_spec, name, **kwargs)
-        self.internal = True
+        super(ScriptTask, self).__init__(wf_spec, bpmn_id, **kwargs)
+        self.script = script
 
-    def _on_complete_hook(self, my_task):
-        my_task._assign_new_thread_id()
-        TaskSpec._on_complete_hook(self, my_task)
-
-    def serialize(self, serializer):
-        return serializer.serialize_thread_start(self)
-
-    @classmethod
-    def deserialize(self, serializer, wf_spec, s_state):
-        return serializer.deserialize_thread_start(wf_spec, s_state)
+    def _execute(self, task):
+        return task.workflow.script_engine.execute(task, self.script)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Transform.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Transform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# -*- coding: utf-8 -*-
-
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
-# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
+
 import logging
 
 from .base import TaskSpec
 
 logger = logging.getLogger('spiff')
 
 
@@ -47,19 +49,22 @@
         """
         assert wf_spec is not None
         assert name is not None
         TaskSpec.__init__(self, wf_spec, name, **kwargs)
         self.transforms = transforms
 
     def _update_hook(self, my_task):
+
+        super()._update_hook(my_task)
+
         if self.transforms:
             for transform in self.transforms:
                 logger.debug(f'Execute transform', extra=my_task.log_info({'transform': transform}))
                 exec(transform)
-        super(Transform, self)._update_hook(my_task)
+        return True
 
     def serialize(self, serializer):
         s_state = serializer.serialize_simple(self)
         s_state['transforms'] = self.transforms
         return s_state
 
     @classmethod
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/Trigger.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Trigger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# -*- coding: utf-8 -*-
-
-from builtins import range
 # Copyright (C) 2007 Samuel Abels
 #
-# This library is free software; you can redistribute it and/or
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from ..task import TaskState
 from .base import TaskSpec
 from ..operators import valueof
 
 
 class Trigger(TaskSpec):
 
@@ -61,38 +61,37 @@
         """
         Enqueue a trigger, such that this tasks triggers multiple times later
         when _on_complete() is called.
         """
         self.queued += 1
         # All tasks that have already completed need to be put back to
         # READY.
-        for thetask in my_task.workflow.task_tree:
-            if thetask.thread_id != my_task.thread_id:
+        for task in my_task.workflow.task_tree:
+            if task.thread_id != my_task.thread_id:
                 continue
-            if (thetask.task_spec == self and
-                    thetask._has_state(TaskState.COMPLETED)):
-                thetask._set_state(TaskState.FUTURE)
-                thetask._ready()
+            if task.task_spec == self and task._has_state(TaskState.COMPLETED):
+                task._set_state(TaskState.FUTURE)
+                task._ready()
 
-    def _on_complete_hook(self, my_task):
+    def _run_hook(self, my_task):
         """
         A hook into _on_complete() that does the task specific work.
 
         :type  my_task: Task
         :param my_task: A task in which this method is executed.
         :rtype:  bool
         :returns: True on success, False otherwise.
         """
         times = int(valueof(my_task, self.times, 1)) + self.queued
         for i in range(times):
             for task_name in self.context:
-                task = my_task.workflow.get_task_spec_from_name(task_name)
-                task._on_trigger(my_task)
+                task_spec = my_task.workflow.get_task_spec_from_name(task_name)
+                task_spec._on_trigger(my_task)
         self.queued = 0
-        TaskSpec._on_complete_hook(self, my_task)
+        return True
 
     def serialize(self, serializer):
         return serializer.serialize_trigger(self)
 
     @classmethod
     def deserialize(cls, serializer, wf_spec, s_state, **kwargs):
         """
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/specs/base.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
+
 from abc import abstractmethod
 
 from ..util.event import Event
 from ..task import TaskState
 from ..exceptions import WorkflowException
 
 
@@ -70,61 +71,49 @@
         Similarly, "defines" are spec data fields that, once defined, can
         no longer be modified.
 
         :type  wf_spec: WorkflowSpec
         :param wf_spec: A reference to the workflow specification that owns it.
         :type  name: string
         :param name: A name for the task.
-        :type  lock: list(str)
-        :param lock: A list of mutex names. The mutex is acquired
-                     on entry of execute() and released on leave of
-                     execute().
         :type  manual: bool
         :param manual: Whether this task requires a manual action to complete.
         :type  data: dict((str, object))
         :param data: name/value pairs
         :type  defines: dict((str, object))
         :param defines: name/value pairs
         :type  pre_assign: list((str, object))
         :param pre_assign: a list of name/value pairs
         :type  post_assign: list((str, object))
         :param post_assign: a list of name/value pairs
-        :type  position: dict((str, object))
-        :param position: a dict containing an 'x' and 'y' with coordinates
-                            that describe where the element occurred in the
-                            diagram.
         """
         assert wf_spec is not None
         assert name is not None
         self._wf_spec = wf_spec
-        self.id = None
         self.name = str(name)
-        self.description = kwargs.get('description', '')
+        self.description = kwargs.get('description', None)
         self.inputs = []
         self.outputs = []
         self.manual = kwargs.get('manual', False)
-        self.internal = False  # Only for easing debugging.
         self.data = kwargs.get('data', {})
         self.defines = kwargs.get('defines', {})
         self.pre_assign = kwargs.get('pre_assign',[])
         self.post_assign = kwargs.get('post_assign', [])
-        self.locks = kwargs.get('lock', [])
         self.lookahead = 2  # Maximum number of MAYBE predictions.
 
         # Events.
         self.entered_event = Event()
         self.reached_event = Event()
         self.ready_event = Event()
         self.completed_event = Event()
         self.cancelled_event = Event()
         self.finished_event = Event()
 
         self._wf_spec._add_notify(self)
         self.data.update(self.defines)
-        assert self.id is not None
 
     @property
     def spec_type(self):
         return f'{self.__class__.__module__}.{self.__class__.__name__}'
 
     def _connect_notify(self, taskspec):
         """
@@ -201,161 +190,143 @@
 
         :type  taskspec: TaskSpec
         :param taskspec: The new output task.
         """
         self.outputs.append(taskspec)
         taskspec._connect_notify(self)
 
-    def follow(self, taskspec):
-        """
-        Make this task follow the provided one. In other words, this task is
-        added to the given task outputs.
-
-        This is an alias to connect, just easier to understand when reading
-        code - ex: my_task.follow(the_other_task)
-        Adding it after being confused by .connect one times too many!
-
-        :type  taskspec: TaskSpec
-        :param taskspec: The task to follow.
-        """
-        taskspec.connect(self)
-
     def test(self):
         """
         Checks whether all required attributes are set. Throws an exception
         if an error was detected.
         """
-        # if self.id is None:
-        #    raise WorkflowException(self, 'TaskSpec is not yet instanciated.')
         if len(self.inputs) < 1:
             raise WorkflowException(self, 'No input task connected.')
 
-    def _predict(self, my_task, seen=None, looked_ahead=0):
+    def _predict(self, my_task, seen=None, looked_ahead=0, mask=TaskState.PREDICTED_MASK):
         """
         Updates the branch such that all possible future routes are added.
 
         Should NOT be overwritten! Instead, overwrite _predict_hook().
 
         :type  my_task: Task
         :param my_task: The associated task in the task tree.
         :type  seen: list[taskspec]
         :param seen: A list of already visited tasks.
         :type  looked_ahead: integer
         :param looked_ahead: The depth of the predicted path so far.
         """
-        if my_task._is_finished():
-            return
         if seen is None:
             seen = []
-        elif self in seen:
-            return
-        if not my_task._is_finished():
+
+        if my_task._has_state(mask):
             self._predict_hook(my_task)
-        if not my_task._is_definite():
-            if looked_ahead + 1 >= self.lookahead:
-                return
+
+        if my_task._is_predicted():
             seen.append(self)
+
+        look_ahead = my_task._is_definite() or looked_ahead + 1 < self.lookahead
         for child in my_task.children:
-            child.task_spec._predict(child, seen[:], looked_ahead + 1)
+            if child._has_state(mask) and child not in seen and look_ahead:
+                child.task_spec._predict(child, seen[:], looked_ahead + 1, mask)
 
     def _predict_hook(self, my_task):
-        # If the task's status is not predicted, we default to FUTURE
-        # for all it's outputs.
+        # If the task's status is definite, we default to FUTURE for all it's outputs.
         # Otherwise, copy my own state to the children.
-        if my_task._is_definite():
+        if  my_task._is_definite():
             best_state = TaskState.FUTURE
         else:
             best_state = my_task.state
-
         my_task._sync_children(self.outputs, best_state)
-        for child in my_task.children:
-            if not child._is_definite():
-                child._set_state(best_state)
 
     def _update(self, my_task):
         """
         Called whenever any event happens that may affect the
         state of this task in the workflow. For example, if a predecessor
         completes it makes sure to call this method so we can react.
         """
-        my_task._inherit_data()
-        self._update_hook(my_task)
+        if my_task._is_predicted():
+            self._predict(my_task)
+        self.entered_event.emit(my_task.workflow, my_task)
+        if self._update_hook(my_task):
+            my_task._ready()
 
     def _update_hook(self, my_task):
         """
-        Typically this method should perform the following actions::
-
-            - Update the state of the corresponding task.
-            - Update the predictions for its successors.
-
-        Returning non-False will cause the task to go into READY.
-        Returning any other value will cause no action.
+        This method should decide whether the task should run now or need to wait.
+        Tasks can also optionally choose not to inherit data.
+        Returning True will cause the task to go into READY.
         """
-        if my_task._is_predicted():
-            self._predict(my_task)
-        if not my_task.parent._is_finished():
-            return
-        self.entered_event.emit(my_task.workflow, my_task)
-        my_task._ready()
+        my_task._inherit_data()
+        return True
 
     def _on_ready(self, my_task):
         """
         Return True on success, False otherwise.
 
         :type  my_task: Task
         :param my_task: The associated task in the task tree.
         """
         assert my_task is not None
         self.test()
 
-        # Acquire locks, if any.
-        for lock in self.locks:
-            mutex = my_task.workflow._get_mutex(lock)
-            if not mutex.testandset():
-                return
-
         # Assign variables, if so requested.
         for assignment in self.pre_assign:
             assignment.assign(my_task, my_task)
 
         # Run task-specific code.
-        self._on_ready_before_hook(my_task)
-        self.reached_event.emit(my_task.workflow, my_task)
         self._on_ready_hook(my_task)
+        self.reached_event.emit(my_task.workflow, my_task)
 
-        # Run user code, if any.
-        if self.ready_event.emit(my_task.workflow, my_task):
-            # Assign variables, if so requested.
-            for assignment in self.post_assign:
-                assignment.assign(my_task, my_task)
-
-        # Release locks, if any.
-        for lock in self.locks:
-            mutex = my_task.workflow._get_mutex(lock)
-            mutex.unlock()
-
-        self.finished_event.emit(my_task.workflow, my_task)
-
-    def _on_ready_before_hook(self, my_task):
+    def _on_ready_hook(self, my_task):
         """
         A hook into _on_ready() that does the task specific work.
 
         :type  my_task: Task
         :param my_task: The associated task in the task tree.
         """
         pass
 
-    def _on_ready_hook(self, my_task):
+    def _run(self, my_task):
         """
-        A hook into _on_ready() that does the task specific work.
+        Run the task.
 
         :type  my_task: Task
         :param my_task: The associated task in the task tree.
+
+        :rtype: boolean or None
+        :returns: the value returned by the task spec's run method.
         """
-        pass
+        # I'm not sure I like setting the state here.  I'd like to handle it in `task` like
+        # the other transitions, and allow task specific error handling behavior.
+        # Having a task return a boolean indicating success (or None if it should just wait
+        # because the task is running) works well for scripts, but not for other types
+        # This is the easiest way of dealing with all other errors.
+        try:
+            result = self._run_hook(my_task)
+            # Run user code, if any.
+            if self.ready_event.emit(my_task.workflow, my_task):
+                # Assign variables, if so requested.
+                for assignment in self.post_assign:
+                    assignment.assign(my_task, my_task)
+
+            self.finished_event.emit(my_task.workflow, my_task)
+            return result
+        except Exception as exc:
+            my_task._set_state(TaskState.ERROR)
+            raise exc
+
+    def _run_hook(self, my_task):
+        """
+        A hook into _run() that does the task specific work.
+
+        :type  my_task: Task
+        :param my_task: The associated task in the task tree.
+        """
+        return True
 
     def _on_cancel(self, my_task):
         """
         May be called by another task to cancel the operation before it was
         completed.
 
         :type  my_task: Task
@@ -381,46 +352,38 @@
         overwrite _on_complete_hook() instead.
 
         :type  my_task: Task
         :param my_task: The associated task in the task tree.
         :rtype:  boolean
         :returns: True on success, False otherwise.
         """
-        assert my_task is not None
-
-        if my_task.workflow.debug:
-            print("Executing %s: %s (%s)" % (
-                my_task.task_spec.__class__.__name__,
-                my_task.get_name(), my_task.get_description()))
-
-        # We have to set the last task here, because the on_complete_hook
-        # of a loopback task may overwrite what the last_task will be.
-        my_task.workflow.last_task = my_task
         self._on_complete_hook(my_task)
+        for child in my_task.children:
+            if not child._is_finished():
+                child.task_spec._update(child)
         my_task.workflow._task_completed_notify(my_task)
-
-        if my_task.workflow.debug:
-            if hasattr(my_task.workflow, "outer_workflow"):
-                my_task.workflow.outer_workflow.task_tree.dump()
-
         self.completed_event.emit(my_task.workflow, my_task)
-        return True
 
     def _on_complete_hook(self, my_task):
         """
         A hook into _on_complete() that does the task specific work.
 
         :type  my_task: Task
         :param my_task: The associated task in the task tree.
         :rtype:  bool
         :returns: True on success, False otherwise.
         """
-        # If we have more than one output, implicitly split.
-        for child in my_task.children:
-            child.task_spec._update(child)
+        pass
+
+    def _on_error(self, my_task):
+        self._on_error_hook(my_task)
+    
+    def _on_error_hook(self, my_task):
+        """Can be overridden for task specific error handling"""
+        pass
 
     @abstractmethod
     def serialize(self, serializer, **kwargs):
         """
         Serializes the instance using the provided serializer.
 
         .. note::
@@ -436,27 +399,24 @@
         :rtype:  object
         :returns: The serialized object.
         """
         module = self.__class__.__module__
         class_name = module + '.' + self.__class__.__name__
 
         return {
-                  'id':self.id,
                   'class': class_name,
                   'name':self.name,
                   'description':self.description,
-                  'inputs':[x.id for x in self.inputs],
-                  'outputs':[x.id for x in self.outputs],
+                  'inputs':[x.name for x in self.inputs],
+                  'outputs':[x.name for x in self.outputs],
                   'manual':self.manual,
-                  'internal':self.internal,
                   'data':self.data,
                   'defines':self.defines,
                   'pre_assign':self.pre_assign,
                   'post_assign':self.post_assign,
-                  'locks':self.locks,
                   'lookahead':self.lookahead,
                   }
 
     @classmethod
     def deserialize(cls, serializer, wf_spec, s_state, **kwargs):
         """
         Deserializes the instance using the provided serializer.
@@ -474,42 +434,19 @@
         :type  s_state: object
         :param s_state: The serialized task specification object.
         :type  kwargs: dict
         :param kwargs: Passed to the serializer.
         :rtype:  TaskSpec
         :returns: The task specification instance.
         """
-        print(s_state)
-        print(wf_spec)
         out = cls(wf_spec,s_state.get('name'))
-        out.id = s_state.get('id')
         out.name = s_state.get('name')
         out.description = s_state.get('description')
         out.inputs = s_state.get('inputs')
         out.outputs = s_state.get('outputs')
         out.manual = s_state.get('manual')
-        out.internal = s_state.get('internal')
         out.data = s_state.get('data')
         out.defines = s_state.get('defines')
         out.pre_assign = s_state.get('pre_assign')
         out.post_assign = s_state.get('post_assign')
-        out.locks = s_state.get('locks')
         out.lookahead = s_state.get('lookahead')
         return out
-
-    def task_should_set_children_future(self, my_task):
-        """
-        Hook to allow a task_spec to indicate if a task should
-        set_future_children.
-
-        Subclasses can override to influence this decision.
-        """
-        return my_task.state == TaskState.COMPLETED or my_task.state == TaskState.READY
-
-    def task_will_set_children_future(self, my_task):
-        """
-        Called right before a task runs the logic for set_children_future if
-        task_should_set_children_future returns True.
-
-        Subclasses can override to perform work during that stage of execution.
-        """
-        pass
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/parser/event_parsers.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/event_parsers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,72 @@
-from SpiffWorkflow.bpmn.parser.event_parsers import EventDefinitionParser, ReceiveTaskParser
-from SpiffWorkflow.bpmn.parser.event_parsers import StartEventParser, EndEventParser, \
-    IntermediateCatchEventParser, IntermediateThrowEventParser, BoundaryEventParser, \
-    SendTaskParser
-from SpiffWorkflow.spiff.specs.events.event_definitions import MessageEventDefinition
+# Copyright (C) 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3.0 of the License, or (at your option) any later version.
+#
+# SpiffWorkflow is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
+
+from SpiffWorkflow.bpmn.parser.event_parsers import (
+    EventDefinitionParser,
+    StartEventParser,
+    EndEventParser,
+    IntermediateCatchEventParser,
+    IntermediateThrowEventParser,
+    BoundaryEventParser
+)
+from SpiffWorkflow.camunda.specs.event_definitions import MessageEventDefinition
 from SpiffWorkflow.bpmn.parser.util import one
-from SpiffWorkflow.spiff.parser.task_spec import SpiffTaskParser
 
 
-class SpiffEventDefinitionParser(SpiffTaskParser, EventDefinitionParser):
+class CamundaEventDefinitionParser(EventDefinitionParser):
 
     def parse_message_event(self, message_event):
-        """Parse a Spiff message event."""
+        """Parse a Camunda message event node."""
 
         message_ref = message_event.get('messageRef')
         if message_ref:
             message = one(self.doc_xpath('.//bpmn:message[@id="%s"]' % message_ref))
             name = message.get('name')
-            extensions = self.parse_extensions(message)
             correlations = self.get_message_correlations(message_ref)
         else:
             name = message_event.getparent().get('name')
-            extensions = {}
-            correlations = []
+            correlations = {}
 
-        return MessageEventDefinition(name, correlations, 
-            expression=extensions.get('messagePayload'),
-            message_var=extensions.get('messageVariable')
-        )
+        payload = self.attribute('expression', 'camunda', message_event)
+        result_var = self.attribute('resultVariable', 'camunda', message_event)
+        return MessageEventDefinition(name, correlations, payload, result_var)
 
 
-class SpiffStartEventParser(SpiffEventDefinitionParser, StartEventParser):
+# This really sucks, but it's still better than copy-pasting a bunch of code a million times
+# The parser "design" makes it impossible to do anything sensible of intuitive here
+
+class CamundaStartEventParser(CamundaEventDefinitionParser, StartEventParser):
     def create_task(self):
         return StartEventParser.create_task(self)
 
-class SpiffEndEventParser(SpiffEventDefinitionParser, EndEventParser):
+class CamundaEndEventParser(CamundaEventDefinitionParser, EndEventParser):
     def create_task(self):
         return EndEventParser.create_task(self)
 
-class SpiffIntermediateCatchEventParser(SpiffEventDefinitionParser, IntermediateCatchEventParser):
+class CamundaIntermediateCatchEventParser(CamundaEventDefinitionParser, IntermediateCatchEventParser):
     def create_task(self):
         return IntermediateCatchEventParser.create_task(self)
 
-class SpiffIntermediateThrowEventParser(SpiffEventDefinitionParser, IntermediateThrowEventParser):
+class CamundaIntermediateThrowEventParser(CamundaEventDefinitionParser, IntermediateThrowEventParser):
     def create_task(self):
         return IntermediateThrowEventParser.create_task(self)
 
-class SpiffBoundaryEventParser(SpiffEventDefinitionParser, BoundaryEventParser):
+class CamundaBoundaryEventParser(CamundaEventDefinitionParser, BoundaryEventParser):
     def create_task(self):
         return BoundaryEventParser.create_task(self)
-
-class SpiffSendTaskParser(SpiffEventDefinitionParser, SendTaskParser):
-    def create_task(self):
-        return SendTaskParser.create_task(self)
-
-class SpiffReceiveTaskParser(SpiffEventDefinitionParser, ReceiveTaskParser):
-    def create_task(self):
-        return ReceiveTaskParser.create_task(self)
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/spiff/parser/task_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/task_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,62 @@
+# Copyright (C) 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3.0 of the License, or (at your option) any later version.
+#
+# SpiffWorkflow is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
+
 from lxml import etree
 
-from SpiffWorkflow.dmn.specs.BusinessRuleTask import BusinessRuleTask
 from SpiffWorkflow.bpmn.parser.TaskParser import TaskParser
 from SpiffWorkflow.bpmn.parser.task_parsers import SubprocessParser
 from SpiffWorkflow.bpmn.parser.util import xpath_eval
 
+from SpiffWorkflow.spiff.specs.defaults import (
+    StandardLoopTask,
+    ParallelMultiInstanceTask,
+    SequentialMultiInstanceTask,
+    BusinessRuleTask
+)
+
 SPIFFWORKFLOW_MODEL_NS = 'http://spiffworkflow.org/bpmn/schema/1.0/core'
 SPIFFWORKFLOW_MODEL_PREFIX = 'spiffworkflow'
 
 
 class SpiffTaskParser(TaskParser):
 
+    STANDARD_LOOP_CLASS = StandardLoopTask
+    PARALLEL_MI_CLASS = ParallelMultiInstanceTask
+    SEQUENTIAL_MI_CLASS = SequentialMultiInstanceTask
+
     def parse_extensions(self, node=None):
         if node is None:
             node = self.node
         return SpiffTaskParser._parse_extensions(node)
 
     @staticmethod
     def _parse_extensions(node):
         # Too bad doing this works in such a stupid way.
         # We should set a namespace and automatically do this.
         extensions = {}
         extra_ns = {SPIFFWORKFLOW_MODEL_PREFIX: SPIFFWORKFLOW_MODEL_NS}
         xpath = xpath_eval(node, extra_ns)
-        extension_nodes = xpath(f'.//bpmn:extensionElements/{SPIFFWORKFLOW_MODEL_PREFIX}:*')
+        extension_nodes = xpath(f'./bpmn:extensionElements/{SPIFFWORKFLOW_MODEL_PREFIX}:*')
         for node in extension_nodes:
             name = etree.QName(node).localname
             if name == 'properties':
                 extensions['properties'] = SpiffTaskParser._parse_properties(node)
             elif name == 'unitTests':
                 extensions['unitTests'] = SpiffTaskParser._parse_script_unit_tests(node)
             elif name == 'serviceTaskOperator':
@@ -77,91 +106,102 @@
                 parameters[param_node.attrib['id']] = {
                     'value': param_node.attrib['value'],
                     'type': param_node.attrib['type']
                 }
         operator['parameters'] = parameters
         return operator
 
+    def _copy_task_attrs(self, original):
+        # I am so disappointed I have to do this.
+        super()._copy_task_attrs(original)
+        self.task.prescript = original.prescript
+        self.task.postscript = original.postscript
+        original.prescript = None
+        original.postscript = None
+
     def create_task(self):
         # The main task parser already calls this, and even sets an attribute, but
         # 1. It calls it after creating the task so I don't have access to it here yet and
         # 2. I want defined attributes, not a dict of random crap
         # (though the dict of random crap will still be there since the base parser adds it).
         extensions = self.parse_extensions()
         prescript = extensions.get('preScript')
         postscript = extensions.get('postScript')
-        return self.spec_class(self.spec, self.get_task_spec_name(),
-                               lane=self.lane,
-                               description=self.node.get('name', None),
-                               position=self.position,
-                               prescript=prescript,
-                               postscript=postscript)
+        return self.spec_class(self.spec, self.bpmn_id, prescript=prescript, postscript=postscript, **self.bpmn_attributes)
 
 
 class SubWorkflowParser(SpiffTaskParser):
 
     def create_task(self):
         extensions = self.parse_extensions()
         prescript = extensions.get('preScript')
         postscript = extensions.get('postScript')
         subworkflow_spec = SubprocessParser.get_subprocess_spec(self)
         return self.spec_class(
-            self.spec, self.get_task_spec_name(), subworkflow_spec,
-            lane=self.lane, position=self.position,
-            description=self.node.get('name', None),
+            self.spec, 
+            self.bpmn_id,
+            subworkflow_spec=subworkflow_spec,
             prescript=prescript,
-            postscript=postscript)
+            postscript=postscript,
+            **self.bpmn_attributes)
 
 
 class ScriptTaskParser(SpiffTaskParser):
     def create_task(self):
         script = None
         for child_node in self.node:
             if child_node.tag.endswith('script'):
                 script = child_node.text
-        return self.spec_class(
-            self.spec, self.get_task_spec_name(), script,
-            lane=self.lane, position=self.position,
-            description=self.node.get('name', None))
+        return self.spec_class(self.spec, self.bpmn_id, script, **self.bpmn_attributes)
 
 
 class CallActivityParser(SpiffTaskParser):
 
     def create_task(self):
         extensions = self.parse_extensions()
         prescript = extensions.get('preScript')
         postscript = extensions.get('postScript')
         subworkflow_spec = SubprocessParser.get_call_activity_spec(self)
         return self.spec_class(
-            self.spec, self.get_task_spec_name(), subworkflow_spec,
-            lane=self.lane, position=self.position,
-            description=self.node.get('name', None),
+            self.spec, 
+            self.bpmn_id,
+            subworkflow_spec=subworkflow_spec,
             prescript=prescript,
-            postscript=postscript)
+            postscript=postscript,
+            **self.bpmn_attributes)
 
 class ServiceTaskParser(SpiffTaskParser):
     def create_task(self):
         extensions = self.parse_extensions()
         operator = extensions.get('serviceTaskOperator')
+        prescript = extensions.get('preScript')
+        postscript = extensions.get('postScript')
         return self.spec_class(
-                self.spec, self.get_task_spec_name(),
-                operator['name'], operator['parameters'],
-                operator['resultVariable'],
-                description=self.node.get('name', None),
-                lane=self.lane, position=self.position)
+                self.spec,
+                self.bpmn_id,
+                operation_name=operator['name'], 
+                operation_params=operator['parameters'],
+                result_variable=operator['resultVariable'],
+                prescript=prescript,
+                postscript=postscript,
+                **self.bpmn_attributes)
 
 class BusinessRuleTaskParser(SpiffTaskParser):
 
     def create_task(self):
         decision_ref = self.get_decision_ref(self.node)
-        return BusinessRuleTask(self.spec,
-                                self.get_task_spec_name(),
-                                dmnEngine=self.process_parser.parser.get_engine(decision_ref, self.node),
-                                lane=self.lane,
-                                position=self.position,
-                                description=self.node.get('name', None)
-                                )
+        extensions = self.parse_extensions()
+        prescript = extensions.get('preScript')
+        postscript = extensions.get('postScript')
+        return BusinessRuleTask(
+            self.spec,
+            self.bpmn_id,
+            dmnEngine=self.process_parser.parser.get_engine(decision_ref, self.node),
+            prescript=prescript,
+            postscript=postscript,
+            **self.bpmn_attributes,
+        )
 
     @staticmethod
     def get_decision_ref(node):
         extensions = SpiffTaskParser._parse_extensions(node)
         return extensions.get('calledDecisionId')
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/task.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,41 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
-import copy
+from copy import deepcopy
+
 import logging
 import time
 import warnings
 from uuid import uuid4
 
 from .util.deep_merge import DeepMerge
 from .exceptions import WorkflowException
 
 logger = logging.getLogger('spiff')
 metrics = logging.getLogger('spiff.metrics')
 data_log = logging.getLogger('spiff.data')
 
 
-def updateDotDict(dct,dotted_path,value):
-    parts = dotted_path.split(".")
-    path_len = len(parts)
-    root = dct
-    for i, key in enumerate(parts):
-        if (i + 1) < path_len:
-            if key not in dct:
-                dct[key] = {}
-            dct = dct[key]
-        else:
-            dct[key] = value
-    return root
-
-
 class TaskState:
     """
 
     The following states may exist:
 
     - FUTURE: The task will definitely be reached in the future,
       regardless of which choices the user makes within the workflow.
@@ -76,65 +63,52 @@
     - COMPLETED: The task was regularily completed.
 
     Note that the LIKELY and MAYBE tasks are merely predicted/guessed, so
     those tasks may be removed from the tree at runtime later. They are
     created to allow for visualizing the workflow at a time where
     the required decisions have not yet been made.
     """
-    # Note: The states in this list are ordered in the sequence in which
-    # they may appear. Do not change.
     MAYBE = 1
     LIKELY = 2
     FUTURE = 4
     WAITING = 8
     READY = 16
-    COMPLETED = 32
-    CANCELLED = 64
-
-    FINISHED_MASK = CANCELLED | COMPLETED
-    DEFINITE_MASK = FUTURE | WAITING | READY | FINISHED_MASK
-    PREDICTED_MASK = FUTURE | LIKELY | MAYBE
-    NOT_FINISHED_MASK = PREDICTED_MASK | WAITING | READY
+    STARTED = 32
+    COMPLETED = 64
+    ERROR = 128
+    CANCELLED = 256
+
+    FINISHED_MASK = CANCELLED | ERROR | COMPLETED
+    DEFINITE_MASK = FUTURE | WAITING | READY | STARTED
+    PREDICTED_MASK = LIKELY | MAYBE
+    NOT_FINISHED_MASK = PREDICTED_MASK | DEFINITE_MASK
     ANY_MASK = FINISHED_MASK | NOT_FINISHED_MASK
 
 
-TaskStateNames = {TaskState.FUTURE: 'FUTURE',
-                  TaskState.WAITING: 'WAITING',
-                  TaskState.READY: 'READY',
-                  TaskState.CANCELLED: 'CANCELLED',
-                  TaskState.COMPLETED: 'COMPLETED',
-                  TaskState.LIKELY: 'LIKELY',
-                  TaskState.MAYBE: 'MAYBE'}
+TaskStateNames = {
+    TaskState.FUTURE: 'FUTURE',
+    TaskState.WAITING: 'WAITING',
+    TaskState.READY: 'READY',
+    TaskState.STARTED: 'STARTED',
+    TaskState.CANCELLED: 'CANCELLED',
+    TaskState.COMPLETED: 'COMPLETED',
+    TaskState.ERROR: 'ERROR',
+    TaskState.LIKELY: 'LIKELY',
+    TaskState.MAYBE: 'MAYBE'
+}
 TaskStateMasks = {
-                  TaskState.FINISHED_MASK: 'FINISHED_MASK',
-                  TaskState.DEFINITE_MASK: 'DEFINITE_MASK',
-                  TaskState.PREDICTED_MASK: 'PREDICTED_MASK',
-                  TaskState.NOT_FINISHED_MASK: 'NOT_FINISHED_MASK',
-                  TaskState.ANY_MASK: 'ANY_MASK',
-                  }
+    TaskState.FINISHED_MASK: 'FINISHED_MASK',
+    TaskState.DEFINITE_MASK: 'DEFINITE_MASK',
+    TaskState.PREDICTED_MASK: 'PREDICTED_MASK',
+    TaskState.NOT_FINISHED_MASK: 'NOT_FINISHED_MASK',
+    TaskState.ANY_MASK: 'ANY_MASK',
+}
 
 
-class DeprecatedMetaTask(type):
-    """
-    Handle deprecated methods that are now moved to TaskState
-    """
-    TaskNames = {**TaskStateNames, **TaskStateMasks}
-    TaskStateFromNames = {v: k for k, v in TaskNames.items()}
-
-    def __getattribute__(self, item):
-        if item in DeprecatedMetaTask.TaskNames.values():
-            warnings.warn(f'Task.{item} is deprecated.  '
-                          f'Please use TaskState.{item}',
-                          DeprecationWarning, stacklevel=2)
-            return DeprecatedMetaTask.TaskStateFromNames[item]
-        else:
-            return type.__getattribute__(self, item)
-
-
-class Task(object,  metaclass=DeprecatedMetaTask):
+class Task(object):
     """
     Used internally for composing a tree that represents the path that
     is taken (or predicted) within the workflow.
 
     Each Task has a state. For an explanation, consider the following task
     specification::
 
@@ -178,16 +152,15 @@
                 raise StopIteration()
 
             current = self.path[-1]
 
             # Assure we don't recurse forever.
             self.count += 1
             if self.count > self.MAX_ITERATIONS:
-                raise WorkflowException(current,
-                "Task Iterator entered infinite recursion loop" )
+                raise WorkflowException("Task Iterator entered infinite recursion loop", task_spec=current)
 
 
             # If the current task has children, the first child is the next
             # item. If the current task is LIKELY, and predicted tasks are not
             # specificly searched, we can ignore the children, because
             # predicted tasks should only have predicted children.
             ignore_task = False
@@ -244,178 +217,76 @@
         self.children = []
         self._state = state
         self.triggered = False
         self.task_spec = task_spec
         self.id = uuid4()
         self.thread_id = self.__class__.thread_id_pool
         self.data = {}
-        self.terminate_current_loop = False
         self.internal_data = {}
-        self.mi_collect_data = {}
+        self.last_state_change = time.time()
         if parent is not None:
             self.parent._child_added_notify(self)
 
-        # TODO: get rid of this stuff
-        self.last_state_change = time.time()
-        self.state_history = [state]
-
     @property
     def state(self):
         return self._state
 
     @state.setter
     def state(self, value):
         if value < self._state:
             raise WorkflowException(
-                self.task_spec,
-                'state went from %s to %s!' % (self.get_state_name(), TaskStateNames[value])
+                'state went from %s to %s!' % (self.get_state_name(), TaskStateNames[value]),
+                task_spec=self.task_spec
             )
         self._set_state(value)
 
     def _set_state(self, value):
         """Using the setter method will raise an error on a "backwards" state change.
         Call this method directly to force the state change.
         """
         if value != self.state:
             logger.info(f'State change to {TaskStateNames[value]}', extra=self.log_info())
             self.last_state_change = time.time()
-            self.state_history.append(value)
             self._state = value
         else:
             logger.debug(f'State set to {TaskStateNames[value]}', extra=self.log_info())
 
     def __repr__(self):
         return '<Task object (%s) in state %s at %s>' % (
             self.task_spec.name,
             self.get_state_name(),
             hex(id(self)))
 
     def log_info(self, dct=None):
         extra = dct or {}
         extra.update({
-            'workflow': self.workflow.spec.name,
+            'workflow_spec': self.workflow.spec.name,
+            'workflow_name': self.workflow.spec.description,
             'task_spec': self.task_spec.name,
             'task_name': self.task_spec.description,
             'task_id': self.id,
             'task_type': self.task_spec.spec_type,
             'data': self.data if logger.level < 20 else None,
             'internal_data': self.internal_data if logger.level <= 10 else None,
         })
         return extra
 
-    def update_data_var(self, fieldid, value):
-        model = {}
-        updateDotDict(model,fieldid, value)
-        self.update_data(model)
-
     def update_data(self, data):
         """
         If the task.data needs to be updated from a UserTask form or
         a Script task then use this function rather than updating task.data
         directly.  It will handle deeper merges of data,
         and MultiInstance tasks will be updated correctly.
         """
         self.data = DeepMerge.merge(self.data, data)
         data_log.info('Data update', extra=self.log_info())
 
-    def task_info(self):
-        """
-        Returns a dictionary of information about the current task, so that
-        we can give hints to the user about what kind of task we are working
-        with such as a looping task or a Parallel MultiInstance task
-        :returns: dictionary
-        """
-        default = {'is_looping': False,
-                   'is_sequential_mi': False,
-                   'is_parallel_mi': False,
-                   'mi_count': 0,
-                   'mi_index': 0}
-
-        miInfo = getattr(self.task_spec, "multiinstance_info", None)
-        if callable(miInfo):
-            return miInfo(self)
-        else:
-            return default
-
-    def terminate_loop(self):
-        """
-        Used in the case that we are working with a BPMN 'loop' task.
-        The task will loop, repeatedly asking for input until terminate_loop
-        is called on the task
-        """
-        if self.is_looping():
-            self.terminate_current_loop = True
-        else:
-            raise WorkflowException(self.task_spec,
-                                    'The method terminate_loop should only be called in the case of a BPMN Loop Task')
-
-    def is_looping(self):
-        """Returns true if this is a looping task."""
-        islooping = getattr(self.task_spec, "is_loop_task", None)
-        if callable(islooping):
-            return self.task_spec.is_loop_task()
-        else:
-            return False
-
-    def set_children_future(self):
-        """
-        for a parallel gateway, we need to set up our
-        children so that the gateway figures out that it needs to join up
-        the inputs - otherwise our child process never gets marked as
-        'READY'
-        """
-
-        if not self.task_spec.task_should_set_children_future(self):
-            return
-
-        self.task_spec.task_will_set_children_future(self)
-
-        # now we set this one to execute
-
-        self._set_state(TaskState.MAYBE)
-        self._sync_children(self.task_spec.outputs)
-        for child in self.children:
-            child.set_children_future()
-
-    def find_children_by_name(self,name):
-        """
-        for debugging
-        """
-        return [x for x in self.workflow.task_tree if x.task_spec.name == name]
-
-    def reset_token(self, data, reset_data=False):
-        """
-        Resets the token to this task. This should allow a trip 'back in time'
-        as it were to items that have already been completed.
-        :type  reset_data: bool
-        :param reset_data: Do we want to have the data be where we left of in
-                           this task or not
-        """
-        self.internal_data = {}
-        if not reset_data and self.workflow.last_task and self.workflow.last_task.data:
-            # This is a little sly, the data that will get inherited should
-            # be from the last completed task, but we don't want to alter
-            # the tree, so we just set the parent's data to the given data.
-            self.parent.data = copy.deepcopy(data)
-        self.workflow.last_task = self.parent
-        self.set_children_future()  # this method actually fixes the problem
-        self._set_state(TaskState.FUTURE)
-        self.task_spec._update(self)
-
     def __iter__(self):
         return Task.Iterator(self)
 
-    def __setstate__(self, dict):
-        self.__dict__.update(dict)
-        # If unpickled in the same Python process in which a workflow
-        # (Task) is built through the API, we need to make sure
-        # that there will not be any ID collisions.
-        if dict['thread_id'] >= self.__class__.thread_id_pool:
-            self.__class__.thread_id_pool = dict['thread_id']
-
     def _get_root(self):
         """
         Returns the top level parent.
         """
         if self.parent is None:
             return self
         return self.parent._get_root()
@@ -442,143 +313,122 @@
                 drop.append(child)
             else:
                 child._drop_children()
         for task in drop:
             self.children.remove(task)
 
     def _has_state(self, state):
-        """
-        Returns True if the Task has the given state flag set.
-        """
+        """Returns True if the Task has the given state flag set."""
         return (self.state & state) != 0
 
     def _is_finished(self):
         return self._has_state(TaskState.FINISHED_MASK)
 
     def _is_predicted(self):
         return self._has_state(TaskState.PREDICTED_MASK)
 
     def _is_definite(self):
         return self._has_state(TaskState.DEFINITE_MASK)
 
+    def reset_token(self, data):
+        """
+        Reset the workflow to this task,
+        :param data: set the task data (if None, inherit from parent task)
+        """
+        self.internal_data = {}
+        if data is None:
+            self.data = deepcopy(self.parent.data)
+        descendants = [t for t in self]
+        self._drop_children(force=True)
+        self._set_state(TaskState.FUTURE)
+        self.task_spec._predict(self, mask=TaskState.PREDICTED_MASK|TaskState.FUTURE)
+        self.task_spec._update(self)
+        return descendants[1:] if len(descendants) > 1 else []
+
     def _add_child(self, task_spec, state=TaskState.MAYBE):
         """
         Adds a new child and assigns the given TaskSpec to it.
 
         :type  task_spec: TaskSpec
         :param task_spec: The task spec that is assigned to the new child.
         :type  state: integer
         :param state: The bitmask of states for the new child.
         :rtype:  Task
         :returns: The new child task.
         """
-        if task_spec is None:
-            raise ValueError(self, '_add_child() requires a TaskSpec')
         if self._is_predicted() and state & TaskState.PREDICTED_MASK == 0:
-            msg = 'Attempt to add non-predicted child to predicted task'
-            raise WorkflowException(self.task_spec, msg)
+            raise WorkflowException('Attempt to add non-predicted child to predicted task', task_spec=self.task_spec)
         task = Task(self.workflow, task_spec, self, state=state)
         task.thread_id = self.thread_id
         if state == TaskState.READY:
             task._ready()
         return task
 
-    def _assign_new_thread_id(self, recursive=True):
-        """
-        Assigns a new thread id to the task.
-
-        :type  recursive: bool
-        :param recursive: Whether to assign the id to children recursively.
-        :rtype:  bool
-        :returns: The new thread id.
-        """
-        self.__class__.thread_id_pool += 1
-        self.thread_id = self.__class__.thread_id_pool
-        if not recursive:
-            return self.thread_id
-        for child in self:
-            child.thread_id = self.thread_id
-        return self.thread_id
-
     def _sync_children(self, task_specs, state=TaskState.MAYBE):
         """
         This method syncs up the task's children with the given list of task
         specs. In other words::
 
             - Add one child for each given TaskSpec, unless that child already
               exists.
             - Remove all children for which there is no spec in the given list,
               unless it is a "triggered" task.
-            - Handle looping back to previous tasks, so we don't end up with
-              an infinitely large tree.
         .. note::
 
            It is an error if the task has a non-predicted child that is
            not given in the TaskSpecs.
 
         :type  task_specs: list(TaskSpec)
         :param task_specs: The list of task specs that may become children.
         :type  state: integer
         :param state: The bitmask of states for the new children.
         """
         if task_specs is None:
             raise ValueError('"task_specs" argument is None')
-        add = task_specs[:]
-
-        # If a child task_spec is also an ancestor, we are looping back,
-        # replace those specs with a loopReset task.
-        root_task = self._get_root()
-        for index, task_spec in enumerate(add):
-            ancestor_task = self._find_ancestor(task_spec)
-            if ancestor_task and ancestor_task != root_task:
-                destination = ancestor_task
-                new_spec = self.workflow.get_reset_task_spec(destination)
-                new_spec.outputs = []
-                new_spec.inputs = task_spec.inputs
-                add[index] = new_spec
+        new_children = task_specs[:]
 
         # Create a list of all children that are no longer needed.
-        remove = []
+        unneeded_children = []
         for child in self.children:
-            # Triggered tasks are never removed.
             if child.triggered:
-                continue
-
-            # Check whether the task needs to be removed.
-            if child.task_spec in add:
-                add.remove(child.task_spec)
-                continue
-
-            # Non-predicted tasks must not be removed, so they HAVE to be in
-            # the given task spec list.
-            if child._is_definite():
-                raise WorkflowException(self.task_spec,
-                                        'removal of non-predicted child %s' %
-                                        repr(child))
-            remove.append(child)
-
-
+                # Triggered tasks are never removed.
+                pass
+            elif child.task_spec in new_children:
+                # If the task already exists, remove it from to-be-added and update its state
+                new_children.remove(child.task_spec)
+                if not child._is_finished():
+                    child._set_state(state)
+            else:
+                if child._is_definite():
+                    # Definite tasks must not be removed, so they HAVE to be in the given task spec list.
+                    raise WorkflowException(f'removal of non-predicted child {child}', task_spec=self.task_spec)
+                unneeded_children.append(child)
 
-        # Remove and add the children accordingly.
-        for child in remove:
+        # Update children accordingly
+        for child in unneeded_children:
             self.children.remove(child)
-        for task_spec in add:
+        for task_spec in new_children:
             self._add_child(task_spec, state)
 
-    def _set_likely_task(self, task_specs):
-        if not isinstance(task_specs, list):
-            task_specs = [task_specs]
-        for task_spec in task_specs:
-            for child in self.children:
-                if child.task_spec != task_spec:
-                    continue
-                if child._is_definite():
-                    continue
-                child._set_state(TaskState.LIKELY)
-                return
+    def _assign_new_thread_id(self, recursive=True):
+        """
+        Assigns a new thread id to the task.
+
+        :type  recursive: bool
+        :param recursive: Whether to assign the id to children recursively.
+        :rtype:  bool
+        :returns: The new thread id.
+        """
+        self.__class__.thread_id_pool += 1
+        self.thread_id = self.__class__.thread_id_pool
+        if not recursive:
+            return self.thread_id
+        for child in self:
+            child.thread_id = self.thread_id
+        return self.thread_id
 
     def _is_descendant_of(self, parent):
         """
         Returns True if parent is in the list of ancestors, returns False
         otherwise.
 
         :type  parent: Task
@@ -655,44 +505,25 @@
         """
         if self.parent is None:
             return None
         if self.parent.get_name() == name:
             return self.parent
         return self.parent._find_ancestor_from_name(name)
 
-    def _ready(self):
-        """
-        Marks the task as ready for execution.
-        """
-        if self._has_state(TaskState.COMPLETED) or self._has_state(TaskState.CANCELLED):
-            return
-        self._set_state(TaskState.READY)
-        self.task_spec._on_ready(self)
-
     def get_name(self):
         return str(self.task_spec.name)
 
     def get_description(self):
         return str(self.task_spec.description)
 
-    def get_state(self):
-        """
-        Returns this Task's state.
-        """
-        return self.state
-
     def get_state_name(self):
-        """
-        Returns a textual representation of this Task's state.
-        """
-        state_name = []
+        """Returns a textual representation of this Task's state."""
         for state, name in list(TaskStateNames.items()):
             if self._has_state(state):
-                state_name.append(name)
-        return '|'.join(state_name)
+                return name
 
     def get_spec_data(self, name=None, default=None):
         """
         Returns the value of the spec data with the given name, or the given
         default value if the spec data does not exist.
 
         :type  name: str
@@ -714,15 +545,14 @@
         return self.internal_data.get(name, default)
 
     def set_data(self, **kwargs):
         """
         Defines the given attribute/value pairs.
         """
         self.data.update(kwargs)
-        data_log.info('Set data', extra=self.log_info())
 
     def _inherit_data(self):
         """
         Inherits the data from the parent.
         """
         self.set_data(**self.parent.data)
 
@@ -736,46 +566,77 @@
         :type  default: obj
         :param default: Return this value if the data field does not exist.
         :rtype:  obj
         :returns: The value of the data field
         """
         return self.data.get(name, default)
 
-    def cancel(self):
-        """
-        Cancels the item if it was not yet completed, and removes
-        any children that are LIKELY.
-        """
-        if self._is_finished():
-            for child in self.children:
-                child.cancel()
+    def _ready(self):
+        """Marks the task as ready for execution."""
+        if self._has_state(TaskState.COMPLETED) or self._has_state(TaskState.CANCELLED):
             return
-        self._set_state(TaskState.CANCELLED)
-        self._drop_children()
-        self.task_spec._on_cancel(self)
+        self._set_state(TaskState.READY)
+        self.task_spec._on_ready(self)
 
-    def complete(self):
+    def run(self):
         """
-        Called by the associated task to let us know that its state
-        has changed (e.g. from FUTURE to COMPLETED.)
+        Execute the task.
+
+        If the return value of task_spec._run is None, assume the task is not finished,
+        and move the task to WAITING.
+
+        :rtype: boolean or None
+        :returns: the value returned by the task spec's run method
         """
-        self._set_state(TaskState.COMPLETED)
-        # WHY on earth do we mark the task completed and THEN attempt to execute it.
-        # A sane model would have success and failure states and instead we return
-        # a boolean, with no systematic way of dealing with failures.  This is just
-        # crazy!
         start = time.time()
-        retval = self.task_spec._on_complete(self)
+        retval = self.task_spec._run(self)
         extra = self.log_info({
             'action': 'Complete',
             'elapsed': time.time() - start
         })
         metrics.debug('', extra=extra)
+        if retval is None:
+            # This state is intended to indicate a task that is not finished, but will continue
+            # in the background without blocking other unrelated tasks (ie on other branches).
+            # It is a distinct state from "waiting" so that `update` does not have to distinguish
+            # between tasks that can be started and tasks that have already been started.
+            # Spiff can manage deciding if a task can run, but if a task is set to "started", it will
+            # have to be tracked independently of the workflow and completed manually when it finishes
+            # for the time being (probably I'll add polling methods in the future, but I'm not exactly
+            # sure how they should work).
+            # I'm adding this state now because I'm adding an error state (which I think there is a
+            # need for) and don't want to go through the hassle of updating serialization of task states
+            # twice; doing this at all is going to be painful enough.
+            self._set_state(TaskState.STARTED)
+        elif retval is False:
+            self.error()
+        else:
+            self.complete()
         return retval
 
+    def cancel(self):
+        """Cancels the item if it was not yet completed, and removes any children that are LIKELY."""
+        if self._is_finished():
+            for child in self.children:
+                child.cancel()
+        else:
+            self._set_state(TaskState.CANCELLED)
+            self._drop_children()
+            self.task_spec._on_cancel(self)
+
+    def complete(self):
+        """Marks this task complete."""
+        self._set_state(TaskState.COMPLETED)
+        self.task_spec._on_complete(self)
+        self.workflow.last_task = self
+
+    def error(self):
+        self._set_state(TaskState.ERROR)
+        self.task_spec._on_error(self)
+
     def trigger(self, *args):
         """
         If recursive is True, the state is applied to the tree recursively.
         """
         self.task_spec._on_trigger(self, *args)
 
     def get_dump(self, indent=0, recursive=True):
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/util/event.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# -*- coding: utf-8 -*-
-
-from builtins import object
+# Copyright (C) 2007-2010 Samuel Abels.
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3.0 of the License, or (at your option) any later version.
+#
+# SpiffWorkflow is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
 #
 # DO NOT EDIT THIS FILE.
 # THIS CODE IS TAKE FROM Exscript.util:
 #   https://github.com/knipknap/exscript/tree/master/src/Exscript/util
 #
 
-# Copyright (C) 2007-2010 Samuel Abels.
-#
-# This program is free software; you can redistribute it and/or modify
-# it under the terms of the GNU General Public License version 2, as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 """
 A simple signal/event mechanism.
 """
 from threading import Lock
 from . import weakmethod
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/util/impl.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/bpmn_spec_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-# -*- coding: utf-8 -*-
-
-# This library is free software; you can redistribute it and/or
+# Copyright (C) 2012 Matthew Hampton, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
-import sys
 
+from ..bpmn_task_spec import BpmnTaskSpec
+
+
+class BpmnSpecMixin(BpmnTaskSpec):
 
-def get_class(full_class_name):
-    parts = full_class_name.rsplit('.', 1)
-    module_name = parts[0]
-    class_name = parts[1]
-    __import__(module_name)
-    return getattr(sys.modules[module_name], class_name)
+    def __init__(self, wf_spec, bpmn_id, **kwargs):
+        super().__init__(wf_spec, bpmn_id, **kwargs)
+        self.bpmn_id = bpmn_id
+        self.bpmn_name = kwargs.get('bpmn_name')
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/util/weakmethod.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/weakmethod.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-# -*- coding: utf-8 -*-
+# Copyright (C) 2007-2010 Samuel Abels.
+#
+# This file is part of SpiffWorkflow.
+#
+# SpiffWorkflow is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3.0 of the License, or (at your option) any later version.
+#
+# SpiffWorkflow is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
+# 02110-1301  USA
 
-from builtins import object
 #
 # DO NOT EDIT THIS FILE.
 # THIS CODE IS TAKE FROM Exscript.util:
 #   https://github.com/knipknap/exscript/tree/master/src/Exscript/util
 #
 
-# Copyright (C) 2007-2010 Samuel Abels.
-#
-# This program is free software; you can redistribute it and/or modify
-# it under the terms of the GNU General Public License version 2, as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 """
 Weak references to bound and unbound methods.
 """
 import weakref
 
 
 class DeadMethodCalled(Exception):
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow/workflow.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2007 Samuel Abels
+# Copyright (C) 2007 Samuel Abels, 2023 Sartography
+#
+# This file is part of SpiffWorkflow.
 #
-# This library is free software; you can redistribute it and/or
+# SpiffWorkflow is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
+# version 3.0 of the License, or (at your option) any later version.
 #
-# This library is distributed in the hope that it will be useful,
+# SpiffWorkflow is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301  USA
 
 import logging
 
-from . import specs
-from .specs.LoopResetTask import LoopResetTask
+from .specs.Simple import Simple
 from .task import Task, TaskState
 from .util.compat import mutex
 from .util.event import Event
-from .exceptions import WorkflowException
+from .exceptions import TaskNotFoundException, WorkflowException
 
 logger = logging.getLogger('spiff')
 
+
 class Workflow(object):
 
     """
     The engine that executes a workflow.
     It is a essentially a facility for managing all branches.
     A Workflow is also the place that holds the data of a running workflow.
     """
@@ -50,44 +50,41 @@
         self.name = None
         assert workflow_spec is not None
         self.spec = workflow_spec
         self.data = {}
         self.outer_workflow = kwargs.get('parent', self)
         self.locks = {}
         self.last_task = None
-        if deserializing:
-            assert 'Root' in workflow_spec.task_specs
-            root = workflow_spec.task_specs['Root']  # Probably deserialized
+        if 'Root' in workflow_spec.task_specs:
+            root = workflow_spec.task_specs['Root']
         else:
-            if 'Root' in workflow_spec.task_specs:
-                root = workflow_spec.task_specs['Root']
-            else:
-                root = specs.Simple(workflow_spec, 'Root')
-            logger.info('Initialize', extra=self.log_info())
+            root = Simple(workflow_spec, 'Root')
 
         # Setting TaskState.COMPLETED prevents the root task from being executed.
         self.task_tree = Task(self, root, state=TaskState.COMPLETED)
+        start = self.task_tree._add_child(self.spec.start, state=TaskState.FUTURE)
         self.success = True
         self.debug = False
 
         # Events.
         self.completed_event = Event()
 
-        start = self.task_tree._add_child(self.spec.start, state=TaskState.FUTURE)
-
-        self.spec.start._predict(start)
-        if 'parent' not in kwargs:
-            start.task_spec._update(start)
+        if not deserializing:
+            self._predict()
+            if 'parent' not in kwargs:
+                start.task_spec._update(start)
+            logger.info('Initialize', extra=self.log_info())
 
         self.task_mapping = self._get_task_mapping()
 
     def log_info(self, dct=None):
         extra = dct or {}
         extra.update({
-            'workflow': self.spec.name,
+            'workflow_spec': self.spec.name,
+            'workflow_name': self.spec.description,
             'task_spec': '-',
             'task_type': None,
             'task_id': None,
             'data': None,
         })
         return extra
 
@@ -103,14 +100,18 @@
         try:
             nexttask = next(iter)
         except StopIteration:
             # No waiting tasks found.
             return True
         return False
 
+    def _predict(self, mask=TaskState.NOT_FINISHED_MASK):
+        for task in Workflow.get_tasks(self,TaskState.NOT_FINISHED_MASK):
+            task.task_spec._predict(task, mask=mask)
+
     def _get_waiting_tasks(self):
         waiting = Task.Iterator(self.task_tree, TaskState.WAITING)
         return [w for w in waiting]
 
     def _task_completed_notify(self, task):
         if task.get_name() == 'End':
             self.data.update(task.data)
@@ -167,151 +168,112 @@
         return self.data.get(name, default)
 
     def cancel(self, success=False):
         """
         Cancels all open tasks in the workflow.
 
         :type  success: bool
-        :param success: Whether the Workflow should be marked as successfully
-                        completed.
+        :param success: Whether the Workflow should be marked as successfully completed.
         """
         self.success = success
         cancel = []
-        mask = TaskState.NOT_FINISHED_MASK
-        for task in Task.Iterator(self.task_tree, mask):
+        for task in Task.Iterator(self.task_tree, TaskState.NOT_FINISHED_MASK):
             cancel.append(task)
         for task in cancel:
             task.cancel()
         logger.info(f'Cancel with {len(cancel)} remaining', extra=self.log_info())
+        return cancel
 
     def get_task_spec_from_name(self, name):
         """
         Returns the task spec with the given name.
 
         :type  name: str
         :param name: The name of the task.
         :rtype:  TaskSpec
         :returns: The task spec with the given name.
         """
         return self.spec.get_task_spec_from_name(name)
 
-    def get_task(self, id,tasklist=None):
-        """
-        Returns the task with the given id.
-
-        :type id:integer
-        :param id: The id of a task.
-        :param tasklist: Optional cache of get_tasks for operations
-                         where we are calling multiple times as when we
-                         are deserializing the workflow
-        :rtype: Task
-        :returns: The task with the given id.
-        """
-        if tasklist:
-            tasks = [task for task in tasklist if task.id == id]
-        else:
-            tasks = [task for task in self.get_tasks() if task.id == id]
-        return tasks[0] if len(tasks) == 1 else None
-
     def get_tasks_from_spec_name(self, name):
         """
         Returns all tasks whose spec has the given name.
 
         :type name: str
         :param name: The name of a task spec.
         :rtype: list[Task]
         :returns: A list of tasks that relate to the spec with the given name.
         """
-        return [task for task in self.get_tasks_iterator()
-                if task.task_spec.name == name]
-
-    def empty(self,str):
-        if str == None:
-            return True
-        if str == '':
-            return True
-        return False
-
-    def cancel_notify(self):
-        self.task_tree.internal_data['cancels'] = self.task_tree.internal_data.get('cancels', {})
-        self.task_tree.internal_data['cancels']['TokenReset'] = True
-        self.refresh_waiting_tasks()
-        self.do_engine_steps()
-        self.task_tree.internal_data['cancels'] = {}
+        return [task for task in self.get_tasks_iterator() if task.task_spec.name == name]
 
     def get_tasks(self, state=TaskState.ANY_MASK):
         """
         Returns a list of Task objects with the given state.
 
         :type  state: integer
         :param state: A bitmask of states.
         :rtype:  list[Task]
         :returns: A list of tasks.
         """
         return [t for t in Task.Iterator(self.task_tree, state)]
 
-    def reset_task_from_id(self, task_id):
-        """
-        Runs the task with the given id.
-
-        :type  task_id: integer
-        :param task_id: The id of the Task object.
-        """
-        if task_id is None:
-            raise WorkflowException(self.spec, 'task_id is None')
-        data = {}
-        if self.last_task and self.last_task.data:
-            data = self.last_task.data
-        for task in self.task_tree:
-            if task.id == task_id:
-                return task.reset_token(data)
-        msg = 'A task with the given task_id (%s) was not found' % task_id
-        raise WorkflowException(self.spec, msg)
-
-    def get_reset_task_spec(self, destination):
-        """
-        Returns a task, that once complete, will reset the workflow back
-        to a previously completed task.
-        :param destination: Task to reset to, on complete.
-        :return: TaskSpec
-        """
-        name = "return_to_" + destination.task_spec.name
-        spec = self.get_task_spec_from_name(name)
-        if not spec:
-            spec = LoopResetTask(self.spec, name, destination.id,
-                                 destination.task_spec.name)
-        return spec
-
     def get_tasks_iterator(self, state=TaskState.ANY_MASK):
         """
         Returns a iterator of Task objects with the given state.
 
         :type  state: integer
         :param state: A bitmask of states.
         :rtype:  Task.Iterator
         :returns: A list of tasks.
         """
         return Task.Iterator(self.task_tree, state)
 
-    def complete_task_from_id(self, task_id):
+    def get_task_from_id(self, task_id, tasklist=None):
         """
-        Runs the task with the given id.
+        Returns the task with the given id.
 
-        :type  task_id: integer
-        :param task_id: The id of the Task object.
+        :type id:integer
+        :param id: The id of a task.
+        :param tasklist: Optional cache of get_tasks for operations
+                         where we are calling multiple times as when we
+                         are deserializing the workflow
+        :rtype: Task
+        :returns: The task with the given id.
         """
         if task_id is None:
-            raise WorkflowException(self.spec, 'task_id is None')
+            raise WorkflowException('task_id is None', task_spec=self.spec)
+        tasklist = tasklist or self.task_tree
         for task in self.task_tree:
             if task.id == task_id:
-                return task.complete()
+                return task
         msg = 'A task with the given task_id (%s) was not found' % task_id
-        raise WorkflowException(self.spec, msg)
+        raise TaskNotFoundException(msg, task_spec=self.spec)
+
+    def run_task_from_id(self, task_id):
+        """
+        Runs the task with the given id.
+
+        :type  task_id: integer
+        :param task_id: The id of the Task object.
+        """
+        task = self.get_task_from_id(task_id)
+        return task.run()
+
+    def reset_from_task_id(self, task_id, data=None):
+        """
+        Runs the task with the given id.
+
+        :type  task_id: integer
+        :param task_id: The id of the Task object.
+        :param data: optionall set the task data
+        """
+        task = self.get_task_from_id(task_id)
+        return task.reset_token(data)
 
-    def complete_next(self, pick_up=True, halt_on_manual=True):
+    def run_next(self, pick_up=True, halt_on_manual=True):
         """
         Runs the next task.
         Returns True if completed, False otherwise.
 
         :type  pick_up: bool
         :param pick_up: When True, this method attempts to choose the next
                         task not by searching beginning at the root, but by
@@ -331,52 +293,52 @@
                 iter = Task.Iterator(self.last_task, TaskState.READY)
                 task = next(iter)
             except StopIteration:
                 task = None
             self.last_task = None
             if task is not None:
                 if not (halt_on_manual and task.task_spec.manual):
-                    if task.complete():
+                    if task.run():
                         self.last_task = task
                         return True
                 blacklist.append(task)
 
         # Walk through all ready tasks.
         for task in Task.Iterator(self.task_tree, TaskState.READY):
             for blacklisted_task in blacklist:
                 if task._is_descendant_of(blacklisted_task):
                     continue
             if not (halt_on_manual and task.task_spec.manual):
-                if task.complete():
+                if task.run():
                     self.last_task = task
                     return True
             blacklist.append(task)
 
         # Walk through all waiting tasks.
         for task in Task.Iterator(self.task_tree, TaskState.WAITING):
             task.task_spec._update(task)
             if not task._has_state(TaskState.WAITING):
                 self.last_task = task
                 return True
         return False
 
-    def complete_all(self, pick_up=True, halt_on_manual=True):
+    def run_all(self, pick_up=True, halt_on_manual=True):
         """
         Runs all branches until completion. This is a convenience wrapper
         around :meth:`complete_next`, and the pick_up argument is passed
         along.
 
         :type  pick_up: bool
         :param pick_up: Passed on to each call of complete_next().
         :type  halt_on_manual: bool
         :param halt_on_manual: When True, this method will not attempt to
                         complete any tasks that have manual=True.
                         See :meth:`SpiffWorkflow.specs.TaskSpec.__init__`
         """
-        while self.complete_next(pick_up, halt_on_manual):
+        while self.run_next(pick_up, halt_on_manual):
             pass
 
     def get_dump(self):
         """
         Returns a complete dump of the current internal task tree for
         debugging.
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow.egg-info/PKG-INFO` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiffWorkflow
-Version: 1.2.1
+Version: 2.0.0rc0
 Summary: A workflow framework and BPMN/DMN Processor
 Home-page: https://github.com/sartography/SpiffWorkflow
 Author: Sartography
 Author-email: dan@sartography.com
 License: lGPLv2
 Keywords: spiff workflow bpmn engine
 Classifier: Development Status :: 4 - Beta
@@ -88,15 +88,15 @@
 ## Tests
 ```
 cd tests/SpiffWorkflow
 coverage run --source=SpiffWorkflow -m unittest discover -v . "*Test.py"
 ```
 
 ## Support
-You can find us on Discord at https://discord.gg/zDEBEnrF
+You can find us on Discord at https://discord.gg/BYHcc7PpUC
 
 Commercial support for SpiffWorkflow is available from
 [Sartography](https://sartography.com)
 
 ## Contribute
 Pull Requests are and always will be welcome!
```

### Comparing `SpiffWorkflow-1.2.1/SpiffWorkflow.egg-info/SOURCES.txt` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,103 +12,120 @@
 SpiffWorkflow.egg-info/PKG-INFO
 SpiffWorkflow.egg-info/SOURCES.txt
 SpiffWorkflow.egg-info/dependency_links.txt
 SpiffWorkflow.egg-info/requires.txt
 SpiffWorkflow.egg-info/top_level.txt
 SpiffWorkflow/bpmn/FeelLikeScriptEngine.py
 SpiffWorkflow/bpmn/PythonScriptEngine.py
+SpiffWorkflow/bpmn/PythonScriptEngineEnvironment.py
 SpiffWorkflow/bpmn/__init__.py
 SpiffWorkflow/bpmn/exceptions.py
 SpiffWorkflow/bpmn/workflow.py
 SpiffWorkflow/bpmn/parser/BpmnParser.py
 SpiffWorkflow/bpmn/parser/ProcessParser.py
 SpiffWorkflow/bpmn/parser/TaskParser.py
 SpiffWorkflow/bpmn/parser/ValidationException.py
 SpiffWorkflow/bpmn/parser/__init__.py
 SpiffWorkflow/bpmn/parser/event_parsers.py
 SpiffWorkflow/bpmn/parser/node_parser.py
+SpiffWorkflow/bpmn/parser/spec_description.py
 SpiffWorkflow/bpmn/parser/task_parsers.py
 SpiffWorkflow/bpmn/parser/util.py
-SpiffWorkflow/bpmn/serializer/BpmnSerializer.py
-SpiffWorkflow/bpmn/serializer/CompactWorkflowSerializer.py
-SpiffWorkflow/bpmn/serializer/Packager.py
+SpiffWorkflow/bpmn/parser/schema/BPMN20.xsd
+SpiffWorkflow/bpmn/parser/schema/BPMNDI.xsd
+SpiffWorkflow/bpmn/parser/schema/DC.xsd
+SpiffWorkflow/bpmn/parser/schema/DI.xsd
+SpiffWorkflow/bpmn/parser/schema/Semantic.xsd
 SpiffWorkflow/bpmn/serializer/__init__.py
-SpiffWorkflow/bpmn/serializer/bpmn_converters.py
-SpiffWorkflow/bpmn/serializer/dict.py
-SpiffWorkflow/bpmn/serializer/dictionary.py
-SpiffWorkflow/bpmn/serializer/json.py
-SpiffWorkflow/bpmn/serializer/task_spec_converters.py
-SpiffWorkflow/bpmn/serializer/version_migration.py
+SpiffWorkflow/bpmn/serializer/data_spec.py
+SpiffWorkflow/bpmn/serializer/event_definition.py
+SpiffWorkflow/bpmn/serializer/process_spec.py
+SpiffWorkflow/bpmn/serializer/task_spec.py
 SpiffWorkflow/bpmn/serializer/workflow.py
-SpiffWorkflow/bpmn/serializer/workflow_spec_converter.py
-SpiffWorkflow/bpmn/specs/BpmnProcessSpec.py
-SpiffWorkflow/bpmn/specs/BpmnSpecMixin.py
-SpiffWorkflow/bpmn/specs/ExclusiveGateway.py
-SpiffWorkflow/bpmn/specs/InclusiveGateway.py
-SpiffWorkflow/bpmn/specs/ManualTask.py
-SpiffWorkflow/bpmn/specs/MultiInstanceTask.py
-SpiffWorkflow/bpmn/specs/NoneTask.py
-SpiffWorkflow/bpmn/specs/ParallelGateway.py
-SpiffWorkflow/bpmn/specs/ScriptTask.py
-SpiffWorkflow/bpmn/specs/ServiceTask.py
-SpiffWorkflow/bpmn/specs/SubWorkflowTask.py
-SpiffWorkflow/bpmn/specs/UnstructuredJoin.py
-SpiffWorkflow/bpmn/specs/UserTask.py
+SpiffWorkflow/bpmn/serializer/helpers/__init__.py
+SpiffWorkflow/bpmn/serializer/helpers/dictionary.py
+SpiffWorkflow/bpmn/serializer/helpers/registry.py
+SpiffWorkflow/bpmn/serializer/helpers/spec.py
+SpiffWorkflow/bpmn/serializer/migration/__init__.py
+SpiffWorkflow/bpmn/serializer/migration/exceptions.py
+SpiffWorkflow/bpmn/serializer/migration/version_1_1.py
+SpiffWorkflow/bpmn/serializer/migration/version_1_2.py
+SpiffWorkflow/bpmn/serializer/migration/version_migration.py
 SpiffWorkflow/bpmn/specs/__init__.py
-SpiffWorkflow/bpmn/specs/events/EndEvent.py
-SpiffWorkflow/bpmn/specs/events/IntermediateEvent.py
-SpiffWorkflow/bpmn/specs/events/StartEvent.py
-SpiffWorkflow/bpmn/specs/events/__init__.py
-SpiffWorkflow/bpmn/specs/events/event_definitions.py
-SpiffWorkflow/bpmn/specs/events/event_types.py
+SpiffWorkflow/bpmn/specs/bpmn_process_spec.py
+SpiffWorkflow/bpmn/specs/bpmn_task_spec.py
+SpiffWorkflow/bpmn/specs/control.py
+SpiffWorkflow/bpmn/specs/data_spec.py
+SpiffWorkflow/bpmn/specs/defaults.py
+SpiffWorkflow/bpmn/specs/event_definitions.py
+SpiffWorkflow/bpmn/specs/mixins/__init__.py
+SpiffWorkflow/bpmn/specs/mixins/bpmn_spec_mixin.py
+SpiffWorkflow/bpmn/specs/mixins/exclusive_gateway.py
+SpiffWorkflow/bpmn/specs/mixins/inclusive_gateway.py
+SpiffWorkflow/bpmn/specs/mixins/manual_task.py
+SpiffWorkflow/bpmn/specs/mixins/multiinstance_task.py
+SpiffWorkflow/bpmn/specs/mixins/none_task.py
+SpiffWorkflow/bpmn/specs/mixins/parallel_gateway.py
+SpiffWorkflow/bpmn/specs/mixins/script_task.py
+SpiffWorkflow/bpmn/specs/mixins/service_task.py
+SpiffWorkflow/bpmn/specs/mixins/subworkflow_task.py
+SpiffWorkflow/bpmn/specs/mixins/unstructured_join.py
+SpiffWorkflow/bpmn/specs/mixins/user_task.py
+SpiffWorkflow/bpmn/specs/mixins/events/__init__.py
+SpiffWorkflow/bpmn/specs/mixins/events/end_event.py
+SpiffWorkflow/bpmn/specs/mixins/events/event_types.py
+SpiffWorkflow/bpmn/specs/mixins/events/intermediate_event.py
+SpiffWorkflow/bpmn/specs/mixins/events/start_event.py
 SpiffWorkflow/camunda/__init__.py
 SpiffWorkflow/camunda/parser/CamundaParser.py
-SpiffWorkflow/camunda/parser/UserTaskParser.py
 SpiffWorkflow/camunda/parser/__init__.py
-SpiffWorkflow/camunda/parser/business_rule_task.py
 SpiffWorkflow/camunda/parser/event_parsers.py
+SpiffWorkflow/camunda/parser/task_spec.py
 SpiffWorkflow/camunda/serializer/__init__.py
-SpiffWorkflow/camunda/serializer/task_spec_converters.py
-SpiffWorkflow/camunda/specs/UserTask.py
+SpiffWorkflow/camunda/serializer/config.py
+SpiffWorkflow/camunda/serializer/event_definition.py
+SpiffWorkflow/camunda/serializer/task_spec.py
 SpiffWorkflow/camunda/specs/__init__.py
-SpiffWorkflow/camunda/specs/events/__init__.py
-SpiffWorkflow/camunda/specs/events/event_definitions.py
+SpiffWorkflow/camunda/specs/business_rule_task.py
+SpiffWorkflow/camunda/specs/event_definitions.py
+SpiffWorkflow/camunda/specs/multiinstance_task.py
+SpiffWorkflow/camunda/specs/user_task.py
 SpiffWorkflow/dmn/__init__.py
 SpiffWorkflow/dmn/engine/DMNEngine.py
 SpiffWorkflow/dmn/engine/__init__.py
 SpiffWorkflow/dmn/parser/BpmnDmnParser.py
 SpiffWorkflow/dmn/parser/DMNParser.py
 SpiffWorkflow/dmn/parser/__init__.py
+SpiffWorkflow/dmn/parser/schema/DC.xsd
+SpiffWorkflow/dmn/parser/schema/DMN.xsd
+SpiffWorkflow/dmn/parser/schema/DMN12.xsd
+SpiffWorkflow/dmn/parser/schema/DMN13.xsd
+SpiffWorkflow/dmn/parser/schema/DMNDI12.xsd
+SpiffWorkflow/dmn/parser/schema/DMNDI13.xsd
 SpiffWorkflow/dmn/serializer/__init__.py
-SpiffWorkflow/dmn/serializer/task_spec_converters.py
-SpiffWorkflow/dmn/specs/BusinessRuleTask.py
+SpiffWorkflow/dmn/serializer/task_spec.py
 SpiffWorkflow/dmn/specs/__init__.py
+SpiffWorkflow/dmn/specs/business_rule_task_mixin.py
 SpiffWorkflow/dmn/specs/model.py
 SpiffWorkflow/serializer/__init__.py
 SpiffWorkflow/serializer/base.py
 SpiffWorkflow/serializer/dict.py
 SpiffWorkflow/serializer/dotv.py
 SpiffWorkflow/serializer/exceptions.py
 SpiffWorkflow/serializer/json.py
 SpiffWorkflow/serializer/prettyxml.py
 SpiffWorkflow/serializer/xml.py
-SpiffWorkflow/signavio/__init__.py
-SpiffWorkflow/signavio/parser/__init__.py
-SpiffWorkflow/signavio/parser/bpmn.py
-SpiffWorkflow/signavio/parser/tasks.py
 SpiffWorkflow/specs/AcquireMutex.py
 SpiffWorkflow/specs/Cancel.py
 SpiffWorkflow/specs/CancelTask.py
-SpiffWorkflow/specs/Celery.py
 SpiffWorkflow/specs/Choose.py
 SpiffWorkflow/specs/ExclusiveChoice.py
 SpiffWorkflow/specs/Execute.py
 SpiffWorkflow/specs/Gate.py
 SpiffWorkflow/specs/Join.py
-SpiffWorkflow/specs/LoopResetTask.py
 SpiffWorkflow/specs/Merge.py
 SpiffWorkflow/specs/MultiChoice.py
 SpiffWorkflow/specs/MultiInstance.py
 SpiffWorkflow/specs/ReleaseMutex.py
 SpiffWorkflow/specs/Simple.py
 SpiffWorkflow/specs/StartTask.py
 SpiffWorkflow/specs/SubWorkflow.py
@@ -122,26 +139,23 @@
 SpiffWorkflow/specs/base.py
 SpiffWorkflow/spiff/__init__.py
 SpiffWorkflow/spiff/parser/__init__.py
 SpiffWorkflow/spiff/parser/event_parsers.py
 SpiffWorkflow/spiff/parser/process.py
 SpiffWorkflow/spiff/parser/task_spec.py
 SpiffWorkflow/spiff/serializer/__init__.py
-SpiffWorkflow/spiff/serializer/task_spec_converters.py
+SpiffWorkflow/spiff/serializer/config.py
+SpiffWorkflow/spiff/serializer/event_definition.py
+SpiffWorkflow/spiff/serializer/task_spec.py
 SpiffWorkflow/spiff/specs/__init__.py
-SpiffWorkflow/spiff/specs/manual_task.py
-SpiffWorkflow/spiff/specs/none_task.py
-SpiffWorkflow/spiff/specs/script_task.py
-SpiffWorkflow/spiff/specs/service_task.py
+SpiffWorkflow/spiff/specs/defaults.py
+SpiffWorkflow/spiff/specs/event_definitions.py
 SpiffWorkflow/spiff/specs/spiff_task.py
-SpiffWorkflow/spiff/specs/subworkflow_task.py
-SpiffWorkflow/spiff/specs/user_task.py
-SpiffWorkflow/spiff/specs/events/__init__.py
-SpiffWorkflow/spiff/specs/events/event_definitions.py
-SpiffWorkflow/spiff/specs/events/event_types.py
+SpiffWorkflow/spiff/specs/mixins/__init__.py
+SpiffWorkflow/spiff/specs/mixins/service_task.py
 SpiffWorkflow/util/__init__.py
 SpiffWorkflow/util/compat.py
 SpiffWorkflow/util/deep_merge.py
 SpiffWorkflow/util/event.py
 SpiffWorkflow/util/impl.py
 SpiffWorkflow/util/levenshtein.py
 SpiffWorkflow/util/weakmethod.py
```

### Comparing `SpiffWorkflow-1.2.1/setup.py` & `SpiffWorkflow-2.0.0rc0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='SpiffWorkflow',
-      version='1.2.1',
+      version='2.0.0rc0',
       description='A workflow framework and BPMN/DMN Processor',
       long_description=README,
       long_description_content_type="text/markdown",
       author='Sartography',
       author_email='dan@sartography.com',
       license='lGPLv2',
       packages=find_packages(exclude=['tests', 'tests.*']),
-      install_requires=['configparser', 'lxml', 'celery', 'dateparser', 'pytz',
+      package_data={
+          'SpiffWorkflow.bpmn.parser': ['schema/*.xsd'],
+          'SpiffWorkflow.dmn.parser': ['schema/*.xsd'],
+      },
+      install_requires=['configparser', 'lxml',
           # required for python 3.7 - https://stackoverflow.com/a/73932581
           'importlib-metadata<5.0; python_version <= "3.7"'],
       keywords='spiff workflow bpmn engine',
       url='https://github.com/sartography/SpiffWorkflow',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Intended Audience :: Developers',
```


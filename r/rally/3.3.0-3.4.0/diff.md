# Comparing `tmp/rally-3.3.0.tar.gz` & `tmp/rally-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rally-3.3.0.tar", last modified: Thu Jun 17 11:50:00 2021, max compression
+gzip compressed data, was "rally-3.4.0.tar", last modified: Fri May 26 08:45:05 2023, max compression
```

## Comparing `rally-3.3.0.tar` & `rally-3.4.0.tar`

### file list

```diff
@@ -1,767 +1,775 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.758591 rally-3.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-06-17 11:49:25.000000 rally-3.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-06-17 11:49:25.000000 rally-3.3.0/.dockerignore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.674586 rally-3.3.0/.zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2365 2021-06-17 11:49:25.000000 rally-3.3.0/.zuul.d/docker-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2021-06-17 11:49:25.000000 rally-3.3.0/.zuul.d/install-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2425 2021-06-17 11:49:25.000000 rally-3.3.0/.zuul.d/python-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2021-06-17 11:49:25.000000 rally-3.3.0/.zuul.d/zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17415 2021-06-17 11:50:00.000000 rally-3.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13924 2021-06-17 11:49:25.000000 rally-3.3.0/CHANGELOG.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2021-06-17 11:49:25.000000 rally-3.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   158369 2021-06-17 11:50:00.000000 rally-3.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3715 2021-06-17 11:49:25.000000 rally-3.3.0/DOCKER_README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1245 2021-06-17 11:49:25.000000 rally-3.3.0/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2021-06-17 11:49:25.000000 rally-3.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5895 2021-06-17 11:50:00.758591 rally-3.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4001 2021-06-17 11:49:25.000000 rally-3.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2021-06-17 11:49:25.000000 rally-3.3.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.678586 rally-3.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1292 2021-06-17 11:49:25.000000 rally-3.3.0/doc/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.678586 rally-3.3.0/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8051 2021-06-17 11:49:25.000000 rally-3.3.0/doc/ext/cli_reference.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2021-06-17 11:49:25.000000 rally-3.3.0/doc/ext/include_vars.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16313 2021-06-17 11:49:25.000000 rally-3.3.0/doc/ext/plugin_reference.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2021-06-17 11:49:25.000000 rally-3.3.0/doc/ext/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.678586 rally-3.3.0/doc/feature_request/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/capture_task_logging.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/check_queue_perfdata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/comparing_results_of_2_tasks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/distributed_load_generation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/explicitly_specify_existing_users_for_scenarios.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/historical_performance_data.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.678586 rally-3.3.0/doc/feature_request/implemented/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/implemented/LDAP_support.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/implemented/add_possibility_to_specify_concurrency_for_tempest.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2361 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/implemented/stop_scenario_after_several_errors.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/installation_script_enhancements.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/installing_isolated.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/launch_specific_benchmark.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/multi_scenarios_load_gen.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/multiple_attach_volume.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/persistence_benchmark_env.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2021-06-17 11:49:25.000000 rally-3.3.0/doc/feature_request/production_ready_cleanup.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.678586 rally-3.3.0/doc/release_notes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.682586 rally-3.3.0/doc/release_notes/archive/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.0.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.0.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3786 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.0.3.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7345 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.0.4.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13260 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.1.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.1.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.1.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22893 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.10.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.10.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10366 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.11.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2904 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.11.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2534 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.11.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.12.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.12.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4818 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.2.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5616 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.3.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.3.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.3.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.3.3.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8588 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.4.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13852 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.5.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7624 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.6.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5842 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.7.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10065 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.8.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.8.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5551 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.9.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.9.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v0.9.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive/v1.0.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/archive.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2021-06-17 11:49:25.000000 rally-3.3.0/doc/release_notes/latest.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2021-06-17 11:49:25.000000 rally-3.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.682586 rally-3.3.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6758 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.662585 rally-3.3.0/doc/source/_templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.682586 rally-3.3.0/doc/source/_templates/openstackrally/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.686586 rally-3.3.0/doc/source/_templates/openstackrally/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/_templates/openstackrally/_static/img.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/_templates/openstackrally/layout.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       27 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/_templates/openstackrally/theme.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/cli_reference.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9583 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2296 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/contribute.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/feature_requests.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.694587 rally-3.3.0/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18652 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Amqp_rpc_single_reply_queue.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64751 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Hook-Aggregated-Report.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    88398 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Hook-Per-Hook-Report.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38695 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Hook-Results.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    95868 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally-Actions.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29546 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally-Plugins.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   127052 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally-UseCases.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   175620 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally_Architecture.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   168071 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally_Distributed_Runner.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105436 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally_QA.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67056 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally_VM_list.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   116187 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally_snapshot_vm.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59267 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Rally_who_is_using.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   118771 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Abort-on-SLA-task-1.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   133861 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Abort-on-SLA-task-2.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   188455 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Collage.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48010 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Multiple-Configurations-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44839 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Multiple-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39473 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40004 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-SLA-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    73756 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-SLA-Scenario.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    76785 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Scenario-Atomic.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   111232 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Scenario-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20517 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Actions-durations.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24204 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Distribution.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77249 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Failures.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   103829 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Input-file.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8784 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Load-profile.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   101257 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28224 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-SLA.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55099 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Scenario-Data-Aggregated.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25172 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration-profiler.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82653 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20731 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Subtask-configuration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34215 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Task-Total-durations.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74855 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Trends-Atomic-actions.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21142 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Trends-Configuration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25032 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Trends-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    75196 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Trends-Total.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9812 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Trends-single-run.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81001 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Verify-filter-by-status.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    98165 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Verify-for-4-Verifications.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26831 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Verify-toggle-tags.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    84067 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Verify-tracebacks.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   134147 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/images/Report-Verify-xfail.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.694587 rally-3.3.0/doc/source/install_and_upgrade/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/install_and_upgrade/db_migrations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/install_and_upgrade/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1390 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/install_and_upgrade/install.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.694587 rally-3.3.0/doc/source/overview/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4945 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/overview/glossary.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/overview/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6449 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/overview/overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/overview/user_stories.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.694587 rally-3.3.0/doc/source/plugins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.694587 rally-3.3.0/doc/source/plugins/implementation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4729 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/plugins/implementation/context_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11825 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/plugins/implementation/hook_and_trigger_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/plugins/implementation/runner_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/plugins/implementation/scenario_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/plugins/implementation/sla_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2615 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/plugins/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/plugins/plugin_reference.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.694587 rally-3.3.0/doc/source/project_info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9741 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/project_info/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/project_info/release_notes.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.694587 rally-3.3.0/doc/source/quick_start/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/gates.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.698587 rally-3.3.0/doc/source/quick_start/tutorial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1687 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_0_installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2778 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13844 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9129 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_2_input_task_format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5211 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5731 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10059 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_5_task_templates.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6075 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8178 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_7_working_with_multple_openstack_clouds.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8103 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_8_discovering_more_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45309 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial/step_9_verifying_cloud_via_tempest_verifier.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/quick_start/tutorial.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.698587 rally-3.3.0/doc/source/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10006 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/task/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.698587 rally-3.3.0/doc/source/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/cli_reference.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.698587 rally-3.3.0/doc/source/verification/howto/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3773 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/howto/add_new_reporter.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/howto/add_support_for_new_tool.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/howto/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16640 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/howto/migrate_from_old_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3075 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4254 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/reports.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3626 2021-06-17 11:49:25.000000 rally-3.3.0/doc/source/verification/verifiers.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.698587 rally-3.3.0/doc/specs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/doc/specs/implemented/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2713 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/class-based-scenarios.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4492 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/consistent_resource_names.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10835 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/db_refactoring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6472 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/deployment_type.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7816 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/hook_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/improve_atomic_actions_format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11368 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/improve_scenario_output_format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10567 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/new_rally_input_task_format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/osprofiler.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/pluggable_validators.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1466 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/sla_pd_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/split_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/task_and_verification_export.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30381 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/implemented/verification_refactoring.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/doc/specs/in-progress/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/in-progress/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7564 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/in-progress/cleanup_refactoring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5158 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/in-progress/distributed_runner.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11197 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/in-progress/pluggable-types.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11188 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/in-progress/raas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11465 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/in-progress/refactor_scenario_utils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2021-06-17 11:49:25.000000 rally-3.3.0/doc/specs/template.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.662585 rally-3.3.0/doc/user_stories/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/doc/user_stories/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6391 2021-06-17 11:49:25.000000 rally-3.3.0/doc/user_stories/keystone/authenticate.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/doc/user_stories/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8685 2021-06-17 11:49:25.000000 rally-3.3.0/doc/user_stories/nova/boot_server.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2021-06-17 11:49:25.000000 rally-3.3.0/etc/motd_for_docker
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/etc/rally/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-06-17 11:49:25.000000 rally-3.3.0/etc/rally/rally-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11258 2021-06-17 11:49:25.000000 rally-3.3.0/etc/rally/rally.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4643 2021-06-17 11:49:25.000000 rally-3.3.0/etc/rally.bash_completion
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/rally/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.706587 rally-3.3.0/rally/aas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-06-17 11:49:25.000000 rally-3.3.0/rally/aas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    54948 2021-06-17 11:49:25.000000 rally-3.3.0/rally/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.706587 rally-3.3.0/rally/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27184 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/cliutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.706587 rally-3.3.0/rally/cli/commands/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/commands/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/commands/db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15083 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/commands/deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13986 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/commands/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4609 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/commands/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37125 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/commands/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40419 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/commands/verify.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6286 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/envutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9054 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/task_results_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2021-06-17 11:49:25.000000 rally-3.3.0/rally/cli/yamlutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.710588 rally-3.3.0/rally/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2699 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/broker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/cfg.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.710588 rally-3.3.0/rally/common/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24554 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.710588 rally-3.3.0/rally/common/db/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.714588 rally-3.3.0/rally/common/db/migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7920 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_01_ca3626f62937_init_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_03_3177d36ea270_merge_credentials_from_users_and_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5678 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_04_4ef544102ba7_change_task_status_enum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15421 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_04_e654a0648db0_refactor_task_results.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2938 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_07_54e844ebfbc3_update_deployment_configs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_08_32fada9b2fde_remove_admin_domain_name.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3778 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_09_08e1515a576c_fix_invalid_verification_logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_09_6ad4f426f005_add_hooks_to_task_result.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7712 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_11_484cd9413e66_new_db_schema_for_verification_component.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2016_12_37fdbb373e8d_fix_test_results_for_verifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_01_a6f364988fc2_change_tag_type_enum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_01_f33f4610dcda_change_verification_statuses.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_02_92aaaa2a6bb3_refactor_credentials.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3450 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_06_35fe16d4ab1c_update_tasks_based_on_workloads.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_06_c517b0011857_fill_missed_workload_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_07_7948b83229f6_workload_min_max_durations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_08_fab4f4f31f8a_fill_missed_workload_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2221 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_09_046a38742e89_port_configs_to_new_formats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_09_e0a5df2c5153_upsize_the_size_of_task_title.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5002 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_10_4394bdc32cfd_fill_missed_workload_info_r3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_10_9a18c6fe265c_rename_namespace_to_platform.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8561 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_10_dc46687661df_update_contexts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2017_12_a43700a813a5_add_env_platforms_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2018_01_44169f4d455e_deleted_worker_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2018_01_7287df262dbc_move_deployment_to_env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2018_02_95208e4eface_add_config_field_to_env_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7981 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2018_02_bc908ac9a1fc_move_deployment_to_env_2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2285 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/migrations/versions/2018_02_dc0fe6de6786_update_old_deployment_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11978 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5215 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/sa_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5099 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/db/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/fileutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.714588 rally-3.3.0/rally/common/io/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/io/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5509 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/io/junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9839 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/io/subunit_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11272 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/logging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.714588 rally-3.3.0/rally/common/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/objects/deploy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24513 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/objects/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3248 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/objects/verification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/objects/verifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.714588 rally-3.3.0/rally/common/plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5846 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/plugin/discover.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4372 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/plugin/info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4549 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/plugin/meta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7390 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/plugin/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/sshutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7808 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/streaming_algorithms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26145 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10594 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2021-06-17 11:49:25.000000 rally-3.3.0/rally/common/yamlutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6911 2021-06-17 11:49:25.000000 rally-3.3.0/rally/consts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.714588 rally-3.3.0/rally/env/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/env/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25830 2021-06-17 11:49:25.000000 rally-3.3.0/rally/env/env_mgr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3978 2021-06-17 11:49:25.000000 rally-3.3.0/rally/env/platform.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6680 2021-06-17 11:49:25.000000 rally-3.3.0/rally/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.714588 rally-3.3.0/rally/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.714588 rally-3.3.0/rally/plugins/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.714588 rally-3.3.0/rally/plugins/common/exporters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/exporters/elastic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/elastic/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      936 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/elastic/client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      940 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/elastic/exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/elastic/flatten.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/html.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/json_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/exporters/trends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/hook/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/hook/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/hook/sys_call.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/hook/triggers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/hook/triggers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/hook/triggers/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/hook/triggers/periodic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/runners/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/runners/constant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/runners/rps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/runners/serial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/scenarios/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/scenarios/dummy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/scenarios/dummy/dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/scenarios/requests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/scenarios/requests/http_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/scenarios/requests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/sla/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/sla/failure_rate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/sla/iteration_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/sla/max_average_duration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/sla/max_average_duration_per_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/sla/outliers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/sla/performance_degradation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16380 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/common/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/verification/reporters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/common/verification/testr.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.718588 rally-3.3.0/rally/plugins/task/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/contexts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/contexts/dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/exporters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/exporters/elastic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/elastic/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6196 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/elastic/client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16360 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/elastic/exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/elastic/flatten.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/html.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5596 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/json_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3560 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/old_json_results.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1406 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/exporters/trends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/hook_triggers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/hook_triggers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/hook_triggers/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2702 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/hook_triggers/periodic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/hooks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2562 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/hooks/sys_call.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/runners/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14074 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/runners/constant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11662 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/runners/rps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3062 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/runners/serial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/scenarios/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/scenarios/dummy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11367 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/scenarios/dummy/dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/scenarios/requests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/scenarios/requests/http_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/scenarios/requests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.722588 rally-3.3.0/rally/plugins/task/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/sla/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/sla/failure_rate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/sla/iteration_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/sla/max_average_duration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3150 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/sla/max_average_duration_per_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/sla/outliers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/sla/performance_degradation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/task/types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.726589 rally-3.3.0/rally/plugins/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18676 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/verification/reporters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5791 2021-06-17 11:49:25.000000 rally-3.3.0/rally/plugins/verification/testr.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.726589 rally-3.3.0/rally/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4535 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11493 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21514 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/engine.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3544 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7062 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/functional.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8618 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/hook.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.726589 rally-3.3.0/rally/task/processing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/processing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35108 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/processing/charts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16819 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/processing/plot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3080 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/processing/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9895 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/runner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7474 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/scenario.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14952 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6003 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/sla.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15607 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/task_cfg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8847 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2021-06-17 11:49:25.000000 rally-3.3.0/rally/task/validation.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.726589 rally-3.3.0/rally/ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.726589 rally-3.3.0/rally/ui/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2802 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/base.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.726589 rally-3.3.0/rally/ui/templates/ci/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/ci/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2138 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/ci/index_verify.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/rally/ui/templates/libs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/libs/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   124229 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/libs/angular.1.3.3.min.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   148039 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/libs/d3.3.4.13.min.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8796 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   188436 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/rally/ui/templates/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10234 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/task/directive_widget.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31337 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/task/report.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17746 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/task/trends.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/rally/ui/templates/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12229 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/templates/verification/report.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2021-06-17 11:49:25.000000 rally-3.3.0/rally/ui/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/rally/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2021-06-17 11:49:25.000000 rally-3.3.0/rally/utils/encodeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10743 2021-06-17 11:49:25.000000 rally-3.3.0/rally/utils/sshutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2021-06-17 11:49:25.000000 rally-3.3.0/rally/utils/strutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/rally/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2021-06-17 11:49:25.000000 rally-3.3.0/rally/verification/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16784 2021-06-17 11:49:25.000000 rally-3.3.0/rally/verification/manager.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3035 2021-06-17 11:49:25.000000 rally-3.3.0/rally/verification/reporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2021-06-17 11:49:25.000000 rally-3.3.0/rally/verification/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/rally-jobs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2021-06-17 11:49:25.000000 rally-3.3.0/rally-jobs/plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally-jobs/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2021-06-17 11:49:25.000000 rally-3.3.0/rally-jobs/plugins/fake_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2021-06-17 11:49:25.000000 rally-3.3.0/rally-jobs/plugins/rally_profile.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.702587 rally-3.3.0/rally-jobs/plugins/test_relative_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/rally-jobs/plugins/test_relative_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2021-06-17 11:49:25.000000 rally-3.3.0/rally-jobs/plugins/test_relative_import/zzz.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11899 2021-06-17 11:49:25.000000 rally-3.3.0/rally-jobs/self-rally.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.706587 rally-3.3.0/rally.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5895 2021-06-17 11:50:00.000000 rally-3.3.0/rally.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25578 2021-06-17 11:50:00.000000 rally-3.3.0/rally.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-06-17 11:50:00.000000 rally-3.3.0/rally.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-06-17 11:50:00.000000 rally-3.3.0/rally.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-06-17 11:50:00.000000 rally-3.3.0/rally.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-06-17 11:50:00.000000 rally-3.3.0/rally.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2021-06-17 11:50:00.000000 rally-3.3.0/rally.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-06-17 11:50:00.000000 rally-3.3.0/rally.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2021-06-17 11:49:25.000000 rally-3.3.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-06-17 11:49:25.000000 rally-3.3.0/samples/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/samples/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/samples/tasks/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/contexts/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/contexts/dummy-context.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/contexts/dummy-context.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/samples/tasks/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/samples/tasks/runners/constant/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/constant/constant-for-duration.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/constant/constant-for-duration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/constant/constant-timeout.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/constant/constant-timeout.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/samples/tasks/runners/rps/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/rps/rps.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/rps/rps.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/samples/tasks/runners/serial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/serial/serial.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/runners/serial/serial.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.730589 rally-3.3.0/samples/tasks/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.734589 rally-3.3.0/samples/tasks/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-exception-probability.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-exception-probability.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-exception.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-exception.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-failure.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-failure.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-output.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-output.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-random-action.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-random-action.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/dummy/dummy.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.734589 rally-3.3.0/samples/tasks/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/requests/check-random-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/requests/check-random-request.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/requests/check-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/scenarios/requests/check-request.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.734589 rally-3.3.0/samples/tasks/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/sla/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/sla/dummy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-06-17 11:49:25.000000 rally-3.3.0/samples/tasks/sla/dummy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2021-06-17 11:50:00.758591 rally-3.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2021-06-17 11:49:25.000000 rally-3.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2021-06-17 11:49:25.000000 rally-3.3.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.734589 rally-3.3.0/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2021-06-17 11:49:25.000000 rally-3.3.0/tests/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.734589 rally-3.3.0/tests/ci/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2323 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/cover.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/ci/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/docker-build-and-check.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/docker-build-check-and-push.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2653 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/rally-install-pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/rally-install-run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.670585 rally-3.3.0/tests/ci/playbooks/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.670585 rally-3.3.0/tests/ci/playbooks/roles/docker-build-image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/ci/playbooks/roles/docker-build-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/roles/docker-build-image/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/ci/playbooks/roles/docker-build-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.670585 rally-3.3.0/tests/ci/playbooks/roles/docker-push-image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/ci/playbooks/roles/docker-push-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/roles/docker-push-image/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/ci/playbooks/roles/docker-push-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1660 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/tox-install.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/playbooks/tox-run.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3993 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/pytest_launcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/rally_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4012 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/rally_self_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/render.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13962 2021-06-17 11:49:25.000000 rally-3.3.0/tests/ci/sync_requirements.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/functional/extra/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/functional/extra/fake_dir1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/extra/fake_dir1/fake_plugin1.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/functional/extra/fake_dir2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/extra/fake_dir2/fake_plugin2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/extra/fake_platforms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2044 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/extra/fake_verify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/extra/test_fake_scenario.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/test_cli_deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3216 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/test_cli_env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/test_cli_functional.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/test_cli_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58028 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/test_cli_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5542 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/test_cli_verify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/test_lib_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7839 2021-06-17 11:49:25.000000 rally-3.3.0/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21689 2021-06-17 11:49:25.000000 rally-3.3.0/tests/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.738589 rally-3.3.0/tests/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/samples/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7006 2021-06-17 11:49:25.000000 rally-3.3.0/tests/samples/test_task_samples.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.742590 rally-3.3.0/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.742590 rally-3.3.0/tests/unit/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.742590 rally-3.3.0/tests/unit/cli/commands/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/commands/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/commands/test_db.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23141 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/commands/test_deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/commands/test_docstrings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21802 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/commands/test_env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/commands/test_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50082 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/commands/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36667 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/commands/test_verify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37060 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/test_cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5589 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/test_envutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9219 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/test_task_results_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/cli/test_yamlutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.742590 rally-3.3.0/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.746590 rally-3.3.0/tests/unit/common/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38662 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/db/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   111129 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/db/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5796 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/db/test_migrations_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5995 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/db/test_types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.746590 rally-3.3.0/tests/unit/common/io/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/io/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3470 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/io/subunit_v2.stream
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2334 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/io/test_junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6267 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/io/test_subunit_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.746590 rally-3.3.0/tests/unit/common/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8664 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/objects/test_deploy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26722 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/objects/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6230 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/objects/test_verification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/objects/test_verifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.746590 rally-3.3.0/tests/unit/common/plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9817 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/plugin/test_discover.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4208 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/plugin/test_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5204 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/plugin/test_meta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/plugin/test_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2822 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/test_broker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12226 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10136 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/test_streaming_algorithms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27264 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6137 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/test_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/common/test_version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.746590 rally-3.3.0/tests/unit/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/doc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/doc/test_docker_readme.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6020 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/doc/test_docstrings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/doc/test_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8647 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/doc/test_jsonschemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4530 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/doc/test_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/doc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.746590 rally-3.3.0/tests/unit/env/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/env/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31964 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/env/test_env_mgr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/env/test_platform.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4637 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.746590 rally-3.3.0/tests/unit/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17384 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/common/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/contexts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/contexts/test_dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/exporters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4766 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/dummy_data.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/exporters/elastic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/elastic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8347 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/elastic/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20745 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/elastic/test_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/elastic/test_flatten.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/junit_report.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/test_html.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5144 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/test_json_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/test_junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5414 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/test_old_json_results.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/exporters/test_trends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/hook_triggers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/hook_triggers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2774 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/hook_triggers/test_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3498 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/hook_triggers/test_periodic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/hooks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/hooks/test_sys_call.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/runners/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13700 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/runners/test_constant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13691 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/runners/test_rps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2937 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/runners/test_serial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/scenarios/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/scenarios/dummy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9988 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/scenarios/dummy/test_dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.750590 rally-3.3.0/tests/unit/plugins/task/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/scenarios/requests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/scenarios/requests/test_http_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/scenarios/requests/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.754590 rally-3.3.0/tests/unit/plugins/task/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/sla/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4983 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/sla/test_failure_rate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/sla/test_iteration_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/sla/test_max_average_duration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5397 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/sla/test_max_average_duration_per_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5363 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/sla/test_outliers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3428 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/sla/test_performance_degradation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3558 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/task/test_types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.754590 rally-3.3.0/tests/unit/plugins/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/verification/junit_report.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18394 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/verification/test_reporters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17456 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/plugins/verification/test_testr.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.754590 rally-3.3.0/tests/unit/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.754590 rally-3.3.0/tests/unit/task/processing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/processing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47254 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/processing/test_charts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33744 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/processing/test_plot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4654 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/processing/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4935 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13920 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43091 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_functional.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13183 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_hook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9218 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_runner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6440 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_scenario.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9279 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6932 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_sla.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11894 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_task_cfg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5377 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23353 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/task/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90112 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_ddt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15398 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12518 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_mock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2569 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_pytest_launcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_test_ddt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14784 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/test_test_mock.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.754590 rally-3.3.0/tests/unit/ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/ui/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/ui/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.758591 rally-3.3.0/tests/unit/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/utils/test_encodeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14022 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/utils/test_sshutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7744 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/utils/test_strutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:50:00.758591 rally-3.3.0/tests/unit/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/verification/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15834 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/verification/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3241 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/verification/test_reporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3837 2021-06-17 11:49:25.000000 rally-3.3.0/tests/unit/verification/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4949 2021-06-17 11:49:25.000000 rally-3.3.0/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2021-06-17 11:49:25.000000 rally-3.3.0/upper-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.505195 rally-3.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-26 08:44:34.000000 rally-3.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2023-05-26 08:44:34.000000 rally-3.4.0/.dockerignore
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.381155 rally-3.4.0/.zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2023-05-26 08:44:34.000000 rally-3.4.0/.zuul.d/docker-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-05-26 08:44:34.000000 rally-3.4.0/.zuul.d/install-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2652 2023-05-26 08:44:34.000000 rally-3.4.0/.zuul.d/python-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-05-26 08:44:34.000000 rally-3.4.0/.zuul.d/zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17551 2023-05-26 08:45:05.000000 rally-3.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14673 2023-05-26 08:44:34.000000 rally-3.4.0/CHANGELOG.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-05-26 08:44:34.000000 rally-3.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   158962 2023-05-26 08:45:04.000000 rally-3.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3692 2023-05-26 08:44:34.000000 rally-3.4.0/DOCKER_README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2023-05-26 08:44:34.000000 rally-3.4.0/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2023-05-26 08:44:34.000000 rally-3.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5996 2023-05-26 08:45:05.505195 rally-3.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4001 2023-05-26 08:44:34.000000 rally-3.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2023-05-26 08:44:34.000000 rally-3.4.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.381155 rally-3.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1292 2023-05-26 08:44:34.000000 rally-3.4.0/doc/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.381155 rally-3.4.0/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8055 2023-05-26 08:44:34.000000 rally-3.4.0/doc/ext/cli_reference.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2023-05-26 08:44:34.000000 rally-3.4.0/doc/ext/include_vars.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16313 2023-05-26 08:44:34.000000 rally-3.4.0/doc/ext/plugin_reference.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2023-05-26 08:44:34.000000 rally-3.4.0/doc/ext/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.385156 rally-3.4.0/doc/feature_request/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/capture_task_logging.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/check_queue_perfdata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/comparing_results_of_2_tasks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/distributed_load_generation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/explicitly_specify_existing_users_for_scenarios.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/historical_performance_data.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.385156 rally-3.4.0/doc/feature_request/implemented/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/implemented/LDAP_support.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/implemented/add_possibility_to_specify_concurrency_for_tempest.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2361 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/implemented/stop_scenario_after_several_errors.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/installation_script_enhancements.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/installing_isolated.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/launch_specific_benchmark.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/multi_scenarios_load_gen.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/multiple_attach_volume.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/persistence_benchmark_env.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-05-26 08:44:34.000000 rally-3.4.0/doc/feature_request/production_ready_cleanup.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.385156 rally-3.4.0/doc/release_notes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.393159 rally-3.4.0/doc/release_notes/archive/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.0.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.0.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3786 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.0.3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7345 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.0.4.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13260 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.1.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.1.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.1.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22893 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.10.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.10.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10366 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.11.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2904 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.11.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2534 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.11.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.12.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.12.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4818 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.2.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5616 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.3.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.3.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.3.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.3.3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8588 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.4.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13852 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.5.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7624 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.6.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5842 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.7.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10065 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.8.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.8.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5551 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.9.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.9.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v0.9.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive/v1.0.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/archive.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2023-05-26 08:44:34.000000 rally-3.4.0/doc/release_notes/latest.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-05-26 08:44:34.000000 rally-3.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.393159 rally-3.4.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6758 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.361148 rally-3.4.0/doc/source/_templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.393159 rally-3.4.0/doc/source/_templates/openstackrally/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.393159 rally-3.4.0/doc/source/_templates/openstackrally/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/_templates/openstackrally/_static/img.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/_templates/openstackrally/layout.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       27 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/_templates/openstackrally/theme.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/cli_reference.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9577 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2296 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/contribute.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/feature_requests.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.409164 rally-3.4.0/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18652 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Amqp_rpc_single_reply_queue.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64751 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Hook-Aggregated-Report.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    88398 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Hook-Per-Hook-Report.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38695 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Hook-Results.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    95868 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally-Actions.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29546 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally-Plugins.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   127052 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally-UseCases.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   175620 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally_Architecture.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   168071 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally_Distributed_Runner.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105436 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally_QA.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67056 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally_VM_list.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   116187 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally_snapshot_vm.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59267 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Rally_who_is_using.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   118771 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Abort-on-SLA-task-1.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   133861 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Abort-on-SLA-task-2.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   188455 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Collage.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48010 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Multiple-Configurations-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44839 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Multiple-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39473 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40004 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-SLA-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    73756 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-SLA-Scenario.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76785 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Scenario-Atomic.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   111232 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Scenario-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20517 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Actions-durations.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24204 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Distribution.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77249 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Failures.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   103829 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Input-file.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8784 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Load-profile.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101257 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28224 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-SLA.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55099 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Scenario-Data-Aggregated.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25172 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration-profiler.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82653 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20731 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Subtask-configuration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34215 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Task-Total-durations.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74855 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Trends-Atomic-actions.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21142 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Trends-Configuration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25032 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Trends-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    75196 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Trends-Total.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9812 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Trends-single-run.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81001 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Verify-filter-by-status.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    98165 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Verify-for-4-Verifications.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26831 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Verify-toggle-tags.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    84067 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Verify-tracebacks.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   134147 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/images/Report-Verify-xfail.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.409164 rally-3.4.0/doc/source/install_and_upgrade/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/install_and_upgrade/db_migrations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/install_and_upgrade/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1390 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/install_and_upgrade/install.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.409164 rally-3.4.0/doc/source/overview/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4941 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/overview/glossary.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/overview/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6449 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/overview/overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/overview/user_stories.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.409164 rally-3.4.0/doc/source/plugins/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.409164 rally-3.4.0/doc/source/plugins/implementation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4729 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/plugins/implementation/context_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11825 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/plugins/implementation/hook_and_trigger_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/plugins/implementation/runner_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/plugins/implementation/scenario_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/plugins/implementation/sla_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2615 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/plugins/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/plugins/plugin_reference.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.409164 rally-3.4.0/doc/source/project_info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9725 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/project_info/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/project_info/release_notes.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.413165 rally-3.4.0/doc/source/quick_start/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/gates.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.413165 rally-3.4.0/doc/source/quick_start/tutorial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2778 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13823 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9129 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_2_input_task_format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5211 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5731 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10059 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_5_task_templates.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6075 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8178 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_7_working_with_multple_openstack_clouds.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8103 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_8_discovering_more_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45288 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial/step_9_verifying_cloud_via_tempest_verifier.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/quick_start/tutorial.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.413165 rally-3.4.0/doc/source/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10006 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/task/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.413165 rally-3.4.0/doc/source/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/cli_reference.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.417167 rally-3.4.0/doc/source/verification/howto/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3773 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/howto/add_new_reporter.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/howto/add_support_for_new_tool.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/howto/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16640 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/howto/migrate_from_old_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3075 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4254 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/reports.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3626 2023-05-26 08:44:34.000000 rally-3.4.0/doc/source/verification/verifiers.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.417167 rally-3.4.0/doc/specs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.417167 rally-3.4.0/doc/specs/implemented/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2713 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/class-based-scenarios.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4492 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/consistent_resource_names.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10835 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/db_refactoring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6472 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/deployment_type.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7816 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/hook_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/improve_atomic_actions_format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11368 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/improve_scenario_output_format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10567 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/new_rally_input_task_format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/osprofiler.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/pluggable_validators.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1466 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/sla_pd_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/split_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/task_and_verification_export.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30381 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/implemented/verification_refactoring.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/doc/specs/in-progress/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/in-progress/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7564 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/in-progress/cleanup_refactoring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5158 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/in-progress/distributed_runner.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11197 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/in-progress/pluggable-types.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11188 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/in-progress/raas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11465 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/in-progress/refactor_scenario_utils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2023-05-26 08:44:34.000000 rally-3.4.0/doc/specs/template.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.365150 rally-3.4.0/doc/user_stories/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/doc/user_stories/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6391 2023-05-26 08:44:34.000000 rally-3.4.0/doc/user_stories/keystone/authenticate.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/doc/user_stories/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8685 2023-05-26 08:44:34.000000 rally-3.4.0/doc/user_stories/nova/boot_server.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2023-05-26 08:44:34.000000 rally-3.4.0/etc/motd_for_docker
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/etc/rally/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-05-26 08:44:34.000000 rally-3.4.0/etc/rally/rally-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11258 2023-05-26 08:44:34.000000 rally-3.4.0/etc/rally/rally.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4643 2023-05-26 08:44:34.000000 rally-3.4.0/etc/rally.bash_completion
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/rally/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.425169 rally-3.4.0/rally/aas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-26 08:44:34.000000 rally-3.4.0/rally/aas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    54948 2023-05-26 08:44:34.000000 rally-3.4.0/rally/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.425169 rally-3.4.0/rally/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27181 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/cliutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.429170 rally-3.4.0/rally/cli/commands/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/commands/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/commands/db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15083 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/commands/deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13986 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/commands/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4609 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/commands/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37124 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/commands/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40419 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/commands/verify.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6286 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/envutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9054 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/task_results_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2023-05-26 08:44:34.000000 rally-3.4.0/rally/cli/yamlutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.429170 rally-3.4.0/rally/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2699 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/broker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/cfg.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.429170 rally-3.4.0/rally/common/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24554 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.433172 rally-3.4.0/rally/common/db/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.437173 rally-3.4.0/rally/common/db/migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7920 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_01_ca3626f62937_init_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_03_3177d36ea270_merge_credentials_from_users_and_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5678 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_04_4ef544102ba7_change_task_status_enum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15421 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_04_e654a0648db0_refactor_task_results.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2938 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_07_54e844ebfbc3_update_deployment_configs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_08_32fada9b2fde_remove_admin_domain_name.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3700 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_09_08e1515a576c_fix_invalid_verification_logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_09_6ad4f426f005_add_hooks_to_task_result.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7712 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_11_484cd9413e66_new_db_schema_for_verification_component.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2016_12_37fdbb373e8d_fix_test_results_for_verifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_01_a6f364988fc2_change_tag_type_enum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_01_f33f4610dcda_change_verification_statuses.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_02_92aaaa2a6bb3_refactor_credentials.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3450 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_06_35fe16d4ab1c_update_tasks_based_on_workloads.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_06_c517b0011857_fill_missed_workload_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_07_7948b83229f6_workload_min_max_durations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_08_fab4f4f31f8a_fill_missed_workload_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2221 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_09_046a38742e89_port_configs_to_new_formats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_09_e0a5df2c5153_upsize_the_size_of_task_title.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5002 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_10_4394bdc32cfd_fill_missed_workload_info_r3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_10_9a18c6fe265c_rename_namespace_to_platform.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8561 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_10_dc46687661df_update_contexts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2017_12_a43700a813a5_add_env_platforms_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2018_01_44169f4d455e_deleted_worker_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2018_01_7287df262dbc_move_deployment_to_env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2018_02_95208e4eface_add_config_field_to_env_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7918 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2018_02_bc908ac9a1fc_move_deployment_to_env_2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/migrations/versions/2018_02_dc0fe6de6786_update_old_deployment_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11978 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5325 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/sa_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5099 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/db/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/fileutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.437173 rally-3.4.0/rally/common/io/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/io/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5509 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/io/junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9839 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/io/subunit_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11272 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/logging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.437173 rally-3.4.0/rally/common/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/objects/deploy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24513 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/objects/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3248 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/objects/verification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/objects/verifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.437173 rally-3.4.0/rally/common/plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5846 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/plugin/discover.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4372 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/plugin/info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4549 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/plugin/meta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7390 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/plugin/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/sshutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7808 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/streaming_algorithms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26145 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10594 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-05-26 08:44:34.000000 rally-3.4.0/rally/common/yamlutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6911 2023-05-26 08:44:34.000000 rally-3.4.0/rally/consts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.441174 rally-3.4.0/rally/env/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/env/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25830 2023-05-26 08:44:34.000000 rally-3.4.0/rally/env/env_mgr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3978 2023-05-26 08:44:34.000000 rally-3.4.0/rally/env/platform.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6680 2023-05-26 08:44:34.000000 rally-3.4.0/rally/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.441174 rally-3.4.0/rally/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.441174 rally-3.4.0/rally/plugins/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.441174 rally-3.4.0/rally/plugins/common/exporters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.441174 rally-3.4.0/rally/plugins/common/exporters/elastic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/elastic/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      936 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/elastic/client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      940 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/elastic/exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/elastic/flatten.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/html.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/json_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/exporters/trends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.441174 rally-3.4.0/rally/plugins/common/hook/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/hook/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/hook/sys_call.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.441174 rally-3.4.0/rally/plugins/common/hook/triggers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/hook/triggers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/hook/triggers/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/hook/triggers/periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.445176 rally-3.4.0/rally/plugins/common/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/runners/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/runners/constant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/runners/rps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/runners/serial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.445176 rally-3.4.0/rally/plugins/common/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/scenarios/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.445176 rally-3.4.0/rally/plugins/common/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/scenarios/dummy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/scenarios/dummy/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.445176 rally-3.4.0/rally/plugins/common/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/scenarios/requests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/scenarios/requests/http_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/scenarios/requests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.445176 rally-3.4.0/rally/plugins/common/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/sla/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/sla/failure_rate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/sla/iteration_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/sla/max_average_duration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/sla/max_average_duration_per_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/sla/outliers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/sla/performance_degradation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16380 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.445176 rally-3.4.0/rally/plugins/common/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/verification/reporters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/common/verification/testr.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.445176 rally-3.4.0/rally/plugins/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.445176 rally-3.4.0/rally/plugins/task/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/contexts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/contexts/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.449177 rally-3.4.0/rally/plugins/task/exporters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.449177 rally-3.4.0/rally/plugins/task/exporters/elastic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/elastic/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6196 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/elastic/client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16360 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/elastic/exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/elastic/flatten.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/html.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5596 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/json_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3560 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/old_json_results.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1406 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/exporters/trends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.449177 rally-3.4.0/rally/plugins/task/hook_triggers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/hook_triggers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/hook_triggers/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2702 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/hook_triggers/periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.449177 rally-3.4.0/rally/plugins/task/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/hooks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2562 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/hooks/sys_call.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.449177 rally-3.4.0/rally/plugins/task/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/runners/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14074 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/runners/constant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11662 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/runners/rps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3062 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/runners/serial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.449177 rally-3.4.0/rally/plugins/task/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/scenarios/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.449177 rally-3.4.0/rally/plugins/task/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/scenarios/dummy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11367 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/scenarios/dummy/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.453178 rally-3.4.0/rally/plugins/task/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/scenarios/requests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/scenarios/requests/http_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/scenarios/requests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.453178 rally-3.4.0/rally/plugins/task/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/sla/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/sla/failure_rate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/sla/iteration_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/sla/max_average_duration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3150 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/sla/max_average_duration_per_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/sla/outliers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/sla/performance_degradation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/task/types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.453178 rally-3.4.0/rally/plugins/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18676 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/verification/reporters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5791 2023-05-26 08:44:34.000000 rally-3.4.0/rally/plugins/verification/testr.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.457179 rally-3.4.0/rally/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4535 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11493 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21517 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/engine.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3544 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7062 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/functional.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8619 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/hook.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.457179 rally-3.4.0/rally/task/processing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/processing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35108 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/processing/charts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16819 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/processing/plot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3080 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/processing/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9895 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/runner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7474 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/scenario.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14952 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6003 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/sla.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15607 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/task_cfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8847 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2023-05-26 08:44:34.000000 rally-3.4.0/rally/task/validation.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.457179 rally-3.4.0/rally/ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.457179 rally-3.4.0/rally/ui/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2802 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/base.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.457179 rally-3.4.0/rally/ui/templates/ci/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/ci/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2138 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/ci/index_verify.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.461181 rally-3.4.0/rally/ui/templates/libs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/libs/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   124229 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/libs/angular.1.3.3.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   148039 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/libs/d3.3.4.13.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8796 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   188436 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.461181 rally-3.4.0/rally/ui/templates/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10234 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/task/directive_widget.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31337 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/task/report.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17746 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/task/trends.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.461181 rally-3.4.0/rally/ui/templates/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12229 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/templates/verification/report.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2023-05-26 08:44:34.000000 rally-3.4.0/rally/ui/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.461181 rally-3.4.0/rally/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2023-05-26 08:44:34.000000 rally-3.4.0/rally/utils/encodeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10988 2023-05-26 08:44:34.000000 rally-3.4.0/rally/utils/sshutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2023-05-26 08:44:34.000000 rally-3.4.0/rally/utils/strutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.461181 rally-3.4.0/rally/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2023-05-26 08:44:34.000000 rally-3.4.0/rally/verification/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16784 2023-05-26 08:44:34.000000 rally-3.4.0/rally/verification/manager.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3035 2023-05-26 08:44:34.000000 rally-3.4.0/rally/verification/reporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2023-05-26 08:44:34.000000 rally-3.4.0/rally/verification/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/rally-jobs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-05-26 08:44:34.000000 rally-3.4.0/rally-jobs/plugins/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally-jobs/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-05-26 08:44:34.000000 rally-3.4.0/rally-jobs/plugins/fake_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-05-26 08:44:34.000000 rally-3.4.0/rally-jobs/plugins/rally_profile.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.421168 rally-3.4.0/rally-jobs/plugins/test_relative_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/rally-jobs/plugins/test_relative_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2023-05-26 08:44:34.000000 rally-3.4.0/rally-jobs/plugins/test_relative_import/zzz.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11899 2023-05-26 08:44:34.000000 rally-3.4.0/rally-jobs/self-rally.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.425169 rally-3.4.0/rally.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5996 2023-05-26 08:45:05.000000 rally-3.4.0/rally.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25799 2023-05-26 08:45:05.000000 rally-3.4.0/rally.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-26 08:45:05.000000 rally-3.4.0/rally.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-05-26 08:45:05.000000 rally-3.4.0/rally.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-26 08:45:05.000000 rally-3.4.0/rally.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2023-05-26 08:45:05.000000 rally-3.4.0/rally.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-05-26 08:45:05.000000 rally-3.4.0/rally.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2023-05-26 08:45:05.000000 rally-3.4.0/rally.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1496 2023-05-26 08:44:34.000000 rally-3.4.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.461181 rally-3.4.0/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-05-26 08:44:34.000000 rally-3.4.0/samples/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.461181 rally-3.4.0/samples/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.461181 rally-3.4.0/samples/tasks/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/contexts/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/contexts/dummy-context.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/contexts/dummy-context.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.465182 rally-3.4.0/samples/tasks/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.465182 rally-3.4.0/samples/tasks/runners/constant/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/constant/constant-for-duration.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/constant/constant-for-duration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/constant/constant-timeout.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/constant/constant-timeout.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.465182 rally-3.4.0/samples/tasks/runners/rps/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/rps/rps.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/rps/rps.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.465182 rally-3.4.0/samples/tasks/runners/serial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/serial/serial.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/runners/serial/serial.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.465182 rally-3.4.0/samples/tasks/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.469183 rally-3.4.0/samples/tasks/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-exception-probability.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-exception-probability.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-exception.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-exception.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-failure.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-failure.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-output.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-output.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-random-action.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-random-action.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/dummy/dummy.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.469183 rally-3.4.0/samples/tasks/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/requests/check-random-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/requests/check-random-request.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/requests/check-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/scenarios/requests/check-request.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.469183 rally-3.4.0/samples/tasks/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/sla/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/sla/dummy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-05-26 08:44:34.000000 rally-3.4.0/samples/tasks/sla/dummy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2023-05-26 08:45:05.509196 rally-3.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2023-05-26 08:44:34.000000 rally-3.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2023-05-26 08:44:34.000000 rally-3.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.469183 rally-3.4.0/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2023-05-26 08:44:34.000000 rally-3.4.0/tests/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.469183 rally-3.4.0/tests/ci/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:34.000000 rally-3.4.0/tests/ci/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2323 2023-05-26 08:44:34.000000 rally-3.4.0/tests/ci/cover.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.473185 rally-3.4.0/tests/ci/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-26 08:44:34.000000 rally-3.4.0/tests/ci/playbooks/docker-build-and-check.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-05-26 08:44:34.000000 rally-3.4.0/tests/ci/playbooks/docker-build-check-and-push.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-05-26 08:44:34.000000 rally-3.4.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1531 2023-05-26 08:44:34.000000 rally-3.4.0/tests/ci/playbooks/rally-install-pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2023-05-26 08:44:34.000000 rally-3.4.0/tests/ci/playbooks/rally-install-run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.373152 rally-3.4.0/tests/ci/playbooks/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.373152 rally-3.4.0/tests/ci/playbooks/roles/docker-build-image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.473185 rally-3.4.0/tests/ci/playbooks/roles/docker-build-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-05-26 08:44:34.000000 rally-3.4.0/tests/ci/playbooks/roles/docker-build-image/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.473185 rally-3.4.0/tests/ci/playbooks/roles/docker-build-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.373152 rally-3.4.0/tests/ci/playbooks/roles/docker-push-image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.473185 rally-3.4.0/tests/ci/playbooks/roles/docker-push-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/roles/docker-push-image/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.473185 rally-3.4.0/tests/ci/playbooks/roles/docker-push-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.373152 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.473185 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.473185 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/files/find_python_for_tox_env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.473185 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/tasks/install.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/roles/rally-tox/tasks/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/tox-install.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/playbooks/tox-run.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3993 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/pytest_launcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/rally_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4012 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/rally_self_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/render.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13962 2023-05-26 08:44:35.000000 rally-3.4.0/tests/ci/sync_requirements.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.477186 rally-3.4.0/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.477186 rally-3.4.0/tests/functional/extra/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.477186 rally-3.4.0/tests/functional/extra/fake_dir1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/extra/fake_dir1/fake_plugin1.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.477186 rally-3.4.0/tests/functional/extra/fake_dir2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/extra/fake_dir2/fake_plugin2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/extra/fake_platforms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2044 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/extra/fake_verify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/extra/test_fake_scenario.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/test_cli_deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3216 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/test_cli_env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/test_cli_functional.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/test_cli_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58028 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/test_cli_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5542 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/test_cli_verify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/test_lib_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7839 2023-05-26 08:44:35.000000 rally-3.4.0/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.477186 rally-3.4.0/tests/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20461 2023-05-26 08:44:35.000000 rally-3.4.0/tests/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.477186 rally-3.4.0/tests/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/samples/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7006 2023-05-26 08:44:35.000000 rally-3.4.0/tests/samples/test_task_samples.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.481187 rally-3.4.0/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.481187 rally-3.4.0/tests/unit/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.485189 rally-3.4.0/tests/unit/cli/commands/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/commands/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/commands/test_db.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23141 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/commands/test_deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/commands/test_docstrings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21802 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/commands/test_env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/commands/test_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50082 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/commands/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36667 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/commands/test_verify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37060 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/test_cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5589 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/test_envutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9219 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/test_task_results_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/cli/test_yamlutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.485189 rally-3.4.0/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.485189 rally-3.4.0/tests/unit/common/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38662 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/db/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   111129 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/db/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5796 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/db/test_migrations_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5995 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/db/test_types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.489190 rally-3.4.0/tests/unit/common/io/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/io/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3470 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/io/subunit_v2.stream
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2334 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/io/test_junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6267 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/io/test_subunit_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.489190 rally-3.4.0/tests/unit/common/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8664 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/objects/test_deploy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26722 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/objects/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6230 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/objects/test_verification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/objects/test_verifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.489190 rally-3.4.0/tests/unit/common/plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9817 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/plugin/test_discover.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4208 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/plugin/test_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5204 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/plugin/test_meta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/plugin/test_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2822 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/test_broker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12226 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10136 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/test_streaming_algorithms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27264 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6137 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/test_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/common/test_version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.489190 rally-3.4.0/tests/unit/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/doc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/doc/test_docker_readme.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6020 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/doc/test_docstrings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/doc/test_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8647 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/doc/test_jsonschemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4530 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/doc/test_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/doc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.493191 rally-3.4.0/tests/unit/env/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/env/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31964 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/env/test_env_mgr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/env/test_platform.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4637 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.493191 rally-3.4.0/tests/unit/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.493191 rally-3.4.0/tests/unit/plugins/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17384 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/common/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.493191 rally-3.4.0/tests/unit/plugins/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.493191 rally-3.4.0/tests/unit/plugins/task/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/contexts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/contexts/test_dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.493191 rally-3.4.0/tests/unit/plugins/task/exporters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4766 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/dummy_data.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.493191 rally-3.4.0/tests/unit/plugins/task/exporters/elastic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/elastic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8347 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/elastic/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20745 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/elastic/test_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/elastic/test_flatten.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/junit_report.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/test_html.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5144 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/test_json_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/test_junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5414 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/test_old_json_results.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/exporters/test_trends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.497192 rally-3.4.0/tests/unit/plugins/task/hook_triggers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/hook_triggers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2774 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/hook_triggers/test_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3498 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/hook_triggers/test_periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.497192 rally-3.4.0/tests/unit/plugins/task/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/hooks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/hooks/test_sys_call.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.497192 rally-3.4.0/tests/unit/plugins/task/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/runners/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13700 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/runners/test_constant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13691 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/runners/test_rps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2937 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/runners/test_serial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.497192 rally-3.4.0/tests/unit/plugins/task/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/scenarios/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.497192 rally-3.4.0/tests/unit/plugins/task/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/scenarios/dummy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9988 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/scenarios/dummy/test_dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.497192 rally-3.4.0/tests/unit/plugins/task/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/scenarios/requests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/scenarios/requests/test_http_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/scenarios/requests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.497192 rally-3.4.0/tests/unit/plugins/task/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/sla/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4983 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/sla/test_failure_rate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/sla/test_iteration_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/sla/test_max_average_duration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5397 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/sla/test_max_average_duration_per_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5363 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/sla/test_outliers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3428 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/sla/test_performance_degradation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3558 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/task/test_types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.501194 rally-3.4.0/tests/unit/plugins/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/verification/junit_report.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18394 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/verification/test_reporters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17456 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/plugins/verification/test_testr.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.501194 rally-3.4.0/tests/unit/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.505195 rally-3.4.0/tests/unit/task/processing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/processing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47254 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/processing/test_charts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33744 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/processing/test_plot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4654 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/processing/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4935 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13920 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43094 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_functional.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13183 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_hook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9218 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_runner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6440 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_scenario.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9279 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6932 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_sla.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11894 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_task_cfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5377 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23353 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/task/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90112 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_ddt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14649 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12518 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_mock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2569 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_pytest_launcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_test_ddt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14784 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/test_test_mock.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.505195 rally-3.4.0/tests/unit/ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/ui/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/ui/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.505195 rally-3.4.0/tests/unit/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/utils/test_encodeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14089 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/utils/test_sshutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7744 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/utils/test_strutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:45:05.505195 rally-3.4.0/tests/unit/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/verification/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15834 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/verification/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3241 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/verification/test_reporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3837 2023-05-26 08:44:35.000000 rally-3.4.0/tests/unit/verification/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6059 2023-05-26 08:44:35.000000 rally-3.4.0/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2023-05-26 08:44:35.000000 rally-3.4.0/upper-constraints.txt
```

### Comparing `rally-3.3.0/.zuul.d/docker-jobs.yaml` & `rally-3.4.0/.zuul.d/docker-jobs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,25 @@
           UakGoIOovwcV7HpfFHQDijDBz/+6DR4iD+MSbOrG2QRzrjSix9kSk2b7t2liUZ0ODEPWe
           DvlbYngfxXRzxdh/lxQ8AvCXtdRQNYrahyhhCsruBtQTptUgjxnPRe/tZyYAAKXILadZM
           1cA3UecdfuFWhah/ffS1wWC0TvP+UPcJ/dNw3Xlurjt2USJfdyw0MueN7Wsj3Q=
 
 - job:
     name: rally-docker-build
     parent: build-docker-image
-    nodeset: ubuntu-bionic
+    nodeset: ubuntu-jammy
     run: tests/ci/playbooks/docker-build-and-check.yaml
     post-run: tests/ci/playbooks/fetch-html-and-json-reports.yaml
     timeout: 1800
     vars:
       docker_image_version: latest
 
 - job:
     name: rally-docker-build-and-push
     parent: build-docker-image
-    nodeset: ubuntu-bionic
+    nodeset: ubuntu-jammy
     run: tests/ci/playbooks/docker-build-check-and-push.yaml
     post-run: tests/ci/playbooks/fetch-html-and-json-reports.yaml
     timeout: 1800
     secrets:
       name: docker_credentials
       secret: rally-dockerhub-credentials
       pass-to-parent: false
```

### Comparing `rally-3.3.0/.zuul.d/install-jobs.yaml` & `rally-3.4.0/.zuul.d/install-jobs.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,25 @@
     parent: base
     pre-run: tests/ci/playbooks/rally-install-pre.yaml
     run: tests/ci/playbooks/rally-install-run.yaml
     post-run: tests/ci/playbooks/fetch-html-and-json-reports.yaml
     timeout: 1800
 
 - job:
-    name: rally-install-ubuntu-bionic
+    name: rally-install-ubuntu-focal
     parent: rally-install-base
-    nodeset: ubuntu-bionic
+    nodeset: ubuntu-focal
 
 - job:
-    name: rally-install-ubuntu-focal
+    name: rally-install-ubuntu-jammy
     parent: rally-install-base
-    nodeset: ubuntu-focal
+    nodeset: ubuntu-jammy
 
 - job:
-    name: rally-install-centos-7
+    name: rally-install-centos-8s
     parent: rally-install-base
-    nodeset: centos-7
+    nodeset: centos-8-stream
 
 - job:
-    name: rally-install-centos-8
+    name: rally-install-centos-9s
     parent: rally-install-base
-    nodeset: centos-8
+    nodeset: centos-9-stream
```

### Comparing `rally-3.3.0/.zuul.d/python-jobs.yaml` & `rally-3.4.0/.zuul.d/python-jobs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     name: rally-tox-base
     parent: unittests
     pre-run: tests/ci/playbooks/tox-install.yaml
     run: tests/ci/playbooks/tox-run.yaml
     post-run: tests/ci/playbooks/fetch-html-and-json-reports.yaml
     description: |
       Run test for rally project.
-    nodeset: ubuntu-bionic
+    nodeset: ubuntu-jammy
 
 - job:
     name: rally-tox-docs
     parent: rally-tox-base
     description: |
       Run test for rally project.
 
@@ -25,24 +25,14 @@
       Run test for rally project.
 
       Uses tox with the ``self`` environment.
     vars:
       tox_env: pep8
 
 - job:
-    name: rally-tox-functional-py38
-    parent: rally-tox-base
-    description: |
-      Run test for rally project.
-
-      Uses tox with the ``functional`` environment.
-    vars:
-      tox_env: functional-py38
-
-- job:
     name: rally-tox-functional
     parent: rally-tox-base
     description: |
       Run test for rally project.
 
       Uses tox with the ``functional`` environment.
     vars:
@@ -63,35 +53,58 @@
     parent: rally-tox-base
     description: |
       Run unit test for rally project.
 
       Uses tox with the ``py36`` environment.
     vars:
       tox_env: py36
+    nodeset: ubuntu-bionic
 
 - job:
     name: rally-tox-py37
     parent: rally-tox-base
     description: |
       Run unit test for rally project.
 
       Uses tox with the ``py37`` environment.
     vars:
       tox_env: py37
+    nodeset: ubuntu-bionic
 
 - job:
     name: rally-tox-py38
     parent: rally-tox-base
     description: |
       Run unit test for rally project.
 
       Uses tox with the ``py38`` environment.
-    nodeset: ubuntu-focal
     vars:
       tox_env: py38
+    nodeset: ubuntu-focal
+
+- job:
+    name: rally-tox-py39
+    parent: rally-tox-base
+    description: |
+      Run unit test for rally project.
+
+      Uses tox with the ``py39`` environment.
+    vars:
+      tox_env: py39
+    nodeset: ubuntu-focal
+
+- job:
+    name: rally-tox-py310
+    parent: rally-tox-base
+    description: |
+      Run unit test for rally project.
+
+      Uses tox with the ``py310`` environment.
+    vars:
+      tox_env: py310
 
 - job:
     name: rally-tox-samples
     parent: rally-tox-base
     description: |
       Run unit test for rally project.
 
@@ -102,11 +115,10 @@
 - job:
     name: rally-tox-cover
     parent: tox-cover
     description: |
       Run test for rally project.
 
       Uses tox with the ``cover`` environment.
-    nodeset: ubuntu-bionic
     vars:
       coverage_output_src: '{{ zuul.project.src_dir }}/cover/'
       zuul_executor_dest: '{{ zuul.executor.log_root }}/coverage/'
```

### Comparing `rally-3.3.0/.zuul.d/zuul.yaml` & `rally-3.4.0/.zuul.d/zuul.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -8,37 +8,40 @@
       jobs:
         - rally-tox-cover
         - rally-tox-docs
         - rally-tox-pep8
         - rally-tox-py36
         - rally-tox-py37
         - rally-tox-py38
+        - rally-tox-py39
+        - rally-tox-py310
         - rally-tox-samples
         - rally-tox-functional
-        - rally-tox-functional-py38
         - rally-tox-self
-        - rally-install-ubuntu-bionic
         - rally-install-ubuntu-focal
-        - rally-install-centos-7
-        - rally-install-centos-8
+        - rally-install-ubuntu-jammy
+        - rally-install-centos-8s
+        - rally-install-centos-9s
         - rally-docker-build
     gate:
       jobs:
         - rally-tox-cover
         - rally-tox-docs
         - rally-tox-pep8
         - rally-tox-py36
         - rally-tox-py37
         - rally-tox-py38
+        - rally-tox-py39
+        - rally-tox-py310
         - rally-tox-functional
         - rally-tox-self
-        - rally-install-ubuntu-bionic
         - rally-install-ubuntu-focal
-        - rally-install-centos-7
-        - rally-install-centos-8
+        - rally-install-ubuntu-jammy
+        - rally-install-centos-8s
+        - rally-install-centos-9s
     post:
       jobs:
         - rally-docker-build-and-push:
             vars:
               docker_image_version: latest
     release:
       jobs:
```

### Comparing `rally-3.3.0/AUTHORS` & `rally-3.4.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 DeepaJon <deepak.os31@yahoo.com>
 Dina Belova <dbelova@mirantis.com>
 Dmitrii Shcherbakov <dmitrii.shcherbakov@canonical.com>
 Dmitriy Uvarenkov <duvarenkov@mirantis.com>
 Dmitry Ratushnyy <dratushn@cisco.com>
 Doug Hellmann <doug.hellmann@dreamhost.com>
 Doug Hellmann <doug@doughellmann.com>
+Dr. Jens Harbott <harbott@osism.tech>
 Duncan Thomas <duncan.thomas@hp.com>
 Edgar Magana <emagana@gmail.com>
 Egor Tolmachev <etolmachev@mirantis.com>
 Endre Karlson <endre.karlson@hp.com>
 Evgeniy <ekonstantinov@mirantis.com>
 Evgeny Ivanov <eivanov@mirantis.com>
 Evgeny Sikachev <esikachev@mirantis.com>
@@ -165,14 +166,15 @@
 Kun Huang <gareth@openstacker.org>
 Kyle Jorgensen <kyle.jorgensen@workday.com>
 LIU Yulong <liuyulong@le.com>
 Lee Yarwood <lyarwood@redhat.com>
 Li Ma <skywalker.nick@gmail.com>
 Li Tianqing <jazeltq@163.com>
 Li, Chen <chen.li@intel.com>
+LiZekun <2954674728@qq.com>
 Lianhao Lu <lianhao.lu@intel.com>
 Linda Wang <wangwulin@hotmail.com>
 Linda Wang <wangwulin@huawei.com>
 Lingxian Kong <konglingxian@huawei.com>
 LingxianKong <konglingxian@huawei.com>
 Liping Mao <limao@cisco.com>
 LipingMao <limao@cisco.com>
@@ -279,14 +281,15 @@
 Steve Heyman <steve.heyman@rackspace.com>
 Steve Wilkerson <sw5822@att.com>
 Subhash Dasyam <sd@wanclouds.net>
 Sumant Murke <sumant.murke@intel.com>
 Sunil Mamillapalli <sunil_mamillapalli@persistent.co.in>
 Swapnil Kulkarni <coolsvap@redhat.com>
 Swapnil Kulkarni <me@coolsvap.net>
+Takashi Kajinami <tkajinam@redhat.com>
 Takashi NATSUME <natsume.takashi@lab.ntt.co.jp>
 Takeaki Matsumoto <takeaki.matsumoto@ntt.com>
 Takyuki Mitsui <tkyk.mitsui@gmail.com>
 Tetsuo Nakamura <t-nakamura@bit-isle.co.jp>
 Thobias Salazar Trevisan <thobiast@gmail.com>
 Thomas Bechtold <tbechtold@suse.com>
 Timothy R. Chavez <timrchavez@us.ibm.com>
@@ -447,14 +450,15 @@
 wangfaxin <wangfaxin@inspur.com>
 wangqiangbj <wangqiangbj@inspur.com>
 wangxf <wangxf@awcloud.com>
 xiaozhuangqing <zhuangqing.xiao@easystack.cn>
 xuchao <xu.chao@99cloud.net>
 yanyanhu <yanyanhu@cn.ibm.com>
 yaohelan <yaohelan@huawei.com>
+yatinkarel <ykarel@redhat.com>
 yuhui_inspur <yuhui@inspur.com>
 yuli <yuli.stremovsky@huawei.com>
 yuriy_n <ynesenenko@mirantis.com>
 yuyafei <yu.yafei@zte.com.cn>
 zhangdaolong <zhangdaolong@fiberhome.com>
 zhangdelong <zhangdelong@cmss.chinamobile.com>
 zhanghao <zhang.hao16@zte.com.cn>
```

### Comparing `rally-3.3.0/CHANGELOG.rst` & `rally-3.4.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,52 @@
     - **Deprecated** for soon-to-be removed features/plugins.
     - **Removed** for now removed features/plugins.
     - **Fixed** for any bug fixes.
 
 .. Release notes for existing releases are MUTABLE! If there is something that
    was missed or can be improved, feel free to change it!
 
-[3.3.0] - 2021-06-16
+[3.4.0] - 2023-05-23
 --------------------
 
+This is the last release with support of Python 3.6 and Python 3.7
+
+Fixed
+~~~~~
+
+* rally.utils.sshutils.SSH.execute leaves fifo files.
+
+  `Launchpad-bug #1956956 <https://launchpad.net/bugs/1956956>`_
+
 Changed
+~~~~~~~
+
+`xrally/xrally docker image <https://hub.docker.com/r/xrally/xrally>`_ switched
+to use python3.9-slim as a base image instead of ubuntu 20.04.
+
+Added
 ~~~~~
 
+* Pin SQLAlchemy to <2.0.0
+* CI for running unit and functional tests using python 3.10
+* CI jobs that check Rally installation compatibility with CentOS 9 Stream and
+  Ubuntu Jammy
+
+Removed
+~~~~~~~
+
+* CI jobs with installation compatibility checks for CentOS 7, CentOS 8
+  (CentOS 8 Stream is checked instead), Ubuntu Bionic.
+
+[3.3.0] - 2021-06-16
+--------------------
+
+Changed
+~~~~~~~
+
 * ``rally verify`` returns 0 on success, 1, 2 or 3 depending on detected issue.
 
 * Switch docker image from ubuntu 18.04 to ubuntu 20.04
 
 * Move from Freenode to OFTC irc network
 
 Removed
```

### Comparing `rally-3.3.0/CONTRIBUTING.rst` & `rally-3.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/ChangeLog` & `rally-3.4.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 CHANGES
 =======
 
+3.4.0
+-----
+
+* Propose rally 3.4.0 release
+* Update requirements and upper-constraints.txt
+* Use official python docker images
+* Keep CI up-to-date
+* Re-enable tox cover zuul job
+* Pin SQLAlchemy to <2.0.0
+* remove unicode literal from code
+* Suppress deprecation warning from docutils
+* Fix CI issues
+* [ci] Update used nodesets
+* Call pip install tox differently
+* [ci] force reinstall of pip
+* Close stringio objects at sshutils
+* Update doc to do not refer to old installation script
+* Add rally-tox-py39 job
+* Replace deprecated inspect.getargspec
+* Moving IRC network reference to OFTC
+
 3.3.0
 -----
 
 * Fix contribute page
 * Prepare for a new release 3.3.0
 * Update installation guide
 * Update requirements
```

### Comparing `rally-3.3.0/DOCKER_README.md` & `rally-3.4.0/DOCKER_README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # What is Rally/xRally
 
 Rally is tool & framework that allows one to write simple plugins and combine
 them in complex tests scenarios that allows to perform all kinds of testing!
 
 # The purpose of xrally image or how to use it
 
-**xrally** image bases on the latest LTS release of *ubuntu* which is 20.04 at
-the moment. It provides raw xrally framework with only in-tree plugins (no
+**xrally** image bases on the official python3.9-slim docker image.
+It provides raw xrally framework with only in-tree plugins (no
 pre-installed plugins for Kubernetes, OpenStack, etc).
 
 You can use this image as a base image and extend it with installation of
 additional plugins:
 
     # It is an example of Dockerfile for xrally/xrally_docker image. There are
     #   only 2 critical lines: `FROM instruction` and the last line is a check
     #   for rally user is used.
     #
     # Tags of the image are the same as releases of xRally/Rally
-    FROM xrally/xrally:3.3.0
+    FROM xrally/xrally:3.4.0
     
     # "rally" user (which is selected by-default) is owner of "/rally" directory,
     #   so there is no need to call chown or switch the user
     COPY . /rally/xrally_docker
     WORKDIR /rally/xrally_docker
     
     # to install package system-wide, we need to temporary switch to root user
@@ -36,16 +36,16 @@
 details)
 
 # How to run xrally container
 
 First, you need to pull the container. We suggest using the last tagged 
 version:
 
-    # pull the 3.3.0 image (the latest release at the point of writing the note)
-    $ docker pull xrally/xrally:3.3.0
+    # pull the 3.4.0 image (the latest release at the point of writing the note)
+    $ docker pull xrally/xrally:3.4.0
 
 **WARNING: never attach folders and volumes to `/rally` inside the container. It can break everything.**
 
 The default configuration file is located at `/etc/rally/rally.conf`. You
 should not be aware of it. If you want to override some options, use
 `/home/rally/.rally/rally.conf` location instead. Rally does not load all
 configuration files, so the primary one will be used.
@@ -53,15 +53,15 @@
 The default place for rally database file is `/home/rally/.rally/rally.sqlite`.
 To make the storage persistent across all container runs, you may want to use
 docker volumes or mount the directory.
 
 * use docker volumes. It is the easiest way. You just need to do something like:
 
       $ docker volume create --name rally_volume
-      $ docker run -v rally_volume:/home/rally/.rally xrally/xrally:3.3.0 env create --name "foo"
+      $ docker run -v rally_volume:/home/rally/.rally xrally/xrally:3.4.0 env create --name "foo"
 
 
 * mount outer directory inside the container
 
       # you can create directory in whatever you want to place, but you
       # may wish to make the data available for all users
       $ sudo mkdir /var/lib/rally_container
```

### Comparing `rally-3.3.0/Dockerfile` & `rally-3.4.0/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-FROM ubuntu:20.04
+FROM python:3.9-slim
 
-RUN sed -i s/^deb-src.*// /etc/apt/sources.list
-
-RUN apt-get update && apt-get install --yes sudo python3-dev python3-pip vim git-core && \
+RUN apt-get update && apt-get install --yes sudo vim git-core && \
     apt clean && \
-    pip3 --no-cache-dir install --upgrade pip setuptools && \
+    python3 -m pip --no-cache-dir install --upgrade pip setuptools && \
     useradd -u 65500 -m rally && \
     usermod -aG sudo rally && \
     echo "rally ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/00-rally-user && \
     mkdir /rally && chown -R rally:rally /rally
 
 COPY ./ /rally/source
 WORKDIR /rally/source
 
-RUN pip3 install . --constraint upper-constraints.txt --no-cache-dir && \
-    pip3 install pymysql psycopg2-binary --no-cache-dir && \
+RUN python3 -m pip install . --constraint upper-constraints.txt --no-cache-dir && \
+    python3 -m pip install pymysql psycopg2-binary --no-cache-dir && \
     mkdir -p /etc/rally && \
     echo "[database]" > /etc/rally/rally.conf && \
     echo "connection=sqlite:////home/rally/.rally/rally.db" >> /etc/rally/rally.conf
 
 COPY ./etc/motd_for_docker /etc/motd
 RUN echo '[ ! -z "$TERM" -a -r /etc/motd ] && cat /etc/motd' >> /etc/bash.bashrc
```

### Comparing `rally-3.3.0/LICENSE` & `rally-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/PKG-INFO` & `rally-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rally
-Version: 3.3.0
+Version: 3.4.0
 Summary: Generic Testing Framework & Tool that unifies all types of testing.
 Home-page: https://rally.readthedocs.io/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: =====
         Rally
@@ -131,11 +131,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: test
```

### Comparing `rally-3.3.0/README.rst` & `rally-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/bindep.txt` & `rally-3.4.0/bindep.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,12 +9,11 @@
 libffi48-devel [platform:opensuse]
 libssl-dev [platform:dpkg]
 libxml2-dev [platform:dpkg]
 libxml2-devel [platform:rpm]
 libxslt1-dev [platform:dpkg]
 libxslt-devel [platform:rpm]
 openssl-devel [platform:rpm]
-python-dev [platform:dpkg]
 python3-devel [platform:rpm]
 redhat-rpm-config [platform:rpm !platform:suse]
 iputils-ping [platform:dpkg]
 iputils [platform:rpm]
```

### Comparing `rally-3.3.0/doc/README.rst` & `rally-3.4.0/doc/README.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/ext/cli_reference.py` & `rally-3.4.0/doc/ext/cli_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         elements.extend(utils.make_definition(", ".join(args),
                                               ref, description))
     return elements
 
 
 def get_defaults(func):
     """Return a map of argument:default_value for specified function."""
-    spec = inspect.getargspec(func)
+    spec = inspect.getfullargspec(func)
     if spec.defaults:
         return dict(zip(spec.args[-len(spec.defaults):], spec.defaults))
     return {}
 
 
 def make_command_section(category_name, name, parser):
     section = utils.subcategory("rally %s %s" % (category_name, name))
```

### Comparing `rally-3.3.0/doc/ext/include_vars.py` & `rally-3.4.0/doc/ext/include_vars.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/ext/plugin_reference.py` & `rally-3.4.0/doc/ext/plugin_reference.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/ext/utils.py` & `rally-3.4.0/doc/ext/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/check_queue_perfdata.rst` & `rally-3.4.0/doc/feature_request/check_queue_perfdata.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/explicitly_specify_existing_users_for_scenarios.rst` & `rally-3.4.0/doc/feature_request/explicitly_specify_existing_users_for_scenarios.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/historical_performance_data.rst` & `rally-3.4.0/doc/feature_request/historical_performance_data.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/implemented/LDAP_support.rst` & `rally-3.4.0/doc/feature_request/implemented/LDAP_support.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/implemented/add_possibility_to_specify_concurrency_for_tempest.rst` & `rally-3.4.0/doc/feature_request/implemented/add_possibility_to_specify_concurrency_for_tempest.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/implemented/stop_scenario_after_several_errors.rst` & `rally-3.4.0/doc/feature_request/implemented/stop_scenario_after_several_errors.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/installation_script_enhancements.rst` & `rally-3.4.0/doc/feature_request/installation_script_enhancements.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/installing_isolated.rst` & `rally-3.4.0/doc/feature_request/installing_isolated.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/launch_specific_benchmark.rst` & `rally-3.4.0/doc/feature_request/launch_specific_benchmark.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/multi_scenarios_load_gen.rst` & `rally-3.4.0/doc/feature_request/multi_scenarios_load_gen.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/persistence_benchmark_env.rst` & `rally-3.4.0/doc/feature_request/persistence_benchmark_env.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/feature_request/production_ready_cleanup.rst` & `rally-3.4.0/doc/feature_request/production_ready_cleanup.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.0.1.rst` & `rally-3.4.0/doc/release_notes/archive/v0.0.1.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.0.2.rst` & `rally-3.4.0/doc/release_notes/archive/v0.0.2.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.0.3.rst` & `rally-3.4.0/doc/release_notes/archive/v0.0.3.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.0.4.rst` & `rally-3.4.0/doc/release_notes/archive/v0.0.4.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.1.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.1.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.1.1.rst` & `rally-3.4.0/doc/release_notes/archive/v0.1.1.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.1.2.rst` & `rally-3.4.0/doc/release_notes/archive/v0.1.2.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.10.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.10.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.10.1.rst` & `rally-3.4.0/doc/release_notes/archive/v0.10.1.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.11.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.11.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.11.1.rst` & `rally-3.4.0/doc/release_notes/archive/v0.11.1.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.11.2.rst` & `rally-3.4.0/doc/release_notes/archive/v0.11.2.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.12.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.12.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.12.1.rst` & `rally-3.4.0/doc/release_notes/archive/v0.12.1.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.2.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.2.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.3.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.3.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.3.1.rst` & `rally-3.4.0/doc/release_notes/archive/v0.3.1.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.3.2.rst` & `rally-3.4.0/doc/release_notes/archive/v0.3.2.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.3.3.rst` & `rally-3.4.0/doc/release_notes/archive/v0.3.3.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.4.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.4.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.5.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.5.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.6.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.6.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.7.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.7.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.8.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.8.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.8.1.rst` & `rally-3.4.0/doc/release_notes/archive/v0.8.1.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.9.0.rst` & `rally-3.4.0/doc/release_notes/archive/v0.9.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.9.1.rst` & `rally-3.4.0/doc/release_notes/archive/v0.9.1.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v0.9.2.rst` & `rally-3.4.0/doc/release_notes/archive/v0.9.2.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/archive/v1.0.0.rst` & `rally-3.4.0/doc/release_notes/archive/v1.0.0.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/release_notes/latest.rst` & `rally-3.4.0/doc/release_notes/latest.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/Makefile` & `rally-3.4.0/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/_templates/openstackrally/layout.html` & `rally-3.4.0/doc/source/_templates/openstackrally/layout.html`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 {# Turn off sections "Previous topic" and "Next topic" #}
 {%- block sidebarrel %}{% endblock %}
 
 {% block projectsource %}
     <h3>Contacts</h3>
     <p class="topless" style="color: black">
-        <b>IRC</b> <br /><a href="ircs://irc.freenode.net:6697/#openstack-rally">#openstack-rally</a> channel at FreeNode<br />
+        <b>IRC</b> <br /><a href="ircs://irc.oftc.net:6697/#openstack-rally">#openstack-rally</a> channel at OFTC<br />
         <b>E-mail</b> <br /><a href="mailto:openstack-discuss@lists.openstack.org?subject=[Rally]">openstack-discuss@lists.openstack.org</a> with "[Rally]" tag in subject
     </p>
     <h3>Useful links</h3>
     <ul>
         <li><a href="{{ pathto(master_doc) }}">Documentation</a></li>
         <li><a href="http://rally.readthedocs.org/en/latest/">Documentation at RTD</a></li>
         <li><a href="http://opendev.org/openstack/rally">Source</a></li>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 {%- endblock %} {# Display global toc instead of local #} {%- block sidebartoc
 %}
 **** Contents ****
 {{ toctree() }} {%- endblock %} {# Turn off sections "Previous topic" and "Next
 topic" #} {%- block sidebarrel %}{% endblock %} {% block projectsource %}
 **** Contacts ****
 IRC
-#openstack-rally channel at FreeNode
+#openstack-rally channel at OFTC
 E-mail
 openstack-discuss@lists.openstack.org with "[Rally]" tag in subject
 **** Useful links ****
     * Documentation
     * Documentation_at_RTD
     * Source
     * GitHub_mirror
```

### Comparing `rally-3.3.0/doc/source/conf.py` & `rally-3.4.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 # The encoding of source files.
 # source_encoding = "utf-8-sig"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"Rally"
-copyright = u"%d, OpenStack Foundation" % dt.datetime.now().year
+project = "Rally"
+copyright = "%d, OpenStack Foundation" % dt.datetime.now().year
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 
@@ -235,16 +235,16 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual])
 latex_documents = [
     ("index",
      "%s.tex" % project,
-     u"%s Documentation" % project,
-     u"OpenStack Foundation", "manual"),
+     "%s Documentation" % project,
+     "OpenStack Foundation", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -279,16 +279,16 @@
 
 # -- Options for Texinfo output -----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    ("index", "Rally", u"Rally Documentation",
-     u"Rally Team", "Rally",
+    ("index", "Rally", "Rally Documentation",
+     "Rally Team", "Rally",
      "Testing framework and tool for all kinds of tests",
      "Development"),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
```

### Comparing `rally-3.3.0/doc/source/contribute.rst` & `rally-3.4.0/doc/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/feature_requests.rst` & `rally-3.4.0/doc/source/feature_requests.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Amqp_rpc_single_reply_queue.png` & `rally-3.4.0/doc/source/images/Amqp_rpc_single_reply_queue.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Hook-Aggregated-Report.png` & `rally-3.4.0/doc/source/images/Hook-Aggregated-Report.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Hook-Per-Hook-Report.png` & `rally-3.4.0/doc/source/images/Hook-Per-Hook-Report.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Hook-Results.png` & `rally-3.4.0/doc/source/images/Hook-Results.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally-Actions.png` & `rally-3.4.0/doc/source/images/Rally-Actions.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally-Plugins.png` & `rally-3.4.0/doc/source/images/Rally-Plugins.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally-UseCases.png` & `rally-3.4.0/doc/source/images/Rally-UseCases.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally_Architecture.png` & `rally-3.4.0/doc/source/images/Rally_Architecture.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally_Distributed_Runner.png` & `rally-3.4.0/doc/source/images/Rally_Distributed_Runner.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally_QA.png` & `rally-3.4.0/doc/source/images/Rally_QA.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally_VM_list.png` & `rally-3.4.0/doc/source/images/Rally_VM_list.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally_snapshot_vm.png` & `rally-3.4.0/doc/source/images/Rally_snapshot_vm.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Rally_who_is_using.png` & `rally-3.4.0/doc/source/images/Rally_who_is_using.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Abort-on-SLA-task-1.png` & `rally-3.4.0/doc/source/images/Report-Abort-on-SLA-task-1.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Abort-on-SLA-task-2.png` & `rally-3.4.0/doc/source/images/Report-Abort-on-SLA-task-2.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Collage.png` & `rally-3.4.0/doc/source/images/Report-Collage.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Multiple-Configurations-Overview.png` & `rally-3.4.0/doc/source/images/Report-Multiple-Configurations-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Multiple-Overview.png` & `rally-3.4.0/doc/source/images/Report-Multiple-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Overview.png` & `rally-3.4.0/doc/source/images/Report-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-SLA-Overview.png` & `rally-3.4.0/doc/source/images/Report-SLA-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-SLA-Scenario.png` & `rally-3.4.0/doc/source/images/Report-SLA-Scenario.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Scenario-Atomic.png` & `rally-3.4.0/doc/source/images/Report-Scenario-Atomic.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Scenario-Overview.png` & `rally-3.4.0/doc/source/images/Report-Scenario-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Actions-durations.png` & `rally-3.4.0/doc/source/images/Report-Task-Actions-durations.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Distribution.png` & `rally-3.4.0/doc/source/images/Report-Task-Distribution.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Failures.png` & `rally-3.4.0/doc/source/images/Report-Task-Failures.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Input-file.png` & `rally-3.4.0/doc/source/images/Report-Task-Input-file.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Load-profile.png` & `rally-3.4.0/doc/source/images/Report-Task-Load-profile.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Overview.png` & `rally-3.4.0/doc/source/images/Report-Task-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-SLA.png` & `rally-3.4.0/doc/source/images/Report-Task-SLA.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Scenario-Data-Aggregated.png` & `rally-3.4.0/doc/source/images/Report-Task-Scenario-Data-Aggregated.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration-profiler.png` & `rally-3.4.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration-profiler.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration.png` & `rally-3.4.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Subtask-configuration.png` & `rally-3.4.0/doc/source/images/Report-Task-Subtask-configuration.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Task-Total-durations.png` & `rally-3.4.0/doc/source/images/Report-Task-Total-durations.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Trends-Atomic-actions.png` & `rally-3.4.0/doc/source/images/Report-Trends-Atomic-actions.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Trends-Configuration.png` & `rally-3.4.0/doc/source/images/Report-Trends-Configuration.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Trends-Overview.png` & `rally-3.4.0/doc/source/images/Report-Trends-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Trends-Total.png` & `rally-3.4.0/doc/source/images/Report-Trends-Total.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Trends-single-run.png` & `rally-3.4.0/doc/source/images/Report-Trends-single-run.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Verify-filter-by-status.png` & `rally-3.4.0/doc/source/images/Report-Verify-filter-by-status.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Verify-for-4-Verifications.png` & `rally-3.4.0/doc/source/images/Report-Verify-for-4-Verifications.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Verify-toggle-tags.png` & `rally-3.4.0/doc/source/images/Report-Verify-toggle-tags.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Verify-tracebacks.png` & `rally-3.4.0/doc/source/images/Report-Verify-tracebacks.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/images/Report-Verify-xfail.png` & `rally-3.4.0/doc/source/images/Report-Verify-xfail.png`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/index.rst` & `rally-3.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/install_and_upgrade/db_migrations.rst` & `rally-3.4.0/doc/source/install_and_upgrade/db_migrations.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/install_and_upgrade/index.rst` & `rally-3.4.0/doc/source/install_and_upgrade/index.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/install_and_upgrade/install.rst` & `rally-3.4.0/doc/source/install_and_upgrade/install.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/overview/glossary.rst` & `rally-3.4.0/doc/source/overview/glossary.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ========
 Glossary
 ========
 
 .. warning:: Unfortunately, our glossary is not full, but the Rally
   team is working on improving it.  If you cannot find a definition in
   which you are interested, feel free to ping us via IRC
-  (#openstack-rally channel at Freenode) or via E-Mail
+  (#openstack-rally channel at OFTC) or via E-Mail
   (openstack-discuss@lists.openstack.org with tag [Rally]).
 
 .. contents::
   :depth: 1
   :local:
 
 Common
```

### Comparing `rally-3.3.0/doc/source/overview/index.rst` & `rally-3.4.0/doc/source/overview/index.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/overview/overview.rst` & `rally-3.4.0/doc/source/overview/overview.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/overview/user_stories.rst` & `rally-3.4.0/doc/source/overview/user_stories.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/plugins/implementation/context_plugin.rst` & `rally-3.4.0/doc/source/plugins/implementation/context_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/plugins/implementation/hook_and_trigger_plugins.rst` & `rally-3.4.0/doc/source/plugins/implementation/hook_and_trigger_plugins.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/plugins/implementation/runner_plugin.rst` & `rally-3.4.0/doc/source/plugins/implementation/runner_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/plugins/implementation/scenario_plugin.rst` & `rally-3.4.0/doc/source/plugins/implementation/scenario_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/plugins/implementation/sla_plugin.rst` & `rally-3.4.0/doc/source/plugins/implementation/sla_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/plugins/index.rst` & `rally-3.4.0/doc/source/plugins/index.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/project_info/index.rst` & `rally-3.4.0/doc/source/project_info/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -136,26 +136,26 @@
 Useful links
 ------------
 - `Source code`_
 - `Rally roadmap`_
 - `Project space`_
 - `Bugs`_
 - `Patches on review`_
-- `Meeting logs`_ (server: **irc.freenode.net**, channel:
+- `Meeting logs`_ (server: **irc.oftc.net**, channel:
    **#openstack-meeting**)
-- `IRC logs`_ (server: **irc.freenode.net**, channel: **#openstack-rally**)
+- `IRC logs`_ (server: **irc.oftc.net**, channel: **#openstack-rally**)
 - `Gitter chat`_
 - `Trello board`_
 
 
 Where can I discuss and propose changes?
 ----------------------------------------
-- Our IRC channel: **#openstack-rally** on **irc.freenode.net**;
+- Our IRC channel: **#openstack-rally** on **irc.oftc.net**;
 - Weekly Rally team meeting (in IRC): **#openstack-meeting** on
-  **irc.freenode.net**, held on Mondays at 14:00 UTC;
+  **irc.oftc.net**, held on Mondays at 14:00 UTC;
 - OpenStack mailing list: **openstack-discuss@lists.openstack.org** (see
   `subscription and usage instructions`_);
 - `Rally team on Launchpad`_: Answers/Bugs/Blueprints.
 
 .. _release_notes:
 
 .. include:: release_notes.rst
```

### Comparing `rally-3.3.0/doc/source/project_info/release_notes.rst` & `rally-3.4.0/doc/source/project_info/release_notes.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/gates.rst` & `rally-3.4.0/doc/source/quick_start/gates.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/index.rst` & `rally-3.4.0/doc/source/quick_start/index.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 .. contents::
    :local:
 
 In this demo basic operations in Rally are performed, such as adding
 OpenStack cloud deployment, running task against it and generating report.
 
-It's assumed that you have gone through :ref:`tutorial_step_0_installation` and
+It's assumed that you have gone through :ref:`install` and
 have an already existing OpenStack deployment with Keystone available at
 *<KEYSTONE_AUTH_URL>*.
 
 
 Installing rally-openstack package
 ----------------------------------
 First, you have to provider Rally with `rally-openstack`_ package, to be done
```

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_2_input_task_format.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_2_input_task_format.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_5_task_templates.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_5_task_templates.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_7_working_with_multple_openstack_clouds.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_7_working_with_multple_openstack_clouds.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_8_discovering_more_plugins.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_8_discovering_more_plugins.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial/step_9_verifying_cloud_via_tempest_verifier.rst` & `rally-3.4.0/doc/source/quick_start/tutorial/step_9_verifying_cloud_via_tempest_verifier.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 verification component allows us to simplify work not only with Tempest but
 also with any test frameworks or tools. All you need is to create a plugin for
 your framework or tool, and you will be able to use **'rally verify'**
 interface for it. At this point, Rally supports only one plugin in the
 verification component out of the box - as you might guess, Tempest plugin. In
 this guide, we will show how to use Tempest and Rally together via the updated
 **'rally verify'** interface. We assume that you already have a
-:ref:`Rally installation <tutorial_step_0_installation>` and have already
+:ref:`Rally installation <install>` and have already
 :ref:`registered an OpenStack deployment <tutorial_step_1_setting_up_env_and_running_benchmark_from_samples>`
 in Rally. So, let's get started!
 
 
 Create/delete Tempest verifier
 ------------------------------
```

### Comparing `rally-3.3.0/doc/source/quick_start/tutorial.rst` & `rally-3.4.0/doc/source/quick_start/tutorial.rst`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 more complicated cases.
 
 
 .. toctree::
    :glob:
    :maxdepth: 1
 
-   tutorial/step_0_installation
    tutorial/step_1_setting_up_env_and_running_benchmark_from_samples
    tutorial/step_2_input_task_format
    tutorial/step_3_benchmarking_with_existing_users
    tutorial/step_4_adding_success_criteria_for_benchmarks
    tutorial/step_5_task_templates
    tutorial/step_6_aborting_load_generation_on_sla_failure
    tutorial/step_7_working_with_multple_openstack_clouds
```

### Comparing `rally-3.3.0/doc/source/task/index.rst` & `rally-3.4.0/doc/source/task/index.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/verification/cli_reference.rst` & `rally-3.4.0/doc/source/verification/cli_reference.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/verification/howto/add_new_reporter.rst` & `rally-3.4.0/doc/source/verification/howto/add_new_reporter.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/verification/howto/add_support_for_new_tool.rst` & `rally-3.4.0/doc/source/verification/howto/add_support_for_new_tool.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/verification/howto/migrate_from_old_design.rst` & `rally-3.4.0/doc/source/verification/howto/migrate_from_old_design.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/verification/index.rst` & `rally-3.4.0/doc/source/verification/index.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/verification/overview.rst` & `rally-3.4.0/doc/source/verification/overview.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/verification/reports.rst` & `rally-3.4.0/doc/source/verification/reports.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/source/verification/verifiers.rst` & `rally-3.4.0/doc/source/verification/verifiers.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/README.rst` & `rally-3.4.0/doc/specs/README.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/class-based-scenarios.rst` & `rally-3.4.0/doc/specs/implemented/class-based-scenarios.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/consistent_resource_names.rst` & `rally-3.4.0/doc/specs/implemented/consistent_resource_names.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/db_refactoring.rst` & `rally-3.4.0/doc/specs/implemented/db_refactoring.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/deployment_type.rst` & `rally-3.4.0/doc/specs/implemented/deployment_type.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/hook_plugins.rst` & `rally-3.4.0/doc/specs/implemented/hook_plugins.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/improve_atomic_actions_format.rst` & `rally-3.4.0/doc/specs/implemented/improve_atomic_actions_format.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/improve_scenario_output_format.rst` & `rally-3.4.0/doc/specs/implemented/improve_scenario_output_format.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/new_rally_input_task_format.rst` & `rally-3.4.0/doc/specs/implemented/new_rally_input_task_format.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/osprofiler.rst` & `rally-3.4.0/doc/specs/implemented/osprofiler.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/pluggable_validators.rst` & `rally-3.4.0/doc/specs/implemented/pluggable_validators.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/sla_pd_plugin.rst` & `rally-3.4.0/doc/specs/implemented/sla_pd_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/split_plugins.rst` & `rally-3.4.0/doc/specs/implemented/split_plugins.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/task_and_verification_export.rst` & `rally-3.4.0/doc/specs/implemented/task_and_verification_export.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/implemented/verification_refactoring.rst` & `rally-3.4.0/doc/specs/implemented/verification_refactoring.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/in-progress/cleanup_refactoring.rst` & `rally-3.4.0/doc/specs/in-progress/cleanup_refactoring.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/in-progress/distributed_runner.rst` & `rally-3.4.0/doc/specs/in-progress/distributed_runner.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/in-progress/pluggable-types.rst` & `rally-3.4.0/doc/specs/in-progress/pluggable-types.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/in-progress/raas.rst` & `rally-3.4.0/doc/specs/in-progress/raas.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/in-progress/refactor_scenario_utils.rst` & `rally-3.4.0/doc/specs/in-progress/refactor_scenario_utils.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/specs/template.rst` & `rally-3.4.0/doc/specs/template.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/user_stories/keystone/authenticate.rst` & `rally-3.4.0/doc/user_stories/keystone/authenticate.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/doc/user_stories/nova/boot_server.rst` & `rally-3.4.0/doc/user_stories/nova/boot_server.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/etc/motd_for_docker` & `rally-3.4.0/etc/motd_for_docker`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #                                                                             #
 #  Rally at readthedocs - http://rally.readthedocs.org                        #
 #  How to contribute - http://rally.readthedocs.org/en/latest/contribute.html #
 #  If you have any questions, you can reach the Rally team by:                #
 #    * e-mail - openstack-discuss@lists.openstack.org with tag [Rally] in     #
 #      subject                                                                #
 #    * Gitter - https://gitter.im/xRally/Lobby room                           #
-#    * irc - "#openstack-rally" channel at freenode.net                       #
+#    * irc - "#openstack-rally" channel at oftc.net                           #
 ###############################################################################
```

### Comparing `rally-3.3.0/etc/rally/rally.conf.sample` & `rally-3.4.0/etc/rally/rally.conf.sample`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/etc/rally.bash_completion` & `rally-3.4.0/etc/rally.bash_completion`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/api.py` & `rally-3.4.0/rally/api.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/cliutils.py` & `rally-3.4.0/rally/cli/cliutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -612,19 +612,19 @@
     except ImportError:
         pass
 
     try:
         rapi = api.API(config_args=argv[1:], skip_db_check=True)
     except exceptions.RallyException as e:
         print(e)
-        return(2)
+        return 2
 
     if CONF.category.name == "bash-completion":
         print(_generate_bash_completion_script())
-        return(0)
+        return 0
 
     fn = CONF.category.action_fn
     fn_args = [encodeutils.safe_decode(arg)
                for arg in CONF.category.action_args]
     # api instance always is the first argument
     fn_args.insert(0, rapi)
     fn_kwargs = {}
@@ -648,15 +648,15 @@
         CONF.print_help()
         print("Missing arguments:")
         for missing in e.missing:
             for arg in fn.args:
                 if arg[1].get("dest", "").endswith(missing):
                     print(" " + arg[0][0])
                     break
-        return(1)
+        return 1
 
     try:
         validate_deprecated_args(argv, fn)
 
         # skip db check for db and plugin commands
         if CONF.category.name not in ("db", "plugin"):
             rapi.check_db_revision()
```

### Comparing `rally-3.3.0/rally/cli/commands/db.py` & `rally-3.4.0/rally/cli/commands/db.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/commands/deployment.py` & `rally-3.4.0/rally/cli/commands/deployment.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/commands/env.py` & `rally-3.4.0/rally/cli/commands/env.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/commands/plugin.py` & `rally-3.4.0/rally/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/commands/task.py` & `rally-3.4.0/rally/cli/commands/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,15 @@
 
         if status in consts.TaskStatus:
             filters["status"] = status
         elif status:
             print("Error: Invalid task status '%s'.\nAvailable statuses: %s"
                   % (status, ", ".join(consts.TaskStatus)),
                   file=sys.stderr)
-            return(1)
+            return 1
 
         if not all_deployments:
             filters["deployment"] = deployment
 
         if tags:
             filters["tags"] = tags
```

### Comparing `rally-3.3.0/rally/cli/commands/verify.py` & `rally-3.4.0/rally/cli/commands/verify.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/envutils.py` & `rally-3.4.0/rally/cli/envutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/main.py` & `rally-3.4.0/rally/cli/main.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/task_results_loader.py` & `rally-3.4.0/rally/cli/task_results_loader.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/cli/yamlutils.py` & `rally-3.4.0/rally/cli/yamlutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/broker.py` & `rally-3.4.0/rally/common/broker.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/cfg.py` & `rally-3.4.0/rally/common/cfg.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/__init__.py` & `rally-3.4.0/rally/common/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/alembic.ini` & `rally-3.4.0/rally/common/db/alembic.ini`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/api.py` & `rally-3.4.0/rally/common/db/api.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/README.rst` & `rally-3.4.0/rally/common/db/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/env.py` & `rally-3.4.0/rally/common/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/script.py.mako` & `rally-3.4.0/rally/common/db/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_01_ca3626f62937_init_migration.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_01_ca3626f62937_init_migration.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_03_3177d36ea270_merge_credentials_from_users_and_admin.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_03_3177d36ea270_merge_credentials_from_users_and_admin.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_04_4ef544102ba7_change_task_status_enum.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_04_4ef544102ba7_change_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_04_e654a0648db0_refactor_task_results.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_04_e654a0648db0_refactor_task_results.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_07_54e844ebfbc3_update_deployment_configs.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_07_54e844ebfbc3_update_deployment_configs.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_08_32fada9b2fde_remove_admin_domain_name.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_08_32fada9b2fde_remove_admin_domain_name.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_09_08e1515a576c_fix_invalid_verification_logs.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_09_08e1515a576c_fix_invalid_verification_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,16 @@
 
 
 task_helper = sa.Table(
     "tasks",
     sa.MetaData(),
     sa.Column("id", sa.Integer, primary_key=True, autoincrement=True),
     sa.Column("uuid", sa.String(36), nullable=False),
-    sa.Column("status", sa.Enum(*list(consts.TaskStatus),
-                                name="enum_tasks_status"),
-              default=consts.TaskStatus.INIT, nullable=False),
+    sa.Column("status", sa.String(36), default=consts.TaskStatus.INIT,
+              nullable=False),
     sa.Column("verification_log", sa.Text, default=""),
     sa.Column("tag", sa.String(64), default=""),
     sa.Column("deployment_uuid", sa.String(36), nullable=False)
 )
 
 
 def _make_trace(etype, emsg, raw_trace=None):
```

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_09_6ad4f426f005_add_hooks_to_task_result.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_09_6ad4f426f005_add_hooks_to_task_result.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_11_484cd9413e66_new_db_schema_for_verification_component.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_11_484cd9413e66_new_db_schema_for_verification_component.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2016_12_37fdbb373e8d_fix_test_results_for_verifications.py` & `rally-3.4.0/rally/common/db/migrations/versions/2016_12_37fdbb373e8d_fix_test_results_for_verifications.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_01_a6f364988fc2_change_tag_type_enum.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_01_a6f364988fc2_change_tag_type_enum.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_01_f33f4610dcda_change_verification_statuses.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_01_f33f4610dcda_change_verification_statuses.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_02_92aaaa2a6bb3_refactor_credentials.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_02_92aaaa2a6bb3_refactor_credentials.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_06_35fe16d4ab1c_update_tasks_based_on_workloads.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_06_35fe16d4ab1c_update_tasks_based_on_workloads.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_06_c517b0011857_fill_missed_workload_info.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_06_c517b0011857_fill_missed_workload_info.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_07_7948b83229f6_workload_min_max_durations.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_07_7948b83229f6_workload_min_max_durations.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_08_fab4f4f31f8a_fill_missed_workload_info.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_08_fab4f4f31f8a_fill_missed_workload_info.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_09_046a38742e89_port_configs_to_new_formats.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_09_046a38742e89_port_configs_to_new_formats.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_09_e0a5df2c5153_upsize_the_size_of_task_title.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_09_e0a5df2c5153_upsize_the_size_of_task_title.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_10_4394bdc32cfd_fill_missed_workload_info_r3.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_10_4394bdc32cfd_fill_missed_workload_info_r3.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_10_9a18c6fe265c_rename_namespace_to_platform.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_10_9a18c6fe265c_rename_namespace_to_platform.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_10_dc46687661df_update_contexts.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_10_dc46687661df_update_contexts.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2017_12_a43700a813a5_add_env_platforms_tables.py` & `rally-3.4.0/rally/common/db/migrations/versions/2017_12_a43700a813a5_add_env_platforms_tables.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2018_01_44169f4d455e_deleted_worker_table.py` & `rally-3.4.0/rally/common/db/migrations/versions/2018_01_44169f4d455e_deleted_worker_table.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2018_01_7287df262dbc_move_deployment_to_env.py` & `rally-3.4.0/rally/common/db/migrations/versions/2018_01_7287df262dbc_move_deployment_to_env.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2018_02_95208e4eface_add_config_field_to_env_models.py` & `rally-3.4.0/rally/common/db/migrations/versions/2018_02_95208e4eface_add_config_field_to_env_models.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2018_02_bc908ac9a1fc_move_deployment_to_env_2.py` & `rally-3.4.0/rally/common/db/migrations/versions/2018_02_bc908ac9a1fc_move_deployment_to_env_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 import copy
 import datetime as dt
 import uuid
 
 from alembic import op
 import sqlalchemy as sa
-from sqlalchemy.engine import reflection
 
 from rally.common.db import sa_types
 from rally import exceptions
 
 # revision identifiers, used by Alembic.
 revision = "bc908ac9a1fc"
 down_revision = "dc0fe6de6786"
@@ -123,15 +122,15 @@
     sa.Column("env_uuid", sa.String(36)),
     sa.Column("deployment_uuid", sa.String(36))
 )
 
 
 def upgrade():
     connection = op.get_bind()
-    inspector = reflection.Inspector.from_engine(connection)
+    inspector = sa.inspect(connection)
     if "deployments" not in inspector.get_table_names():
         # 7287df262dbc did not fail. nothing to do
         return
 
     envs = [env["uuid"] for env in connection.execute(envs_helper.select())]
 
     for deployment in connection.execute(deployments_helper.select()):
```

### Comparing `rally-3.3.0/rally/common/db/migrations/versions/2018_02_dc0fe6de6786_update_old_deployment_config.py` & `rally-3.4.0/rally/common/db/migrations/versions/2018_02_dc0fe6de6786_update_old_deployment_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 Revises: 95208e4eface
 Create Date: 2018-02-22 21:02:41.822469
 
 """
 
 from alembic import op
 import sqlalchemy as sa
-from sqlalchemy.engine import reflection
 
 from rally.common.db import sa_types
 from rally import exceptions
 
 # revision identifiers, used by Alembic.
 revision = "dc0fe6de6786"
 down_revision = "95208e4eface"
@@ -40,15 +39,15 @@
     sa.Column("uuid", sa.String(36), nullable=False),
     sa.Column("config", sa_types.MutableJSONEncodedDict()),
 )
 
 
 def upgrade():
     connection = op.get_bind()
-    inspector = reflection.Inspector.from_engine(connection)
+    inspector = sa.inspect(connection)
     if "deployments" not in inspector.get_table_names():
         # 7287df262dbc did not fail. nothing to do
         return
 
     for deployment in connection.execute(deployments_helper.select()):
         config = deployment.config
         if isinstance(config, dict) and (
```

### Comparing `rally-3.3.0/rally/common/db/models.py` & `rally-3.4.0/rally/common/db/models.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/db/sa_types.py` & `rally-3.4.0/rally/common/db/sa_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     timestamps values can be bigger than the limit of Float columns at some
     back-ends (the value will be cropped in such case). Also, using Datetime
     type is not convenient too, since it do not accurate with microseconds.
     """
 
     impl = sa_types.BigInteger
     _coefficient = 1000000.0
+    cache_ok = True
 
     def process_bind_param(self, value, dialect):
         if value is None:
             return None
         return value * self._coefficient
 
     def process_result_value(self, value, dialect):
@@ -53,41 +54,46 @@
 
        MySql can store only 64kb in Text type, and for example in psql or
        sqlite we are able to store more than 1GB. In some cases, like storing
        results of task 64kb is not enough. So this type uses for MySql
        LONGTEXT that allows us to store 4GiB.
     """
 
+    cache_ok = True
+
     def load_dialect_impl(self, dialect):
         if dialect.name == "mysql":
             return dialect.type_descriptor(mysql_types.LONGTEXT)
         else:
             return dialect.type_descriptor(sa_types.Text)
 
 
 class JSONEncodedDict(LongText):
     """Represents an immutable structure as a json-encoded string."""
 
     impl = sa_types.Text
+    cache_ok = True
 
     def process_bind_param(self, value, dialect):
         if value is not None:
             value = json.dumps(value, sort_keys=False)
         return value
 
     def process_result_value(self, value, dialect):
-        if value is not None:
+        if value:
             value = json.loads(
                 value, object_pairs_hook=collections.OrderedDict)
         return value
 
 
 class JSONEncodedList(JSONEncodedDict):
     """Represents an immutable structure as a json-encoded string."""
 
+    cache_ok = True
+
     def process_result_value(self, value, dialect):
         if value is not None:
             value = json.loads(value)
         return value
 
 
 class MutableDict(mutable.Mutable, dict):
@@ -149,15 +155,17 @@
         """Detect list del events and emit change events."""
         list.__delitem__(self, i)
         self.changed()
 
 
 class MutableJSONEncodedList(JSONEncodedList):
     """Represent a mutable structure as a json-encoded string."""
+    cache_ok = True
 
 
 class MutableJSONEncodedDict(JSONEncodedDict):
     """Represent a mutable structure as a json-encoded string."""
+    cache_ok = True
 
 
 MutableDict.associate_with(MutableJSONEncodedDict)
 MutableList.associate_with(MutableJSONEncodedList)
```

### Comparing `rally-3.3.0/rally/common/db/schema.py` & `rally-3.4.0/rally/common/db/schema.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/fileutils.py` & `rally-3.4.0/rally/common/fileutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/io/junit.py` & `rally-3.4.0/rally/common/io/junit.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/io/subunit_v2.py` & `rally-3.4.0/rally/common/io/subunit_v2.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/logging.py` & `rally-3.4.0/rally/common/logging.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/objects/__init__.py` & `rally-3.4.0/rally/common/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/objects/deploy.py` & `rally-3.4.0/rally/common/objects/deploy.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/objects/task.py` & `rally-3.4.0/rally/common/objects/task.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/objects/verification.py` & `rally-3.4.0/rally/common/objects/verification.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/objects/verifier.py` & `rally-3.4.0/rally/common/objects/verifier.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/opts.py` & `rally-3.4.0/rally/common/opts.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/plugin/discover.py` & `rally-3.4.0/rally/common/plugin/discover.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/plugin/info.py` & `rally-3.4.0/rally/common/plugin/info.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/plugin/meta.py` & `rally-3.4.0/rally/common/plugin/meta.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/plugin/plugin.py` & `rally-3.4.0/rally/common/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/sshutils.py` & `rally-3.4.0/rally/common/sshutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/streaming_algorithms.py` & `rally-3.4.0/rally/common/streaming_algorithms.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/utils.py` & `rally-3.4.0/rally/common/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/validation.py` & `rally-3.4.0/rally/common/validation.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/version.py` & `rally-3.4.0/rally/common/version.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/common/yamlutils.py` & `rally-3.4.0/rally/common/yamlutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/consts.py` & `rally-3.4.0/rally/consts.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/env/env_mgr.py` & `rally-3.4.0/rally/env/env_mgr.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/env/platform.py` & `rally-3.4.0/rally/env/platform.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/exceptions.py` & `rally-3.4.0/rally/exceptions.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/__init__.py` & `rally-3.4.0/rally/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/exporters/elastic/client.py` & `rally-3.4.0/rally/plugins/common/exporters/elastic/client.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/exporters/elastic/exporter.py` & `rally-3.4.0/rally/plugins/common/exporters/elastic/exporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/exporters/elastic/flatten.py` & `rally-3.4.0/rally/plugins/common/exporters/elastic/flatten.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/exporters/html.py` & `rally-3.4.0/rally/plugins/common/exporters/html.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/exporters/json_exporter.py` & `rally-3.4.0/rally/plugins/common/exporters/json_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/exporters/junit.py` & `rally-3.4.0/rally/plugins/common/exporters/junit.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/exporters/trends.py` & `rally-3.4.0/rally/plugins/common/exporters/trends.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/hook/sys_call.py` & `rally-3.4.0/rally/plugins/common/hook/sys_call.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/hook/triggers/event.py` & `rally-3.4.0/rally/plugins/common/hook/triggers/event.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/hook/triggers/periodic.py` & `rally-3.4.0/rally/plugins/common/hook/triggers/periodic.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/runners/constant.py` & `rally-3.4.0/rally/plugins/common/runners/constant.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/runners/rps.py` & `rally-3.4.0/rally/plugins/common/runners/rps.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/runners/serial.py` & `rally-3.4.0/rally/plugins/common/runners/serial.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/scenarios/dummy/dummy.py` & `rally-3.4.0/rally/plugins/common/scenarios/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/scenarios/requests/http_requests.py` & `rally-3.4.0/rally/plugins/common/scenarios/requests/http_requests.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/scenarios/requests/utils.py` & `rally-3.4.0/rally/plugins/common/scenarios/requests/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/sla/failure_rate.py` & `rally-3.4.0/rally/plugins/common/sla/failure_rate.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/sla/iteration_time.py` & `rally-3.4.0/rally/plugins/common/sla/iteration_time.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/sla/max_average_duration.py` & `rally-3.4.0/rally/plugins/common/sla/max_average_duration.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/sla/max_average_duration_per_atomic.py` & `rally-3.4.0/rally/plugins/common/sla/max_average_duration_per_atomic.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/sla/outliers.py` & `rally-3.4.0/rally/plugins/common/sla/outliers.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/sla/performance_degradation.py` & `rally-3.4.0/rally/plugins/common/sla/performance_degradation.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/types.py` & `rally-3.4.0/rally/plugins/common/types.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/validators.py` & `rally-3.4.0/rally/plugins/common/validators.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/verification/reporters.py` & `rally-3.4.0/rally/plugins/common/verification/reporters.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/common/verification/testr.py` & `rally-3.4.0/rally/plugins/common/verification/testr.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/contexts/dummy.py` & `rally-3.4.0/rally/plugins/task/contexts/dummy.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/exporters/elastic/client.py` & `rally-3.4.0/rally/plugins/task/exporters/elastic/client.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/exporters/elastic/exporter.py` & `rally-3.4.0/rally/plugins/task/exporters/elastic/exporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/exporters/elastic/flatten.py` & `rally-3.4.0/rally/plugins/task/exporters/elastic/flatten.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/exporters/html.py` & `rally-3.4.0/rally/plugins/task/exporters/html.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/exporters/json_exporter.py` & `rally-3.4.0/rally/plugins/task/exporters/json_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/exporters/junit.py` & `rally-3.4.0/rally/plugins/task/exporters/junit.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/exporters/old_json_results.py` & `rally-3.4.0/rally/plugins/task/exporters/old_json_results.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/exporters/trends.py` & `rally-3.4.0/rally/plugins/task/exporters/trends.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/hook_triggers/event.py` & `rally-3.4.0/rally/plugins/task/hook_triggers/event.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/hook_triggers/periodic.py` & `rally-3.4.0/rally/plugins/task/hook_triggers/periodic.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/hooks/sys_call.py` & `rally-3.4.0/rally/plugins/task/hooks/sys_call.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/runners/constant.py` & `rally-3.4.0/rally/plugins/task/runners/constant.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/runners/rps.py` & `rally-3.4.0/rally/plugins/task/runners/rps.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/runners/serial.py` & `rally-3.4.0/rally/plugins/task/runners/serial.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/scenarios/dummy/dummy.py` & `rally-3.4.0/rally/plugins/task/scenarios/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/scenarios/requests/http_requests.py` & `rally-3.4.0/rally/plugins/task/scenarios/requests/http_requests.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/scenarios/requests/utils.py` & `rally-3.4.0/rally/plugins/task/scenarios/requests/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/sla/failure_rate.py` & `rally-3.4.0/rally/plugins/task/sla/failure_rate.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/sla/iteration_time.py` & `rally-3.4.0/rally/plugins/task/sla/iteration_time.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/sla/max_average_duration.py` & `rally-3.4.0/rally/plugins/task/sla/max_average_duration.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/sla/max_average_duration_per_atomic.py` & `rally-3.4.0/rally/plugins/task/sla/max_average_duration_per_atomic.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/sla/outliers.py` & `rally-3.4.0/rally/plugins/task/sla/outliers.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/sla/performance_degradation.py` & `rally-3.4.0/rally/plugins/task/sla/performance_degradation.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/task/types.py` & `rally-3.4.0/rally/plugins/task/types.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/verification/reporters.py` & `rally-3.4.0/rally/plugins/verification/reporters.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/plugins/verification/testr.py` & `rally-3.4.0/rally/plugins/verification/testr.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/atomic.py` & `rally-3.4.0/rally/task/atomic.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/context.py` & `rally-3.4.0/rally/task/context.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/engine.py` & `rally-3.4.0/rally/task/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,21 +120,21 @@
                     results_chunk = self.results[:chunk_size]
                     self.results = self.results[chunk_size:]
                     results_chunk.sort(key=lambda x: x["timestamp"])
                     self.workload.add_workload_data(self.workload_data_count,
                                                     {"raw": results_chunk})
                     self.workload_data_count += 1
 
-            elif self.is_done.isSet():
+            elif self.is_done.is_set():
                 break
             else:
                 time.sleep(0.1)
 
     def _consume_events(self):
-        while not self.is_done.isSet() or self.runner.event_queue:
+        while not self.is_done.is_set() or self.runner.event_queue:
             if self.runner.event_queue:
                 event = self.runner.event_queue.popleft()
                 self.hook_executor.on_event(
                     event_type=event["type"], value=event["value"])
             else:
                 time.sleep(0.01)
 
@@ -197,15 +197,15 @@
     def wait_and_abort(self):
         """Waits until abort signal is received and aborts runner in this case.
 
         Has to be run from different thread simultaneously with the
         runner.run method.
         """
 
-        while not self.is_done.isSet():
+        while not self.is_done.is_set():
             if self.is_task_in_aborting_status(self.task["uuid"],
                                                check_soft=False):
                 self.runner.abort()
                 self.task.update_status(consts.TaskStatus.ABORTED)
                 break
             time.sleep(2.0)
```

### Comparing `rally-3.3.0/rally/task/exporter.py` & `rally-3.4.0/rally/task/exporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/functional.py` & `rally-3.4.0/rally/task/functional.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/hook.py` & `rally-3.4.0/rally/task/hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
         It generates events with type "time" to inform HookExecutor
         about how many time passed since beginning of the first iteration.
         """
         stopwatch = rutils.Stopwatch(stop_event=self._timer_stop_event)
         stopwatch.start()
         seconds_since_start = 0
-        while not self._timer_stop_event.isSet():
+        while not self._timer_stop_event.is_set():
             self.on_event(event_type="time", value=seconds_since_start)
             seconds_since_start += 1
             stopwatch.sleep(seconds_since_start)
 
     def _start_timer(self):
         self._timer_thread.start()
```

### Comparing `rally-3.3.0/rally/task/processing/charts.py` & `rally-3.4.0/rally/task/processing/charts.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/processing/plot.py` & `rally-3.4.0/rally/task/processing/plot.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/processing/utils.py` & `rally-3.4.0/rally/task/processing/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/runner.py` & `rally-3.4.0/rally/task/runner.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/scenario.py` & `rally-3.4.0/rally/task/scenario.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/service.py` & `rally-3.4.0/rally/task/service.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/sla.py` & `rally-3.4.0/rally/task/sla.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/task_cfg.py` & `rally-3.4.0/rally/task/task_cfg.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/types.py` & `rally-3.4.0/rally/task/types.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/utils.py` & `rally-3.4.0/rally/task/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/task/validation.py` & `rally-3.4.0/rally/task/validation.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/base.html` & `rally-3.4.0/rally/ui/templates/base.html`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/ci/index.html` & `rally-3.4.0/rally/ui/templates/ci/index.html`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/ci/index_verify.html` & `rally-3.4.0/rally/ui/templates/ci/index_verify.html`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/libs/angular.1.3.3.min.js` & `rally-3.4.0/rally/ui/templates/libs/angular.1.3.3.min.js`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/libs/d3.3.4.13.min.js` & `rally-3.4.0/rally/ui/templates/libs/d3.3.4.13.min.js`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.css` & `rally-3.4.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.css`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.js` & `rally-3.4.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.js`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/task/directive_widget.js` & `rally-3.4.0/rally/ui/templates/task/directive_widget.js`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/task/report.html` & `rally-3.4.0/rally/ui/templates/task/report.html`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/task/trends.html` & `rally-3.4.0/rally/ui/templates/task/trends.html`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/templates/verification/report.html` & `rally-3.4.0/rally/ui/templates/verification/report.html`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/ui/utils.py` & `rally-3.4.0/rally/ui/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/utils/encodeutils.py` & `rally-3.4.0/rally/utils/encodeutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/utils/sshutils.py` & `rally-3.4.0/rally/utils/sshutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Execute command and get output:
 
     ssh = sshclient.SSH("root", "example.com", port=33)
     status, stdout, stderr = ssh.execute("ps ax")
     if status:
         raise Exception("Command failed with non-zero status.")
-    print stdout.splitlines()
+    print(stdout.splitlines())
 
 Execute command with huge output:
 
     class PseudoFile(object):
         def write(chunk):
             if "error" in chunk:
                 email_admin(chunk)
@@ -153,20 +153,26 @@
                                 then exception will be raised if non-zero code.
         :param timeout:         Timeout in seconds for command execution.
                                 Default 1 hour. No timeout if set to 0.
         """
 
         client = self._get_client()
 
+        should_close_stdin = False
         if isinstance(stdin, str):
             stdin = io.StringIO(stdin)
+            should_close_stdin = True
 
-        return self._run(client, cmd, stdin=stdin, stdout=stdout,
-                         stderr=stderr, raise_on_error=raise_on_error,
-                         timeout=timeout)
+        try:
+            return self._run(client, cmd, stdin=stdin, stdout=stdout,
+                             stderr=stderr, raise_on_error=raise_on_error,
+                             timeout=timeout)
+        finally:
+            if should_close_stdin:
+                stdin.close()
 
     def _run(self, client, cmd, stdin=None, stdout=None, stderr=None,
              raise_on_error=True, timeout=3600):
 
         if isinstance(cmd, (list, tuple)):
             cmd = " ".join(shlex.quote(str(p)) for p in cmd)
 
@@ -242,23 +248,23 @@
 
         :param cmd:     Command to be executed, can be a list.
         :param stdin:   Open file to be sent on process stdin.
         :param timeout: Timeout for execution of the command.
 
         :returns: tuple (exit_status, stdout, stderr)
         """
-        stdout = io.StringIO()
-        stderr = io.StringIO()
+        with io.StringIO() as stdout:
+            with io.StringIO() as stderr:
 
-        exit_status, data = self.run(cmd, stderr=stderr, stdout=stdout,
-                                     stdin=stdin, timeout=timeout,
-                                     raise_on_error=False)
-        stdout.seek(0)
-        stderr.seek(0)
-        return (exit_status, stdout.read(), stderr.read())
+                exit_status, data = self.run(cmd, stderr=stderr, stdout=stdout,
+                                             stdin=stdin, timeout=timeout,
+                                             raise_on_error=False)
+                stdout.seek(0)
+                stderr.seek(0)
+                return exit_status, stdout.read(), stderr.read()
 
     def wait(self, timeout=120, interval=1):
         """Wait for the host will be available via ssh."""
         start_time = time.time()
         while True:
             try:
                 return self.execute("uname")
```

### Comparing `rally-3.3.0/rally/utils/strutils.py` & `rally-3.4.0/rally/utils/strutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/verification/context.py` & `rally-3.4.0/rally/verification/context.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/verification/manager.py` & `rally-3.4.0/rally/verification/manager.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/verification/reporter.py` & `rally-3.4.0/rally/verification/reporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally/verification/utils.py` & `rally-3.4.0/rally/verification/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally-jobs/plugins/fake_plugin.py` & `rally-3.4.0/rally-jobs/plugins/fake_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally-jobs/plugins/rally_profile.py` & `rally-3.4.0/rally-jobs/plugins/rally_profile.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally-jobs/plugins/test_relative_import/zzz.py` & `rally-3.4.0/rally-jobs/plugins/test_relative_import/zzz.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally-jobs/self-rally.yaml` & `rally-3.4.0/rally-jobs/self-rally.yaml`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/rally.egg-info/PKG-INFO` & `rally-3.4.0/rally.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rally
-Version: 3.3.0
+Version: 3.4.0
 Summary: Generic Testing Framework & Tool that unifies all types of testing.
 Home-page: https://rally.readthedocs.io/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: =====
         Rally
@@ -131,11 +131,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: test
```

### Comparing `rally-3.3.0/rally.egg-info/SOURCES.txt` & `rally-3.4.0/rally.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,14 @@
 doc/source/plugins/implementation/sla_plugin.rst
 doc/source/project_info/index.rst
 doc/source/project_info/release_notes
 doc/source/project_info/release_notes.rst
 doc/source/quick_start/gates.rst
 doc/source/quick_start/index.rst
 doc/source/quick_start/tutorial.rst
-doc/source/quick_start/tutorial/step_0_installation.rst
 doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst
 doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst
 doc/source/quick_start/tutorial/step_2_input_task_format.rst
 doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst
 doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst
 doc/source/quick_start/tutorial/step_5_task_templates.rst
 doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst
@@ -472,14 +471,19 @@
 tests/ci/playbooks/rally-install-run.yaml
 tests/ci/playbooks/tox-install.yaml
 tests/ci/playbooks/tox-run.yaml
 tests/ci/playbooks/roles/docker-build-image/defaults/main.yaml
 tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml
 tests/ci/playbooks/roles/docker-push-image/defaults/main.yaml
 tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml
+tests/ci/playbooks/roles/rally-tox/defaults/main.yaml
+tests/ci/playbooks/roles/rally-tox/files/find_python_for_tox_env.py
+tests/ci/playbooks/roles/rally-tox/tasks/install.yaml
+tests/ci/playbooks/roles/rally-tox/tasks/main.yaml
+tests/ci/playbooks/roles/rally-tox/tasks/run.yaml
 tests/functional/__init__.py
 tests/functional/test_cli_deployment.py
 tests/functional/test_cli_env.py
 tests/functional/test_cli_functional.py
 tests/functional/test_cli_plugin.py
 tests/functional/test_cli_task.py
 tests/functional/test_cli_verify.py
```

### Comparing `rally-3.3.0/requirements.txt` & `rally-3.4.0/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 Jinja2                                                 # BSD-3-Clause
 jsonschema                                             # MIT
 markupsafe                                             # BSD-3-Clause
 oslo.config!=4.3.0,!=4.4.0                             # Apache Software License
 # do not forget to remove `testresources` from test-requirements. it is a
 # dependency of oslo.db for tests
 oslo.db                                                # Apache Software License
-oslo.log!=3.44.2,!=4.1.2,!=4.2.0                       # Apache Software License
-paramiko                                               # LGPL
+oslo.log!=3.44.2,!=4.1.2,!=4.2.0,!=5.0.1,!=5.0.2,!=5.1.0  # Apache Software License
+paramiko!=2.9.0,!=2.9.1                                # LGPL
 pbr!=2.1.0                                             # Apache Software License
-PrettyTable                                            # BSD (3 clause)
+PrettyTable!=3.4.0                                     # BSD (3 clause)
 pyOpenSSL                                              # Apache License, Version 2.0
 PyYAML                                                 # MIT
 python-subunit                                         # Apache-2.0 or BSD
 requests!=2.20.0,!=2.24.0                              # Apache License, Version 2.0
-SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8              # MIT
+SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,<2.0.0       # MIT
 virtualenv!=16.3.0                                     # MIT
```

### Comparing `rally-3.3.0/samples/tasks/README.rst` & `rally-3.4.0/samples/tasks/README.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/samples/tasks/scenarios/requests/check-random-request.json` & `rally-3.4.0/samples/tasks/scenarios/requests/check-random-request.json`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/samples/tasks/scenarios/requests/check-request.json` & `rally-3.4.0/samples/tasks/scenarios/requests/check-request.json`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/samples/tasks/sla/dummy.json` & `rally-3.4.0/samples/tasks/sla/dummy.json`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/setup.cfg` & `rally-3.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [files]
 packages = 
 	rally
 data_files = 
 	etc/bash_completion.d =
 	etc/rally.bash_completion
```

### Comparing `rally-3.3.0/setup.py` & `rally-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/test-requirements.txt` & `rally-3.4.0/test-requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 
 hacking>=3.0                                           # Apache Software License
 
 pytest                                                 # MIT
 # py.test plugin for measuring coverage.
-pytest-cov>=2.2.1                                      # MIT
+pytest-cov                                             # MIT
 # py.test plugin for generating HTML reports
 pytest-html                                            # Mozilla Public License 2.0 (MPL 2.0)
 # py.test xdist plugin for distributed testing and loop-on-failing modes
 pytest-xdist                                           # MIT
 
 ddt                                                    # MIT
 testtools                                              # MIT
 
 testresources                                          # UNKNOWN
 
-docutils                                               # public domain, Python, 2-Clause BSD, GPL 3 (see COPYING.txt)
-Pygments                                               # BSD
+docutils<0.18                                          # public domain, Python, 2-Clause BSD, GPL 3 (see COPYING.txt)
+Pygments                                               # BSD-2-Clause
```

### Comparing `rally-3.3.0/tests/README.rst` & `rally-3.4.0/tests/README.rst`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/ci/cover.sh` & `rally-3.4.0/tests/ci/cover.sh`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml` & `rally-3.4.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml` & `rally-3.4.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   when:
    - '"{{ rally_package_name }}" != ""'
    - '"{{ rally_package_name }}" not in rally_version_info.stdout'
 
 - name: "Check availability of {{ rally_plugin_name }} plugin"
   shell: docker run {{ docker_image_tag }} plugin show {{ rally_plugin_name }}
 
-- name: Execute the similar wokrloads as `tox -e self`
+- name: Execute the similar workloads as `tox -e self`
   shell:
     cmd: >
       python3 {{ rally_project_path }}/tests/ci/rally_self_job.py
       --task /rally/source/rally-jobs/self-rally.yaml
       --plugins-path /rally/source/rally-jobs/plugins
       --rally-cmd 'docker run -v '$(realpath {{ zuul.project.src_dir }})'/.test_results:/home/rally/.rally {{ docker_image_tag }}'
       --results-dir /home/rally/.rally
```

### Comparing `rally-3.3.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml` & `rally-3.4.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/ci/pytest_launcher.py` & `rally-3.4.0/tests/ci/pytest_launcher.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/ci/rally_app.py` & `rally-3.4.0/tests/ci/rally_app.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/ci/rally_self_job.py` & `rally-3.4.0/tests/ci/rally_self_job.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/ci/render.py` & `rally-3.4.0/tests/ci/render.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/ci/sync_requirements.py` & `rally-3.4.0/tests/ci/sync_requirements.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/extra/fake_dir1/fake_plugin1.py` & `rally-3.4.0/tests/functional/extra/fake_dir1/fake_plugin1.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/extra/fake_dir2/fake_plugin2.py` & `rally-3.4.0/tests/functional/extra/fake_dir2/fake_plugin2.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/extra/fake_platforms.py` & `rally-3.4.0/tests/functional/extra/fake_platforms.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/extra/fake_verify.py` & `rally-3.4.0/tests/functional/extra/fake_verify.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/test_cli_deployment.py` & `rally-3.4.0/tests/functional/test_cli_deployment.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/test_cli_env.py` & `rally-3.4.0/tests/functional/test_cli_env.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/test_cli_functional.py` & `rally-3.4.0/tests/functional/test_cli_functional.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/test_cli_plugin.py` & `rally-3.4.0/tests/functional/test_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/test_cli_task.py` & `rally-3.4.0/tests/functional/test_cli_task.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/test_cli_verify.py` & `rally-3.4.0/tests/functional/test_cli_verify.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/test_lib_api.py` & `rally-3.4.0/tests/functional/test_lib_api.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/functional/utils.py` & `rally-3.4.0/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/hacking/checks.py` & `rally-3.4.0/tests/hacking/checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,14 @@
  - Keep the test method code in the source file ordered based
    on the N3xx value.
  - List the new rule in the top level HACKING.rst file
  - Add test cases for each new rule to tests/unit/test_hacking.py
 
 """
 
-import functools
 import re
 import tokenize
 
 from hacking import core
 
 re_assert_equal_end_with_true_or_false = re.compile(
     r"assertEqual\(.*?, \s+(True|False)\)$")
@@ -73,53 +72,38 @@
 re_db_import = re.compile(r"^from rally.common import db")
 re_objects_import = re.compile(r"^from rally.common import objects")
 re_old_type_class = re.compile(r"^\s*class \w+(\(\))?:")
 re_datetime_alias = re.compile(r"^(from|import) datetime(?!\s+as\s+dt$)")
 re_log_warn = re.compile(r"(.)*LOG\.(warn)\(\s*('|\"|_)")
 
 
-def skip_ignored_lines(func):
-
-    @functools.wraps(func)
-    def wrapper(physical_line, logical_line, filename):
-        line = physical_line.strip()
-        if not line or line.startswith("#") or line.endswith("# noqa"):
-            return
-        try:
-            for res in func(physical_line, logical_line, filename):
-                yield res
-        except StopIteration:
-            return
-
-    return wrapper
-
-
 def _parse_assert_mock_str(line):
     point = line.find(".assert_")
 
     if point == -1:
         point = line.find(".called_once_with(")
 
     if point != -1:
         end_pos = line[point:].find("(") + point
         return point, line[point + 1: end_pos], line[: point]
     else:
         return None, None, None
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_assert_methods_from_mock(physical_line, logical_line, filename):
+def check_assert_methods_from_mock(logical_line, filename, noqa=False):
     """Ensure that ``assert_*`` methods from ``mock`` library is used correctly
 
     N301 - base error number
     N302 - related to nonexistent "assert_called"
     N303 - related to nonexistent "assert_called_once"
     N304 - related to nonexistent "called_once_with"
     """
+    if noqa:
+        return
 
     correct_names = ["assert_any_call", "assert_called_once_with",
                      "assert_called_with", "assert_has_calls",
                      "assert_not_called"]
     ignored_files = ["./tests/unit/test_hacking.py"]
 
     if filename.startswith("./tests") and filename not in ignored_files:
@@ -157,20 +141,21 @@
                 yield (pos, msg % {
                     "error_number": error_number,
                     "method": method_name,
                     "custom_msg": custom_msg})
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_import_of_logging(physical_line, logical_line, filename):
+def check_import_of_logging(logical_line, filename, noqa=False):
     """Check correctness import of logging module
 
     N310
     """
+    if noqa:
+        return
 
     excluded_files = ["./rally/common/logging.py",
                       "./tests/unit/common/test_logging.py",
                       "./tests/ci/rally_verify.py",
                       "./tests/ci/sync_requirements.py"]
 
     forbidden_imports = ["from oslo_log",
@@ -181,213 +166,221 @@
         for forbidden_import in forbidden_imports:
             if logical_line.startswith(forbidden_import):
                 yield (0, "N310 Wrong module for logging is imported. Please "
                           "use `rally.common.logging` instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_import_of_config(physical_line, logical_line, filename):
+def check_import_of_config(logical_line, filename, noqa=False):
     """Check correctness import of config module
 
     N311
     """
+    if noqa:
+        return
 
     excluded_files = ["./rally/common/cfg.py"]
 
     forbidden_imports = ["from oslo_config",
                          "import oslo_config"]
 
     if filename not in excluded_files:
         for forbidden_import in forbidden_imports:
             if logical_line.startswith(forbidden_import):
                 yield (0, "N311 Wrong module for config is imported. Please "
                           "use `rally.common.cfg` instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def no_use_conf_debug_check(physical_line, logical_line, filename):
+def no_use_conf_debug_check(logical_line, filename, noqa=False):
     """Check for "cfg.CONF.debug"
 
     Rally has two DEBUG level:
      - Full DEBUG, which include all debug-messages from all OpenStack services
      - Rally DEBUG, which include only Rally debug-messages
     so we should use custom check to know debug-mode, instead of CONF.debug
 
     N312
     """
+    if noqa:
+        return
     excluded_files = ["./rally/common/logging.py"]
 
     point = logical_line.find("CONF.debug")
     if point != -1 and filename not in excluded_files:
         yield (point, "N312 Don't use `CONF.debug`. "
                       "Function `rally.common.logging.is_debug` "
                       "should be used instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_true_instance(physical_line, logical_line, filename):
+def assert_true_instance(logical_line, noqa=False):
     """Check for assertTrue(isinstance(a, b)) sentences
 
     N320
     """
+    if noqa:
+        return
     if re_assert_true_instance.match(logical_line):
         yield (0, "N320 assertTrue(isinstance(a, b)) sentences not allowed, "
                   "you should use assertIsInstance(a, b) instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_equal_type(physical_line, logical_line, filename):
+def assert_equal_type(logical_line, noqa=False):
     """Check for assertEqual(type(A), B) sentences
 
     N321
     """
+    if noqa:
+        return
     if re_assert_equal_type.match(logical_line):
         yield (0, "N321 assertEqual(type(A), B) sentences not allowed, "
                   "you should use assertIsInstance(a, b) instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_equal_none(physical_line, logical_line, filename):
+def assert_equal_none(logical_line, noqa=False):
     """Check for assertEqual(A, None) or assertEqual(None, A) sentences
 
     N322
     """
+    if noqa:
+        return
     res = (re_assert_equal_start_with_none.search(logical_line)
            or re_assert_equal_end_with_none.search(logical_line))
     if res:
         yield (0, "N322 assertEqual(A, None) or assertEqual(None, A) "
                   "sentences not allowed, you should use assertIsNone(A) "
                   "instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_true_or_false_with_in(physical_line, logical_line, filename):
+def assert_true_or_false_with_in(logical_line, noqa=False):
     """Check assertTrue/False(A in/not in B) with collection contents
 
     Check for assertTrue/False(A in B), assertTrue/False(A not in B),
     assertTrue/False(A in B, message) or assertTrue/False(A not in B, message)
     sentences.
 
     N323
     """
+    if noqa:
+        return
     res = (re_assert_true_false_with_in_or_not_in.search(logical_line)
            or re_assert_true_false_with_in_or_not_in_spaces.search(
                logical_line))
     if res:
         yield (0, "N323 assertTrue/assertFalse(A in/not in B)sentences not "
                   "allowed, you should use assertIn(A, B) or assertNotIn(A, B)"
                   " instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_equal_in(physical_line, logical_line, filename):
+def assert_equal_in(logical_line, noqa=False):
     """Check assertEqual(A in/not in B, True/False) with collection contents
 
     Check for assertEqual(A in B, True/False), assertEqual(True/False, A in B),
     assertEqual(A not in B, True/False) or assertEqual(True/False, A not in B)
     sentences.
 
     N324
     """
+    if noqa:
+        return
     res = (re_assert_equal_in_end_with_true_or_false.search(logical_line)
            or re_assert_equal_in_start_with_true_or_false.search(logical_line))
     if res:
         yield (0, "N324: Use assertIn/NotIn(A, B) rather than "
                   "assertEqual(A in/not in B, True/False) when checking "
                   "collection contents.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_not_equal_none(physical_line, logical_line, filename):
+def assert_not_equal_none(logical_line, noqa=False):
     """Check for assertNotEqual(A, None) or assertEqual(None, A) sentences
 
     N325
     """
+    if noqa:
+        return
     res = (re_assert_not_equal_start_with_none.search(logical_line)
            or re_assert_not_equal_end_with_none.search(logical_line))
     if res:
         yield (0, "N325 assertNotEqual(A, None) or assertNotEqual(None, A) "
                   "sentences not allowed, you should use assertIsNotNone(A) "
                   "instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def assert_equal_true_or_false(physical_line, logical_line, filename):
+def assert_equal_true_or_false(logical_line, noqa=False):
     """Check for assertEqual(A, True/False) sentences
 
     Check for assertEqual(A, True/False) sentences or
     assertEqual(True/False, A)
 
     N326
     """
+    if noqa:
+        return
     res = (re_assert_equal_end_with_true_or_false.search(logical_line)
            or re_assert_equal_start_with_true_or_false.search(logical_line))
     if res:
         yield (0, "N326 assertEqual(A, True/False) or "
                   "assertEqual(True/False, A) sentences not allowed,"
                   "you should use assertTrue(A) or assertFalse(A) instead.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_no_direct_rally_objects_import(physical_line, logical_line,
-                                         filename):
+def check_no_direct_rally_objects_import(logical_line, filename, noqa=False):
     """Check if rally.common.objects are properly imported.
 
     If you import "from rally.common import objects" you are able to use
     objects directly like objects.Task.
 
     N340
     """
-    if filename == "./rally/common/objects/__init__.py":
+    if noqa:
         return
-
-    if filename == "./rally/common/objects/endpoint.py":
+    if filename == "./rally/common/objects/__init__.py":
         return
 
     if (logical_line.startswith("from rally.common.objects")
        or logical_line.startswith("import rally.common.objects.")):
         yield (0, "N340: Import objects module:"
                   "`from rally.common import objects`. "
                   "After that you can use directly objects e.g. objects.Task")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_no_oslo_deprecated_import(physical_line, logical_line, filename):
+def check_no_oslo_deprecated_import(logical_line, noqa=False):
     """Check if oslo.foo packages are not imported instead of oslo_foo ones.
 
     Libraries from oslo.foo namespace are deprecated because of namespace
     problems.
 
     N341
     """
+    if noqa:
+        return
     if (logical_line.startswith("from oslo.")
        or logical_line.startswith("import oslo.")):
         yield (0, "N341: Import oslo module: `from oslo_xyz import ...`. "
                   "The oslo.xyz namespace was deprecated, use oslo_xyz "
                   "instead")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_quotes(physical_line, logical_line, filename):
+def check_quotes(logical_line, noqa=False):
     """Check that single quotation marks are not used
 
     N350
     """
+    if noqa:
+        return
 
     in_string = False
     in_multiline_string = False
     single_quotas_are_used = False
 
     check_tripple = (
         lambda line, i, char: (
@@ -428,41 +421,37 @@
         i += 1
 
     if single_quotas_are_used:
         yield i, "N350 Remove Single quotes"
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_no_constructor_data_struct(physical_line, logical_line, filename):
+def check_no_constructor_data_struct(logical_line, noqa=False):
     """Check that data structs (lists, dicts) are declared using literals
 
     N351
     """
+    if noqa:
+        return
 
     match = re_no_construct_dict.search(logical_line)
     if match:
         yield 0, "N351 Remove dict() construct and use literal {}"
     match = re_no_construct_list.search(logical_line)
     if match:
         yield 0, "N351 Remove list() construct and use literal []"
 
 
 @core.flake8ext
-def check_dict_formatting_in_string(logical_line, tokens):
+def check_dict_formatting_in_string(logical_line, tokens, noqa=False):
     """Check that strings do not use dict-formatting with a single replacement
 
     N352
     """
-    # NOTE(stpierre): Can't use @skip_ignored_lines here because it's
-    # a stupid decorator that only works on functions that take
-    # (logical_line, filename) as arguments.
-    if (not logical_line
-            or logical_line.startswith("#")
-            or logical_line.endswith("# noqa")):
+    if noqa:
         return
 
     current_string = ""
     in_string = False
     for token_type, text, start, end, line in tokens:
         if token_type == tokenize.STRING:
             if not in_string:
@@ -512,109 +501,100 @@
         else:
             in_string = False
             if token_type == tokenize.NEWLINE:
                 current_string = ""
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_using_unicode(physical_line, logical_line, filename):
-    """Check crosspython unicode usage
-
-    N353
-    """
-
-    if re.search(r"\bunicode\(", logical_line):
-        yield (0, "N353 'unicode' function is absent in python3. Please "
-                  "use 'str' instead.")
-
-
-@core.flake8ext
-def check_raises(physical_line, logical_line, filename):
+def check_raises(logical_line, filename, noqa=False):
     """Check raises usage
 
     N354
     """
+    if noqa:
+        return
 
     ignored_files = ["./tests/unit/test_hacking.py",
                      "./tests/hacking/checks.py"]
     if filename not in ignored_files:
-        if re_raises.search(physical_line):
+        if re_raises.search(logical_line):
             yield (0, "N354 ':Please use ':raises Exception: conditions' "
                       "in docstrings.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_old_type_class(physical_line, logical_line, filename):
+def check_old_type_class(logical_line, noqa=False):
     """Use new-style Python classes
 
     N355
     """
+    if noqa:
+        return
 
     if re_old_type_class.search(logical_line):
         yield (0, "N355 This class does not inherit from anything and thus "
                   "will be an old-style class by default. Try to inherit from "
                   "``object`` or another new-style class.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_datetime_alias(physical_line, logical_line, filename):
+def check_datetime_alias(logical_line, noqa=False):
     """Ensure using ``dt`` as alias for ``datetime``
 
     N356
     """
+    if noqa:
+        return
     if re_datetime_alias.search(logical_line):
         yield 0, "N356 Please use ``dt`` as alias for ``datetime``."
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_db_imports_in_cli(physical_line, logical_line, filename):
+def check_db_imports_in_cli(logical_line, filename, noqa=False):
     """Ensure that CLI modules do not use ``rally.common.db``
 
     N360
     """
+    if noqa:
+        return
     if (not filename.startswith("./rally/cli")
             or filename == "./rally/cli/commands/db.py"):
         return
     if re_db_import.search(logical_line):
         yield (0, "N360 CLI modules do not allow to work with "
                   "`rally.common.db``.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_objects_imports_in_cli(physical_line, logical_line, filename):
+def check_objects_imports_in_cli(logical_line, filename):
     """Ensure that CLI modules do not use ``rally.common.objects``
 
     N361
     """
     if not filename.startswith("./rally/cli"):
         return
     if re_objects_import.search(logical_line):
         yield (0, "N361 CLI modules do not allow to work with "
                   "`rally.common.objects``.")
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_log_warn(physical_line, logical_line, filename):
+def check_log_warn(logical_line):
     if re_log_warn.search(logical_line):
         yield 0, "N313 LOG.warn is deprecated, please use LOG.warning"
 
 
 @core.flake8ext
-@skip_ignored_lines
-def check_opts_import_path(physical_line, logical_line, filename):
+def check_opts_import_path(logical_line, filename, noqa=False):
     """Ensure that we load opts from correct paths only
 
-     N342
-     """
+    N342
+    """
+    if noqa:
+        return
     excluded_files = ["./rally/task/engine.py",
                       "./rally/task/context.py",
                       "./rally/task/scenario.py",
                       "./rally/common/opts.py"]
     forbidden_methods = [".register_opts("]
 
     if filename not in excluded_files:
```

### Comparing `rally-3.3.0/tests/samples/test_task_samples.py` & `rally-3.4.0/tests/samples/test_task_samples.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/commands/test_db.py` & `rally-3.4.0/tests/unit/cli/commands/test_db.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/commands/test_deployment.py` & `rally-3.4.0/tests/unit/cli/commands/test_deployment.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/commands/test_docstrings.py` & `rally-3.4.0/tests/unit/cli/commands/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/commands/test_env.py` & `rally-3.4.0/tests/unit/cli/commands/test_env.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/commands/test_plugin.py` & `rally-3.4.0/tests/unit/cli/commands/test_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/commands/test_task.py` & `rally-3.4.0/tests/unit/cli/commands/test_task.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/commands/test_verify.py` & `rally-3.4.0/tests/unit/cli/commands/test_verify.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/test_cliutils.py` & `rally-3.4.0/tests/unit/cli/test_cliutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/test_envutils.py` & `rally-3.4.0/tests/unit/cli/test_envutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/test_task_results_loader.py` & `rally-3.4.0/tests/unit/cli/test_task_results_loader.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/cli/test_yamlutils.py` & `rally-3.4.0/tests/unit/cli/test_yamlutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/db/test_api.py` & `rally-3.4.0/tests/unit/common/db/test_api.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/db/test_migrations.py` & `rally-3.4.0/tests/unit/common/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/db/test_migrations_base.py` & `rally-3.4.0/tests/unit/common/db/test_migrations_base.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/db/test_types.py` & `rally-3.4.0/tests/unit/common/db/test_types.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/io/subunit_v2.stream` & `rally-3.4.0/tests/unit/common/io/subunit_v2.stream`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/io/test_junit.py` & `rally-3.4.0/tests/unit/common/io/test_junit.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/io/test_subunit_v2.py` & `rally-3.4.0/tests/unit/common/io/test_subunit_v2.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/objects/test_deploy.py` & `rally-3.4.0/tests/unit/common/objects/test_deploy.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/objects/test_task.py` & `rally-3.4.0/tests/unit/common/objects/test_task.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/objects/test_verification.py` & `rally-3.4.0/tests/unit/common/objects/test_verification.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/objects/test_verifier.py` & `rally-3.4.0/tests/unit/common/objects/test_verifier.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/plugin/test_discover.py` & `rally-3.4.0/tests/unit/common/plugin/test_discover.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/plugin/test_info.py` & `rally-3.4.0/tests/unit/common/plugin/test_info.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/plugin/test_meta.py` & `rally-3.4.0/tests/unit/common/plugin/test_meta.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/plugin/test_plugin.py` & `rally-3.4.0/tests/unit/common/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/test_broker.py` & `rally-3.4.0/tests/unit/common/test_broker.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/test_logging.py` & `rally-3.4.0/tests/unit/common/test_logging.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/test_opts.py` & `rally-3.4.0/tests/unit/common/test_opts.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/test_streaming_algorithms.py` & `rally-3.4.0/tests/unit/common/test_streaming_algorithms.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/test_utils.py` & `rally-3.4.0/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/test_validation.py` & `rally-3.4.0/tests/unit/common/test_validation.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/common/test_version.py` & `rally-3.4.0/tests/unit/common/test_version.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/doc/test_docker_readme.py` & `rally-3.4.0/tests/unit/doc/test_docker_readme.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/doc/test_docstrings.py` & `rally-3.4.0/tests/unit/doc/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/doc/test_format.py` & `rally-3.4.0/tests/unit/doc/test_format.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/doc/test_jsonschemas.py` & `rally-3.4.0/tests/unit/doc/test_jsonschemas.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/doc/test_specs.py` & `rally-3.4.0/tests/unit/doc/test_specs.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/doc/utils.py` & `rally-3.4.0/tests/unit/doc/utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/env/test_env_mgr.py` & `rally-3.4.0/tests/unit/env/test_env_mgr.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/env/test_platform.py` & `rally-3.4.0/tests/unit/env/test_platform.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/fakes.py` & `rally-3.4.0/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/common/test_validators.py` & `rally-3.4.0/tests/unit/plugins/common/test_validators.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/contexts/test_dummy.py` & `rally-3.4.0/tests/unit/plugins/task/contexts/test_dummy.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/dummy_data.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/dummy_data.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/elastic/test_client.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/elastic/test_client.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/elastic/test_exporter.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/elastic/test_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/elastic/test_flatten.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/elastic/test_flatten.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/junit_report.xml` & `rally-3.4.0/tests/unit/plugins/task/exporters/junit_report.xml`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/test_html.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/test_html.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/test_json_exporter.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/test_json_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/test_junit.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/test_junit.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/test_old_json_results.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/test_old_json_results.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/exporters/test_trends.py` & `rally-3.4.0/tests/unit/plugins/task/exporters/test_trends.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/hook_triggers/test_event.py` & `rally-3.4.0/tests/unit/plugins/task/hook_triggers/test_event.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/hook_triggers/test_periodic.py` & `rally-3.4.0/tests/unit/plugins/task/hook_triggers/test_periodic.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/hooks/test_sys_call.py` & `rally-3.4.0/tests/unit/plugins/task/hooks/test_sys_call.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/runners/test_constant.py` & `rally-3.4.0/tests/unit/plugins/task/runners/test_constant.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/runners/test_rps.py` & `rally-3.4.0/tests/unit/plugins/task/runners/test_rps.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/runners/test_serial.py` & `rally-3.4.0/tests/unit/plugins/task/runners/test_serial.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/scenarios/dummy/test_dummy.py` & `rally-3.4.0/tests/unit/plugins/task/scenarios/dummy/test_dummy.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/scenarios/requests/test_http_requests.py` & `rally-3.4.0/tests/unit/plugins/task/scenarios/requests/test_http_requests.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/scenarios/requests/test_utils.py` & `rally-3.4.0/tests/unit/plugins/task/scenarios/requests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/sla/test_failure_rate.py` & `rally-3.4.0/tests/unit/plugins/task/sla/test_failure_rate.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/sla/test_iteration_time.py` & `rally-3.4.0/tests/unit/plugins/task/sla/test_iteration_time.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/sla/test_max_average_duration.py` & `rally-3.4.0/tests/unit/plugins/task/sla/test_max_average_duration.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/sla/test_max_average_duration_per_atomic.py` & `rally-3.4.0/tests/unit/plugins/task/sla/test_max_average_duration_per_atomic.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/sla/test_outliers.py` & `rally-3.4.0/tests/unit/plugins/task/sla/test_outliers.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/sla/test_performance_degradation.py` & `rally-3.4.0/tests/unit/plugins/task/sla/test_performance_degradation.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/task/test_types.py` & `rally-3.4.0/tests/unit/plugins/task/test_types.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/verification/junit_report.xml` & `rally-3.4.0/tests/unit/plugins/verification/junit_report.xml`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/verification/test_reporters.py` & `rally-3.4.0/tests/unit/plugins/verification/test_reporters.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/plugins/verification/test_testr.py` & `rally-3.4.0/tests/unit/plugins/verification/test_testr.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/processing/test_charts.py` & `rally-3.4.0/tests/unit/task/processing/test_charts.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/processing/test_plot.py` & `rally-3.4.0/tests/unit/task/processing/test_plot.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/processing/test_utils.py` & `rally-3.4.0/tests/unit/task/processing/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_atomic.py` & `rally-3.4.0/tests/unit/task/test_atomic.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_context.py` & `rally-3.4.0/tests/unit/task/test_context.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_engine.py` & `rally-3.4.0/tests/unit/task/test_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,15 +701,15 @@
     def test_consume_results_abort_manually(self, mock_sla_checker,
                                             mock_event, mock_thread,
                                             mock_task_get_status,
                                             mock_hook_executor):
         runner = mock.MagicMock(result_queue=False)
 
         is_done = mock.MagicMock()
-        is_done.isSet.side_effect = (False, True)
+        is_done.is_set.side_effect = (False, True)
 
         task = mock.MagicMock()
         mock_task_get_status.return_value = consts.TaskStatus.ABORTED
         subtask = mock.Mock(spec=objects.Subtask)
         workload = mock.Mock(spec=objects.Workload)
 
         workload_cfg = {"fake": 2, "hooks": []}
@@ -919,15 +919,15 @@
         subtask = mock.Mock(spec=objects.Subtask)
         workload = mock.Mock(spec=objects.Workload)
         mock_task_get_status.side_effect = (consts.TaskStatus.RUNNING,
                                             consts.TaskStatus.RUNNING,
                                             consts.TaskStatus.ABORTING)
         mock_is_done = mock.MagicMock()
         mock_event.return_value = mock_is_done
-        mock_is_done.isSet.return_value = False
+        mock_is_done.is_set.return_value = False
         ctx_manager = mock.MagicMock()
 
         res = engine.ResultConsumer(workload_cfg, task=task, subtask=subtask,
                                     workload=workload, runner=runner,
                                     abort_on_sla_failure=True,
                                     ctx_manager=ctx_manager)
         res.wait_and_abort()
@@ -950,15 +950,15 @@
         subtask = mock.Mock(spec=objects.Subtask)
         workload = mock.Mock(spec=objects.Workload)
         mock_task_get_status.return_value = consts.TaskStatus.RUNNING
         mock_is_done = mock.MagicMock()
         mock_event.return_value = mock_is_done
         ctx_manager = mock.MagicMock()
 
-        mock_is_done.isSet.side_effect = [False, False, False, False, True]
+        mock_is_done.is_set.side_effect = [False, False, False, False, True]
 
         res = engine.ResultConsumer(workload_cfg, task=task, subtask=subtask,
                                     workload=workload, runner=runner,
                                     abort_on_sla_failure=True,
                                     ctx_manager=ctx_manager)
         res.wait_and_abort()
```

### Comparing `rally-3.3.0/tests/unit/task/test_exporter.py` & `rally-3.4.0/tests/unit/task/test_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_functional.py` & `rally-3.4.0/tests/unit/task/test_functional.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_hook.py` & `rally-3.4.0/tests/unit/task/test_hook.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_runner.py` & `rally-3.4.0/tests/unit/task/test_runner.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_scenario.py` & `rally-3.4.0/tests/unit/task/test_scenario.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_services.py` & `rally-3.4.0/tests/unit/task/test_services.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_sla.py` & `rally-3.4.0/tests/unit/task/test_sla.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_task_cfg.py` & `rally-3.4.0/tests/unit/task/test_task_cfg.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_types.py` & `rally-3.4.0/tests/unit/task/test_types.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/task/test_utils.py` & `rally-3.4.0/tests/unit/task/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test.py` & `rally-3.4.0/tests/unit/test.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test_api.py` & `rally-3.4.0/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test_ddt.py` & `rally-3.4.0/tests/unit/test_ddt.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test_exceptions.py` & `rally-3.4.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test_hacking.py` & `rally-3.4.0/tests/unit/test_hacking.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,114 +6,111 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+import inspect
 import io
 import tokenize
 
 import ddt
 
 from tests.hacking import checks
 from tests.unit import test
 
 
 @ddt.ddt
 class HackingTestCase(test.TestCase):
 
     def _assert_good_samples(self, checker, samples, module_file="f"):
+        spec = inspect.getfullargspec(checker)
+        base_args = {}
+        if "filename" in spec.args:
+            base_args["filename"] = module_file
         for s in samples:
-            self.assertEqual([], list(checker(s, s, module_file)), s)
+            args = {"logical_line": s, **base_args}
+            self.assertEqual([], list(checker(*args)), s)
 
     def _assert_bad_samples(self, checker, samples, module_file="f"):
+        spec = inspect.getfullargspec(checker)
+        base_args = {}
+        if "filename" in spec.args:
+            base_args["filename"] = module_file
+
         for s in samples:
-            self.assertEqual(1, len(list(checker(s, s, module_file))), s)
+            args = {"logical_line": s, **base_args}
+            self.assertEqual(1, len(list(checker(**args))), s)
 
     def test__parse_assert_mock_str(self):
         pos, method, obj = checks._parse_assert_mock_str(
             "mock_clients.fake().quotas.delete.assert_called_once()")
         self.assertEqual("assert_called_once", method)
         self.assertEqual("mock_clients.fake().quotas.delete", obj)
 
     def test__parse_assert_mock_str_no_assert(self):
         pos, method, obj = checks._parse_assert_mock_str(
             "mock_clients.fake().quotas.delete.")
         self.assertIsNone(pos)
         self.assertIsNone(method)
         self.assertIsNone(obj)
 
-    @ddt.data(
-        {"line": "fdafadfdas  # noqa", "result": []},
-        {"line": "  # fdafadfdas", "result": []},
-        {"line": "  ", "result": []},
-        {"line": "otherstuff", "result": [42]}
-    )
-    @ddt.unpack
-    def test_skip_ignored_lines(self, line, result):
-
-        @checks.skip_ignored_lines
-        def any_gen(physical_line, logical_line, file_name):
-            yield 42
-
-        self.assertEqual(result, list(any_gen(line, line, "f")))
-
     def test_correct_usage_of_assert_from_mock(self):
         correct_method_names = ["assert_any_call", "assert_called_once_with",
                                 "assert_called_with", "assert_has_calls"]
         for name in correct_method_names:
             line = "some_mock.%s(asd)" % name
             self.assertEqual(0, len(
                 list(checks.check_assert_methods_from_mock(
                     line, line, "./tests/fake/test"))))
 
     def test_wrong_usage_of_broad_assert_from_mock(self):
         fake_method = "rtfm.assert_something()"
 
         actual_number, actual_msg = next(checks.check_assert_methods_from_mock(
-            fake_method, fake_method, "./tests/fake/test"))
+            fake_method, "./tests/fake/test"))
         self.assertEqual(4, actual_number)
         self.assertTrue(actual_msg.startswith("N301"))
 
     def test_wrong_usage_of_assert_called_from_mock(self):
         fake_method = "rtfm.assert_called()"
 
         actual_number, actual_msg = next(checks.check_assert_methods_from_mock(
-            fake_method, fake_method, "./tests/fake/test"))
+            fake_method, "./tests/fake/test", False))
         self.assertEqual(4, actual_number)
         self.assertTrue(actual_msg.startswith("N302"))
 
     def test_wrong_usage_of_assert_called_once_from_mock(self):
         fake_method = "rtfm.assert_called_once()"
 
         actual_number, actual_msg = next(checks.check_assert_methods_from_mock(
-            fake_method, fake_method, "./tests/fake/test"))
+            fake_method, "./tests/fake/test", False))
         self.assertEqual(4, actual_number)
         self.assertTrue(actual_msg.startswith("N303"))
 
     def test_check_wrong_logging_import(self):
         bad_imports = ["from oslo_log import log",
                        "import oslo_log",
                        "import logging"]
         good_imports = ["from rally.common import logging",
                         "from rally.common.logging",
                         "import rally.common.logging"]
 
         for bad in bad_imports:
-            checkres = checks.check_import_of_logging(bad, bad, "fakefile")
+            checkres = checks.check_import_of_logging(bad, "fakefile")
             self.assertIsNotNone(next(checkres))
 
         for bad in bad_imports:
             checkres = checks.check_import_of_logging(
-                bad, bad, "./rally/common/logging.py")
+                bad, "./rally/common/logging.py")
             self.assertEqual([], list(checkres))
 
         for good in good_imports:
-            checkres = checks.check_import_of_logging(good, good, "fakefile")
+            checkres = checks.check_import_of_logging(good, "fakefile")
             self.assertEqual([], list(checkres))
 
     def test_no_use_conf_debug_check(self):
         bad_samples = [
             "if CONF.debug:",
             "if cfg.CONF.debug"
         ]
@@ -130,54 +127,49 @@
         {
             "line": "self.assertTrue()",
             "result": 0
         }
     )
     @ddt.unpack
     def test_assert_true_instance(self, line, result):
-        self.assertEqual(
-            result, len(list(checks.assert_true_instance(line, line, "f"))))
+        self.assertEqual(result, len(list(checks.assert_true_instance(line))))
 
     @ddt.data(
         {
             "line": "self.assertEqual(type(als['QuicAssist']), list)",
             "result": 1
         },
         {
             "line": "self.assertTrue()",
             "result": 0
         }
     )
     @ddt.unpack
     def test_assert_equal_type(self, line, result):
-        self.assertEqual(result,
-                         len(list(checks.assert_equal_type(line, line, "f"))))
+        self.assertEqual(result, len(list(checks.assert_equal_type(line))))
 
     @ddt.data(
         {"line": "self.assertEqual(A, None)", "result": 1},
         {"line": "self.assertEqual(None, A)", "result": 1},
         {"line": "self.assertIsNone()", "result": 0}
     )
     @ddt.unpack
     def test_assert_equal_none(self, line, result):
 
-        self.assertEqual(result,
-                         len(list(checks.assert_equal_none(line, line, "f"))))
+        self.assertEqual(result, len(list(checks.assert_equal_none(line))))
 
     @ddt.data(
         {"line": "self.assertNotEqual(A, None)", "result": 1},
         {"line": "self.assertNotEqual(None, A)", "result": 1},
         {"line": "self.assertIsNotNone()", "result": 0}
     )
     @ddt.unpack
     def test_assert_not_equal_none(self, line, result):
 
-        self.assertEqual(result,
-                         len(list(checks.assert_not_equal_none(line,
-                                                               line, "f"))))
+        self.assertEqual(result, len(list(checks.assert_not_equal_none(line))))
 
     def test_assert_true_or_false_with_in_or_not_in(self):
         good_lines = [
             "self.assertTrue(any(A > 5 for A in B))",
             "self.assertTrue(any(A > 5 for A in B), 'some message')",
             "self.assertFalse(some in list1 and some2 in list2)"
         ]
@@ -330,75 +322,61 @@
             sample = "print(%s)" % sample
             tokens = tokenize.generate_tokens(
                 io.StringIO(sample).readline)
             self.assertEqual(
                 [],
                 list(checks.check_dict_formatting_in_string(sample, tokens)))
 
-    @ddt.data(
-        "text = unicode('sometext')",
-        "text = process(unicode('sometext'))"
-    )
-    def test_check_using_unicode(self, line):
-
-        checkres = checks.check_using_unicode(line, line, "fakefile")
-        self.assertIsNotNone(next(checkres))
-        self.assertEqual([], list(checkres))
-
     def test_check_raises(self):
         self._assert_bad_samples(
             checks.check_raises,
             ["text = :raises: Exception if conditions"])
 
         self._assert_good_samples(
             checks.check_raises,
             ["text = :raises Exception: if conditions"]
         )
 
     def test_check_db_imports_of_cli(self):
         line = "from rally.common import db"
 
-        next(checks.check_db_imports_in_cli(
-            line, line, "./rally/cli/filename"))
+        next(checks.check_db_imports_in_cli(line, "./rally/cli/filename"))
 
-        checkres = checks.check_db_imports_in_cli(
-            line, line, "./filename")
+        checkres = checks.check_db_imports_in_cli(line, "./filename")
         self.assertRaises(StopIteration, next, checkres)
 
     def test_check_objects_imports_of_cli(self):
         line = "from rally.common import objects"
 
-        next(checks.check_objects_imports_in_cli(
-            line, line, "./rally/cli/filename"))
+        next(checks.check_objects_imports_in_cli(line, "./rally/cli/filename"))
 
-        checkres = checks.check_objects_imports_in_cli(
-            line, line, "./filename")
+        checkres = checks.check_objects_imports_in_cli(line, "./filename")
         self.assertRaises(StopIteration, next, checkres)
 
     @ddt.data(
         "class Oldstype():",
         "class Oldstyle:"
     )
     def test_check_old_type_class(self, line):
-        checkres = checks.check_old_type_class(line, line, "fakefile")
+        checkres = checks.check_old_type_class(line)
         self.assertIsNotNone(next(checkres))
         self.assertEqual([], list(checkres))
 
     def test_check_datetime_alias(self):
         lines = ["import datetime as date",
                  "import datetime",
                  "import datetime as dto",
                  "from datetime import datetime as dtime"]
 
         for line in lines:
-            checkres = checks.check_datetime_alias(line, line, "fakefile")
+            checkres = checks.check_datetime_alias(line)
             self.assertIsNotNone(next(checkres))
             self.assertEqual([], list(checkres))
 
         line = "import datetime as dt"
-        checkres = checks.check_datetime_alias(line, line, "fakefile")
+        checks.check_datetime_alias(line)
 
     def test_check_log_warn(self):
         bad_samples = ["LOG.warn('foo')", "LOG.warn(_('bar'))"]
         self._assert_bad_samples(checks.check_log_warn, bad_samples)
         good_samples = ["LOG.warning('foo')", "LOG.warning(_('bar'))"]
         self._assert_good_samples(checks.check_log_warn, good_samples)
```

### Comparing `rally-3.3.0/tests/unit/test_mock.py` & `rally-3.4.0/tests/unit/test_mock.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test_pytest_launcher.py` & `rally-3.4.0/tests/unit/test_pytest_launcher.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test_resources.py` & `rally-3.4.0/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test_test_ddt.py` & `rally-3.4.0/tests/unit/test_test_ddt.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/test_test_mock.py` & `rally-3.4.0/tests/unit/test_test_mock.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/ui/test_utils.py` & `rally-3.4.0/tests/unit/ui/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/utils/test_encodeutils.py` & `rally-3.4.0/tests/unit/utils/test_encodeutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/utils/test_sshutils.py` & `rally-3.4.0/tests/unit/utils/test_sshutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,30 +124,34 @@
 
     def test_close_context_manager_exit(self):
         with mock.patch.object(self.ssh, "_client") as m_client:
             self.ssh.__exit__()
         m_client.close.assert_called_once_with()
         self.assertFalse(self.ssh._client)
 
-    @mock.patch("rally.utils.sshutils.io.StringIO")
-    def test_execute(self, mock_string_io):
-        mock_string_io.side_effect = stdio = [mock.Mock(), mock.Mock()]
-        stdio[0].read.return_value = "stdout fake data"
-        stdio[1].read.return_value = "stderr fake data"
-        with mock.patch.object(self.ssh, "run") as mock_run:
-            mock_run.return_value = (0, None)
-            status, stdout, stderr = self.ssh.execute("cmd",
-                                                      stdin="fake_stdin",
-                                                      timeout=43)
+    def test_execute(self):
+        stdout_txt = "stdout fake data"
+        stdout_io = io.StringIO(stdout_txt)
+        stderr_txt = "stderr fake data"
+        stderr_io = io.StringIO(stderr_txt)
+
+        with mock.patch("rally.utils.sshutils.io.StringIO") as mock_string_io:
+            mock_string_io.side_effect = [stdout_io, stderr_io]
+            with mock.patch.object(self.ssh, "run") as mock_run:
+                mock_run.return_value = (0, None)
+                status, stdout, stderr = self.ssh.execute("cmd",
+                                                          stdin="fake_stdin",
+                                                          timeout=43)
+
         mock_run.assert_called_once_with(
-            "cmd", stdin="fake_stdin", stdout=stdio[0],
-            stderr=stdio[1], timeout=43, raise_on_error=False)
+            "cmd", stdin="fake_stdin", stdout=stdout_io, stderr=stderr_io,
+            timeout=43, raise_on_error=False)
         self.assertEqual(0, status)
-        self.assertEqual("stdout fake data", stdout)
-        self.assertEqual("stderr fake data", stderr)
+        self.assertEqual(stdout_txt, stdout)
+        self.assertEqual(stderr_txt, stderr)
 
     @mock.patch("rally.utils.sshutils.time")
     def test_wait_timeout(self, mock_time):
         mock_time.time.side_effect = [1, 50, 150]
         self.ssh.execute = mock.Mock(side_effect=[exceptions.SSHError,
                                                   exceptions.SSHError,
                                                   0])
```

### Comparing `rally-3.3.0/tests/unit/utils/test_strutils.py` & `rally-3.4.0/tests/unit/utils/test_strutils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/verification/test_context.py` & `rally-3.4.0/tests/unit/verification/test_context.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/verification/test_manager.py` & `rally-3.4.0/tests/unit/verification/test_manager.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/verification/test_reporter.py` & `rally-3.4.0/tests/unit/verification/test_reporter.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tests/unit/verification/test_utils.py` & `rally-3.4.0/tests/unit/verification/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-3.3.0/tox.ini` & `rally-3.4.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 [tox]
 minversion = 3.2.0
-skipsdist = True
 ignore_basepython_conflict = true
 envlist = py36,py37,py38,pep8,samples
 
 [testenv]
 extras = {env:RALLY_EXTRAS:}
 setenv = VIRTUAL_ENV={envdir}
-         HOME={homedir}
          LANG=en_US.UTF-8
          LANGUAGE=en_US:en
          LC_ALL=C
          PYTHONHASHSEED=0
          TOX_ENV_NAME={envname}
-whitelist_externals = find
+allowlist_externals = find
                       rm
                       make
+                      mkdir
 deps = -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
        -c{toxinidir}/upper-constraints.txt
 usedevelop = True
 commands =
   find . -type f -name "*.pyc" -delete
   python {toxinidir}/tests/ci/pytest_launcher.py tests/unit --posargs={posargs}
 distribute = false
-basepython = python3.6
-passenv = PYTEST_REPORT http_proxy HTTP_PROXY https_proxy HTTPS_PROXY no_proxy NO_PROXY
+basepython = python3
+passenv =
+          PYTEST_REPORT
+          http_proxy
+          HTTP_PROXY
+          https_proxy
+          HTTPS_PROXY
+          no_proxy
+          NO_PROXY
+          HOME
 
 [testenv:pep8]
 commands = flake8
 distribute = false
 
 [testenv:py36]
 basepython = python3.6
 
 [testenv:py37]
 basepython = python3.7
 
 [testenv:py38]
 basepython = python3.8
 
+[testenv:py39]
+basepython = python3.9
+
 [testenv:samples]
 commands =
   find . -type f -name "*.pyc" -delete
   python {toxinidir}/tests/ci/pytest_launcher.py tests/samples --posargs={posargs}
 
 
 [testenv:venv]
@@ -53,25 +63,17 @@
 deps = -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
        stestr
 commands =
   find . -type f -name "*.pyc" -delete
   python {toxinidir}/tests/ci/pytest_launcher.py tests/functional --posargs={posargs}
 
-[testenv:functional-py38]
-deps = -r{toxinidir}/requirements.txt
-       -r{toxinidir}/test-requirements.txt
-       stestr
-basepython = python3.8
-commands =
-  find . -type f -name "*.pyc" -delete
-  python {toxinidir}/tests/ci/pytest_launcher.py tests/functional --posargs={posargs}
-
 [testenv:cover]
 commands = {toxinidir}/tests/ci/cover.sh {posargs}
+allowlist_externals = {toxinidir}/tests/ci/cover.sh
 
 [testenv:docs]
 # min py3.6
 basepython = python3
 deps =
   -c{toxinidir}/upper-constraints.txt
   -r{toxinidir}/doc/requirements.txt
@@ -112,15 +114,14 @@
     N326 = checks:assert_equal_true_or_false
     N340 = checks:check_no_direct_rally_objects_import
     N341 = checks:check_no_oslo_deprecated_import
     N342 = checks:check_opts_import_path
     N350 = checks:check_quotes
     N351 = checks:check_no_constructor_data_struct
     N352 = checks:check_dict_formatting_in_string
-    N353 = checks:check_using_unicode
     N354 = checks:check_raises
     N355 = checks:check_old_type_class
     N356 = checks:check_datetime_alias
     N360 = checks:check_db_imports_in_cli
     N361 = checks:check_objects_imports_in_cli
 paths = ./tests/hacking
 
@@ -145,16 +146,30 @@
   mkdir -p {toxinidir}/.test_results
   python3 {toxinidir}/tests/ci/rally_self_job.py --task {toxinidir}/rally-jobs/self-rally.yaml --plugins-path {toxinidir}/rally-jobs/plugins
 
 [pytest]
 filterwarnings =
     error
     ignore:.*EngineFacade is deprecated; please use oslo_db.sqlalchemy.enginefacade*:
+    # Introduced with oslo.db-12.1.0
+    ignore:.*Support for the MySQL NDB Cluster storage engine has been deprecated and will be removed in a future release.:DeprecationWarning:
+    # Introuduced with SQLAlchemy-1.4.46, can be removed when rally supports SQLAlchemy>=2.0.0
+    ignore:.*Set environment variable SQLALCHEMY_SILENCE_UBER_WARNING=1 to silence this message.*
     # instead of ignoring all modules, let's list only libraries that are failing
     ignore:invalid escape sequence:DeprecationWarning:.*netaddr.*
     ignore:invalid escape sequence:DeprecationWarning:.*prettytable
     ignore:invalid escape sequence:DeprecationWarning:.*subunit.*
     ignore:invalid escape sequence:DeprecationWarning:.*docutils.*
+    # we do not use anything inner from OptionParser, so we do not care about it's parent
+    ignore:The frontend.OptionParser class will be replaced by a subclass of argparse.ArgumentParser in Docutils 0.21 or later.:DeprecationWarning:
+    # we do not use Option directly, it is initialized by OptionParser by itself.
+    # as soon as docutils team get rid of frontend.Option, they will also fix OptionParser
+    ignore: The frontend.Option class will be removed in Docutils 0.21 or later.:DeprecationWarning:
     # python 3.7
     ignore:Using or importing the ABCs:DeprecationWarning:unittest2.*
     # python 3.8
     ignore:::.*netaddr.strategy.*
+    # python 3.10
+    ignore:The distutils package is deprecated and slated for removal in Python 3.12. Use setuptools or check PEP 632 for potential alternatives:DeprecationWarning:
+    ignore:pkg_resources is deprecated as an API:DeprecationWarning:
+    # pytest-cov
+    ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning:
```


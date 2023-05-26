# Comparing `tmp/humanloop-0.4.4.tar.gz` & `tmp/humanloop-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanloop-0.4.4.tar", max compression
+gzip compressed data, was "humanloop-0.4.5.tar", max compression
```

## Comparing `humanloop-0.4.4.tar` & `humanloop-0.4.5.tar`

### file list

```diff
@@ -1,401 +1,410 @@
--rw-r--r--   0        0        0     1081 2023-05-26 00:09:33.462092 humanloop-0.4.4/LICENSE
--rw-r--r--   0        0        0     8475 2023-05-26 00:09:33.509250 humanloop-0.4.4/README.md
--rw-r--r--   0        0        0     1059 2023-05-26 00:09:33.370349 humanloop-0.4.4/humanloop/__init__.py
--rw-r--r--   0        0        0    73009 2023-05-26 00:09:33.370543 humanloop-0.4.4/humanloop/api_client.py
--rw-r--r--   0        0        0      663 2023-05-26 00:09:33.370741 humanloop-0.4.4/humanloop/api_response.py
--rw-r--r--   0        0        0      214 2023-05-26 00:09:33.370909 humanloop-0.4.4/humanloop/apis/__init__.py
--rw-r--r--   0        0        0     4578 2023-05-26 00:09:33.371066 humanloop-0.4.4/humanloop/apis/path_to_api.py
--rw-r--r--   0        0        0      236 2023-05-26 00:09:33.371192 humanloop-0.4.4/humanloop/apis/paths/__init__.py
--rw-r--r--   0        0        0       91 2023-05-26 00:09:33.371287 humanloop-0.4.4/humanloop/apis/paths/chat.py
--rw-r--r--   0        0        0      108 2023-05-26 00:09:33.371416 humanloop-0.4.4/humanloop/apis/paths/chat_deployed.py
--rw-r--r--   0        0        0      112 2023-05-26 00:09:33.371553 humanloop-0.4.4/humanloop/apis/paths/chat_experiment.py
--rw-r--r--   0        0        0      115 2023-05-26 00:09:33.371727 humanloop-0.4.4/humanloop/apis/paths/chat_model_config.py
--rw-r--r--   0        0        0      103 2023-05-26 00:09:33.371884 humanloop-0.4.4/humanloop/apis/paths/completion.py
--rw-r--r--   0        0        0      120 2023-05-26 00:09:33.372030 humanloop-0.4.4/humanloop/apis/paths/completion_deployed.py
--rw-r--r--   0        0        0      124 2023-05-26 00:09:33.372167 humanloop-0.4.4/humanloop/apis/paths/completion_experiment.py
--rw-r--r--   0        0        0      127 2023-05-26 00:09:33.372312 humanloop-0.4.4/humanloop/apis/paths/completion_model_config.py
--rw-r--r--   0        0        0      226 2023-05-26 00:09:33.372517 humanloop-0.4.4/humanloop/apis/paths/experiments_experiment_id.py
--rw-r--r--   0        0        0      152 2023-05-26 00:09:33.372689 humanloop-0.4.4/humanloop/apis/paths/experiments_experiment_id_model_config.py
--rw-r--r--   0        0        0       99 2023-05-26 00:09:33.372846 humanloop-0.4.4/humanloop/apis/paths/feedback.py
--rw-r--r--   0        0        0       91 2023-05-26 00:09:33.373002 humanloop-0.4.4/humanloop/apis/paths/logs.py
--rw-r--r--   0        0        0      108 2023-05-26 00:09:33.373160 humanloop-0.4.4/humanloop/apis/paths/model_configs.py
--rw-r--r--   0        0        0      110 2023-05-26 00:09:33.373327 humanloop-0.4.4/humanloop/apis/paths/model_configs_id.py
--rw-r--r--   0        0        0      165 2023-05-26 00:09:33.373484 humanloop-0.4.4/humanloop/apis/paths/projects.py
--rw-r--r--   0        0        0      176 2023-05-26 00:09:33.373645 humanloop-0.4.4/humanloop/apis/paths/projects_id.py
--rw-r--r--   0        0        0      219 2023-05-26 00:09:33.373795 humanloop-0.4.4/humanloop/apis/paths/projects_id_active_config.py
--rw-r--r--   0        0        0      144 2023-05-26 00:09:33.373947 humanloop-0.4.4/humanloop/apis/paths/projects_id_active_experiment.py
--rw-r--r--   0        0        0      116 2023-05-26 00:09:33.374084 humanloop-0.4.4/humanloop/apis/paths/projects_id_configs.py
--rw-r--r--   0        0        0      117 2023-05-26 00:09:33.374234 humanloop-0.4.4/humanloop/apis/paths/projects_id_export.py
--rw-r--r--   0        0        0      135 2023-05-26 00:09:33.374375 humanloop-0.4.4/humanloop/apis/paths/projects_id_feedback_types.py
--rw-r--r--   0        0        0      231 2023-05-26 00:09:33.374528 humanloop-0.4.4/humanloop/apis/paths/projects_project_id_experiments.py
--rw-r--r--   0        0        0      165 2023-05-26 00:09:33.374683 humanloop-0.4.4/humanloop/apis/paths/sessions.py
--rw-r--r--   0        0        0      101 2023-05-26 00:09:33.375006 humanloop-0.4.4/humanloop/apis/paths/sessions_id.py
--rw-r--r--   0        0        0       95 2023-05-26 00:09:33.375225 humanloop-0.4.4/humanloop/apis/paths/traces.py
--rw-r--r--   0        0        0     1654 2023-05-26 00:09:33.375391 humanloop-0.4.4/humanloop/apis/tag_to_api.py
--rw-r--r--   0        0        0      572 2023-05-26 00:09:33.375554 humanloop-0.4.4/humanloop/apis/tags/__init__.py
--rw-r--r--   0        0        0     1006 2023-05-26 00:09:33.375697 humanloop-0.4.4/humanloop/apis/tags/chats_api.py
--rw-r--r--   0        0        0     1020 2023-05-26 00:09:33.375842 humanloop-0.4.4/humanloop/apis/tags/completions_api.py
--rw-r--r--   0        0        0     1091 2023-05-26 00:09:33.375984 humanloop-0.4.4/humanloop/apis/tags/experiments_api.py
--rw-r--r--   0        0        0      721 2023-05-26 00:09:33.376127 humanloop-0.4.4/humanloop/apis/tags/feedback_api.py
--rw-r--r--   0        0        0      707 2023-05-26 00:09:33.376281 humanloop-0.4.4/humanloop/apis/tags/logs_api.py
--rw-r--r--   0        0        0      803 2023-05-26 00:09:33.376418 humanloop-0.4.4/humanloop/apis/tags/model_configurations_api.py
--rw-r--r--   0        0        0     1486 2023-05-26 00:09:33.376558 humanloop-0.4.4/humanloop/apis/tags/projects_api.py
--rw-r--r--   0        0        0      834 2023-05-26 00:09:33.376707 humanloop-0.4.4/humanloop/apis/tags/sessions_api.py
--rw-r--r--   0        0        0      717 2023-05-26 00:09:33.376890 humanloop-0.4.4/humanloop/apis/tags/traces_api.py
--rw-r--r--   0        0        0    28032 2023-05-26 00:09:33.377102 humanloop-0.4.4/humanloop/client.py
--rw-r--r--   0        0        0    28032 2023-05-26 00:09:33.377363 humanloop-0.4.4/humanloop/client.pyi
--rw-r--r--   0        0        0     6780 2023-05-26 00:09:33.461499 humanloop-0.4.4/humanloop/client_custom.py
--rw-r--r--   0        0        0    18674 2023-05-26 00:09:33.377771 humanloop-0.4.4/humanloop/configuration.py
--rw-r--r--   0        0        0     7678 2023-05-26 00:09:33.377923 humanloop-0.4.4/humanloop/exceptions.py
--rw-r--r--   0        0        0     2274 2023-05-26 00:09:33.378073 humanloop-0.4.4/humanloop/exceptions_base.py
--rw-r--r--   0        0        0      343 2023-05-26 00:09:33.378294 humanloop-0.4.4/humanloop/model/__init__.py
--rw-r--r--   0        0        0     9140 2023-05-26 00:09:33.378430 humanloop-0.4.4/humanloop/model/agent_config_request.py
--rw-r--r--   0        0        0     8975 2023-05-26 00:09:33.378583 humanloop-0.4.4/humanloop/model/agent_config_request.pyi
--rw-r--r--   0        0        0    11140 2023-05-26 00:09:33.378781 humanloop-0.4.4/humanloop/model/agent_config_response.py
--rw-r--r--   0        0        0    11140 2023-05-26 00:09:33.378963 humanloop-0.4.4/humanloop/model/agent_config_response.pyi
--rw-r--r--   0        0        0     6379 2023-05-26 00:09:33.379130 humanloop-0.4.4/humanloop/model/base_metric_response.py
--rw-r--r--   0        0        0     6379 2023-05-26 00:09:33.379267 humanloop-0.4.4/humanloop/model/base_metric_response.pyi
--rw-r--r--   0        0        0     5150 2023-05-26 00:09:33.379404 humanloop-0.4.4/humanloop/model/categorical_feedback_label.py
--rw-r--r--   0        0        0     5150 2023-05-26 00:09:33.379528 humanloop-0.4.4/humanloop/model/categorical_feedback_label.pyi
--rw-r--r--   0        0        0     8957 2023-05-26 00:09:33.379697 humanloop-0.4.4/humanloop/model/chat_data_response.py
--rw-r--r--   0        0        0     8957 2023-05-26 00:09:33.379968 humanloop-0.4.4/humanloop/model/chat_data_response.pyi
--rw-r--r--   0        0        0     9998 2023-05-26 00:09:33.380203 humanloop-0.4.4/humanloop/model/chat_deployed_request.py
--rw-r--r--   0        0        0     9998 2023-05-26 00:09:33.380397 humanloop-0.4.4/humanloop/model/chat_deployed_request.pyi
--rw-r--r--   0        0        0    10659 2023-05-26 00:09:33.380532 humanloop-0.4.4/humanloop/model/chat_experiment_request.py
--rw-r--r--   0        0        0    10659 2023-05-26 00:09:33.380642 humanloop-0.4.4/humanloop/model/chat_experiment_request.pyi
--rw-r--r--   0        0        0     3702 2023-05-26 00:09:33.380742 humanloop-0.4.4/humanloop/model/chat_message.py
--rw-r--r--   0        0        0     3702 2023-05-26 00:09:33.380870 humanloop-0.4.4/humanloop/model/chat_message.pyi
--rw-r--r--   0        0        0    10693 2023-05-26 00:09:33.381686 humanloop-0.4.4/humanloop/model/chat_model_config_request.py
--rw-r--r--   0        0        0    10693 2023-05-26 00:09:33.381926 humanloop-0.4.4/humanloop/model/chat_model_config_request.pyi
--rw-r--r--   0        0        0    12556 2023-05-26 00:09:33.382103 humanloop-0.4.4/humanloop/model/chat_request.py
--rw-r--r--   0        0        0    12556 2023-05-26 00:09:33.382263 humanloop-0.4.4/humanloop/model/chat_request.pyi
--rw-r--r--   0        0        0    11076 2023-05-26 00:09:33.382438 humanloop-0.4.4/humanloop/model/chat_response.py
--rw-r--r--   0        0        0    11076 2023-05-26 00:09:33.382606 humanloop-0.4.4/humanloop/model/chat_response.pyi
--rw-r--r--   0        0        0     1446 2023-05-26 00:09:33.382751 humanloop-0.4.4/humanloop/model/chat_role.py
--rw-r--r--   0        0        0     1285 2023-05-26 00:09:33.382870 humanloop-0.4.4/humanloop/model/chat_role.pyi
--rw-r--r--   0        0        0     9674 2023-05-26 00:09:33.382985 humanloop-0.4.4/humanloop/model/completion_deployed_request.py
--rw-r--r--   0        0        0     9674 2023-05-26 00:09:33.383129 humanloop-0.4.4/humanloop/model/completion_deployed_request.pyi
--rw-r--r--   0        0        0    10340 2023-05-26 00:09:33.383270 humanloop-0.4.4/humanloop/model/completion_experiment_request.py
--rw-r--r--   0        0        0    10340 2023-05-26 00:09:33.383396 humanloop-0.4.4/humanloop/model/completion_experiment_request.pyi
--rw-r--r--   0        0        0    10376 2023-05-26 00:09:33.383699 humanloop-0.4.4/humanloop/model/completion_model_config_request.py
--rw-r--r--   0        0        0    10376 2023-05-26 00:09:33.383857 humanloop-0.4.4/humanloop/model/completion_model_config_request.pyi
--rw-r--r--   0        0        0    12258 2023-05-26 00:09:33.384017 humanloop-0.4.4/humanloop/model/completion_request.py
--rw-r--r--   0        0        0    12258 2023-05-26 00:09:33.384162 humanloop-0.4.4/humanloop/model/completion_request.pyi
--rw-r--r--   0        0        0    11017 2023-05-26 00:09:33.384298 humanloop-0.4.4/humanloop/model/completion_response.py
--rw-r--r--   0        0        0    11017 2023-05-26 00:09:33.384424 humanloop-0.4.4/humanloop/model/completion_response.pyi
--rw-r--r--   0        0        0     2672 2023-05-26 00:09:33.384526 humanloop-0.4.4/humanloop/model/config_response.py
--rw-r--r--   0        0        0     2672 2023-05-26 00:09:33.384626 humanloop-0.4.4/humanloop/model/config_response.pyi
--rw-r--r--   0        0        0     1546 2023-05-26 00:09:33.384720 humanloop-0.4.4/humanloop/model/config_type.py
--rw-r--r--   0        0        0     1361 2023-05-26 00:09:33.384829 humanloop-0.4.4/humanloop/model/config_type.pyi
--rw-r--r--   0        0        0     6196 2023-05-26 00:09:33.384928 humanloop-0.4.4/humanloop/model/create_experiment_request.py
--rw-r--r--   0        0        0     6196 2023-05-26 00:09:33.385040 humanloop-0.4.4/humanloop/model/create_experiment_request.pyi
--rw-r--r--   0        0        0     3199 2023-05-26 00:09:33.385125 humanloop-0.4.4/humanloop/model/create_log_response.py
--rw-r--r--   0        0        0     3199 2023-05-26 00:09:33.385216 humanloop-0.4.4/humanloop/model/create_log_response.pyi
--rw-r--r--   0        0        0     4266 2023-05-26 00:09:33.385300 humanloop-0.4.4/humanloop/model/create_project_request.py
--rw-r--r--   0        0        0     4266 2023-05-26 00:09:33.385382 humanloop-0.4.4/humanloop/model/create_project_request.pyi
--rw-r--r--   0        0        0     2635 2023-05-26 00:09:33.385464 humanloop-0.4.4/humanloop/model/create_session_response.py
--rw-r--r--   0        0        0     2635 2023-05-26 00:09:33.385546 humanloop-0.4.4/humanloop/model/create_session_response.pyi
--rw-r--r--   0        0        0     3232 2023-05-26 00:09:33.385659 humanloop-0.4.4/humanloop/model/create_trace_request.py
--rw-r--r--   0        0        0     3232 2023-05-26 00:09:33.385751 humanloop-0.4.4/humanloop/model/create_trace_request.pyi
--rw-r--r--   0        0        0     3329 2023-05-26 00:09:33.385854 humanloop-0.4.4/humanloop/model/create_trace_response.py
--rw-r--r--   0        0        0     3329 2023-05-26 00:09:33.385954 humanloop-0.4.4/humanloop/model/create_trace_response.pyi
--rw-r--r--   0        0        0     7455 2023-05-26 00:09:33.386097 humanloop-0.4.4/humanloop/model/data_response.py
--rw-r--r--   0        0        0     7455 2023-05-26 00:09:33.386236 humanloop-0.4.4/humanloop/model/data_response.pyi
--rw-r--r--   0        0        0     8998 2023-05-26 00:09:33.386373 humanloop-0.4.4/humanloop/model/experiment_config_response.py
--rw-r--r--   0        0        0     8998 2023-05-26 00:09:33.386615 humanloop-0.4.4/humanloop/model/experiment_config_response.pyi
--rw-r--r--   0        0        0    12827 2023-05-26 00:09:33.386902 humanloop-0.4.4/humanloop/model/experiment_response.py
--rw-r--r--   0        0        0    12827 2023-05-26 00:09:33.387160 humanloop-0.4.4/humanloop/model/experiment_response.pyi
--rw-r--r--   0        0        0     1376 2023-05-26 00:09:33.387417 humanloop-0.4.4/humanloop/model/experiment_status.py
--rw-r--r--   0        0        0     1229 2023-05-26 00:09:33.387620 humanloop-0.4.4/humanloop/model/experiment_status.pyi
--rw-r--r--   0        0        0     1685 2023-05-26 00:09:33.387813 humanloop-0.4.4/humanloop/model/experiments_list_response.py
--rw-r--r--   0        0        0     1685 2023-05-26 00:09:33.388027 humanloop-0.4.4/humanloop/model/experiments_list_response.pyi
--rw-r--r--   0        0        0     6681 2023-05-26 00:09:33.388222 humanloop-0.4.4/humanloop/model/feedback.py
--rw-r--r--   0        0        0     6681 2023-05-26 00:09:33.388429 humanloop-0.4.4/humanloop/model/feedback.pyi
--rw-r--r--   0        0        0     1463 2023-05-26 00:09:33.388630 humanloop-0.4.4/humanloop/model/feedback_class.py
--rw-r--r--   0        0        0     1296 2023-05-26 00:09:33.388826 humanloop-0.4.4/humanloop/model/feedback_class.pyi
--rw-r--r--   0        0        0     3334 2023-05-26 00:09:33.389017 humanloop-0.4.4/humanloop/model/feedback_label_request.py
--rw-r--r--   0        0        0     3334 2023-05-26 00:09:33.389230 humanloop-0.4.4/humanloop/model/feedback_label_request.pyi
--rw-r--r--   0        0        0     7189 2023-05-26 00:09:33.389411 humanloop-0.4.4/humanloop/model/feedback_request.py
--rw-r--r--   0        0        0     7189 2023-05-26 00:09:33.389571 humanloop-0.4.4/humanloop/model/feedback_request.pyi
--rw-r--r--   0        0        0     7141 2023-05-26 00:09:33.389747 humanloop-0.4.4/humanloop/model/feedback_response.py
--rw-r--r--   0        0        0     7141 2023-05-26 00:09:33.390041 humanloop-0.4.4/humanloop/model/feedback_response.pyi
--rw-r--r--   0        0        0     3200 2023-05-26 00:09:33.390309 humanloop-0.4.4/humanloop/model/feedback_submit_request.py
--rw-r--r--   0        0        0     3200 2023-05-26 00:09:33.390470 humanloop-0.4.4/humanloop/model/feedback_submit_request.pyi
--rw-r--r--   0        0        0     3210 2023-05-26 00:09:33.390620 humanloop-0.4.4/humanloop/model/feedback_submit_response.py
--rw-r--r--   0        0        0     3210 2023-05-26 00:09:33.390801 humanloop-0.4.4/humanloop/model/feedback_submit_response.pyi
--rw-r--r--   0        0        0     1690 2023-05-26 00:09:33.390957 humanloop-0.4.4/humanloop/model/feedback_type.py
--rw-r--r--   0        0        0     1459 2023-05-26 00:09:33.391121 humanloop-0.4.4/humanloop/model/feedback_type.pyi
--rw-r--r--   0        0        0     6161 2023-05-26 00:09:33.391277 humanloop-0.4.4/humanloop/model/feedback_type_model.py
--rw-r--r--   0        0        0     6161 2023-05-26 00:09:33.391439 humanloop-0.4.4/humanloop/model/feedback_type_model.pyi
--rw-r--r--   0        0        0     6289 2023-05-26 00:09:33.391592 humanloop-0.4.4/humanloop/model/feedback_type_request.py
--rw-r--r--   0        0        0     6289 2023-05-26 00:09:33.391728 humanloop-0.4.4/humanloop/model/feedback_type_request.pyi
--rw-r--r--   0        0        0     1659 2023-05-26 00:09:33.391809 humanloop-0.4.4/humanloop/model/feedback_types.py
--rw-r--r--   0        0        0     1659 2023-05-26 00:09:33.391891 humanloop-0.4.4/humanloop/model/feedback_types.pyi
--rw-r--r--   0        0        0     4407 2023-05-26 00:09:33.391974 humanloop-0.4.4/humanloop/model/generic_config_request.py
--rw-r--r--   0        0        0     4238 2023-05-26 00:09:33.392059 humanloop-0.4.4/humanloop/model/generic_config_request.pyi
--rw-r--r--   0        0        0     6562 2023-05-26 00:09:33.392142 humanloop-0.4.4/humanloop/model/generic_config_response.py
--rw-r--r--   0        0        0     6562 2023-05-26 00:09:33.392226 humanloop-0.4.4/humanloop/model/generic_config_response.pyi
--rw-r--r--   0        0        0     9619 2023-05-26 00:09:33.392316 humanloop-0.4.4/humanloop/model/get_model_config_response.py
--rw-r--r--   0        0        0     9619 2023-05-26 00:09:33.392442 humanloop-0.4.4/humanloop/model/get_model_config_response.pyi
--rw-r--r--   0        0        0     3611 2023-05-26 00:09:33.392585 humanloop-0.4.4/humanloop/model/http_validation_error.py
--rw-r--r--   0        0        0     3611 2023-05-26 00:09:33.392724 humanloop-0.4.4/humanloop/model/http_validation_error.pyi
--rw-r--r--   0        0        0     1667 2023-05-26 00:09:33.392867 humanloop-0.4.4/humanloop/model/label_sentiment.py
--rw-r--r--   0        0        0     1468 2023-05-26 00:09:33.393012 humanloop-0.4.4/humanloop/model/label_sentiment.pyi
--rw-r--r--   0        0        0     3156 2023-05-26 00:09:33.393165 humanloop-0.4.4/humanloop/model/log_datapoint_request.py
--rw-r--r--   0        0        0     3156 2023-05-26 00:09:33.393315 humanloop-0.4.4/humanloop/model/log_datapoint_request.pyi
--rw-r--r--   0        0        0    17219 2023-05-26 00:09:33.393566 humanloop-0.4.4/humanloop/model/log_model_config_request.py
--rw-r--r--   0        0        0    17219 2023-05-26 00:09:33.393871 humanloop-0.4.4/humanloop/model/log_model_config_request.pyi
--rw-r--r--   0        0        0    15844 2023-05-26 00:09:33.394106 humanloop-0.4.4/humanloop/model/log_request.py
--rw-r--r--   0        0        0    15844 2023-05-26 00:09:33.394496 humanloop-0.4.4/humanloop/model/log_request.pyi
--rw-r--r--   0        0        0    20160 2023-05-26 00:09:33.394844 humanloop-0.4.4/humanloop/model/log_response.py
--rw-r--r--   0        0        0    20160 2023-05-26 00:09:33.395113 humanloop-0.4.4/humanloop/model/log_response.pyi
--rw-r--r--   0        0        0     3205 2023-05-26 00:09:33.395336 humanloop-0.4.4/humanloop/model/logs_log_response.py
--rw-r--r--   0        0        0     3205 2023-05-26 00:09:33.395496 humanloop-0.4.4/humanloop/model/logs_log_response.pyi
--rw-r--r--   0        0        0    16246 2023-05-26 00:09:33.395666 humanloop-0.4.4/humanloop/model/model_config_chat_request.py
--rw-r--r--   0        0        0    16246 2023-05-26 00:09:33.395878 humanloop-0.4.4/humanloop/model/model_config_chat_request.pyi
--rw-r--r--   0        0        0    15386 2023-05-26 00:09:33.396090 humanloop-0.4.4/humanloop/model/model_config_completion_request.py
--rw-r--r--   0        0        0    15386 2023-05-26 00:09:33.396290 humanloop-0.4.4/humanloop/model/model_config_completion_request.pyi
--rw-r--r--   0        0        0    17859 2023-05-26 00:09:33.396535 humanloop-0.4.4/humanloop/model/model_config_response.py
--rw-r--r--   0        0        0    17859 2023-05-26 00:09:33.396754 humanloop-0.4.4/humanloop/model/model_config_response.pyi
--rw-r--r--   0        0        0    20554 2023-05-26 00:09:33.396963 humanloop-0.4.4/humanloop/model/model_config_response2.py
--rw-r--r--   0        0        0    20554 2023-05-26 00:09:33.397166 humanloop-0.4.4/humanloop/model/model_config_response2.pyi
--rw-r--r--   0        0        0     1460 2023-05-26 00:09:33.397348 humanloop-0.4.4/humanloop/model/model_endpoints.py
--rw-r--r--   0        0        0     1305 2023-05-26 00:09:33.397493 humanloop-0.4.4/humanloop/model/model_endpoints.pyi
--rw-r--r--   0        0        0     1695 2023-05-26 00:09:33.397641 humanloop-0.4.4/humanloop/model/model_providers.py
--rw-r--r--   0        0        0     1468 2023-05-26 00:09:33.397779 humanloop-0.4.4/humanloop/model/model_providers.pyi
--rw-r--r--   0        0        0     5144 2023-05-26 00:09:33.397946 humanloop-0.4.4/humanloop/model/paginated_data_log_response.py
--rw-r--r--   0        0        0     5144 2023-05-26 00:09:33.398153 humanloop-0.4.4/humanloop/model/paginated_data_log_response.pyi
--rw-r--r--   0        0        0     5180 2023-05-26 00:09:33.398327 humanloop-0.4.4/humanloop/model/paginated_data_project_response.py
--rw-r--r--   0        0        0     5180 2023-05-26 00:09:33.398475 humanloop-0.4.4/humanloop/model/paginated_data_project_response.pyi
--rw-r--r--   0        0        0     5180 2023-05-26 00:09:33.398617 humanloop-0.4.4/humanloop/model/paginated_data_session_response.py
--rw-r--r--   0        0        0     5180 2023-05-26 00:09:33.398802 humanloop-0.4.4/humanloop/model/paginated_data_session_response.pyi
--rw-r--r--   0        0        0     3143 2023-05-26 00:09:33.398968 humanloop-0.4.4/humanloop/model/positive_label.py
--rw-r--r--   0        0        0     3143 2023-05-26 00:09:33.399127 humanloop-0.4.4/humanloop/model/positive_label.pyi
--rw-r--r--   0        0        0     8900 2023-05-26 00:09:33.399307 humanloop-0.4.4/humanloop/model/project_config_response.py
--rw-r--r--   0        0        0     8900 2023-05-26 00:09:33.399516 humanloop-0.4.4/humanloop/model/project_config_response.pyi
--rw-r--r--   0        0        0    18363 2023-05-26 00:09:33.399715 humanloop-0.4.4/humanloop/model/project_model_config_request.py
--rw-r--r--   0        0        0    18363 2023-05-26 00:09:33.399923 humanloop-0.4.4/humanloop/model/project_model_config_request.pyi
--rw-r--r--   0        0        0    23968 2023-05-26 00:09:33.400111 humanloop-0.4.4/humanloop/model/project_model_config_response.py
--rw-r--r--   0        0        0    23968 2023-05-26 00:09:33.400242 humanloop-0.4.4/humanloop/model/project_model_config_response.pyi
--rw-r--r--   0        0        0    13895 2023-05-26 00:09:33.400364 humanloop-0.4.4/humanloop/model/project_response.py
--rw-r--r--   0        0        0    13895 2023-05-26 00:09:33.400542 humanloop-0.4.4/humanloop/model/project_response.pyi
--rw-r--r--   0        0        0     1471 2023-05-26 00:09:33.400725 humanloop-0.4.4/humanloop/model/project_sort_by.py
--rw-r--r--   0        0        0     1300 2023-05-26 00:09:33.400871 humanloop-0.4.4/humanloop/model/project_sort_by.pyi
--rw-r--r--   0        0        0     3795 2023-05-26 00:09:33.401033 humanloop-0.4.4/humanloop/model/project_user_response.py
--rw-r--r--   0        0        0     3795 2023-05-26 00:09:33.401194 humanloop-0.4.4/humanloop/model/project_user_response.pyi
--rw-r--r--   0        0        0     1713 2023-05-26 00:09:33.401332 humanloop-0.4.4/humanloop/model/projects_get_configs_response.py
--rw-r--r--   0        0        0     1713 2023-05-26 00:09:33.401471 humanloop-0.4.4/humanloop/model/projects_get_configs_response.pyi
--rw-r--r--   0        0        0     1715 2023-05-26 00:09:33.401609 humanloop-0.4.4/humanloop/model/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0     1715 2023-05-26 00:09:33.401746 humanloop-0.4.4/humanloop/model/projects_update_feedback_types_request.pyi
--rw-r--r--   0        0        0     4150 2023-05-26 00:09:33.401882 humanloop-0.4.4/humanloop/model/provider_api_keys.py
--rw-r--r--   0        0        0     4150 2023-05-26 00:09:33.402020 humanloop-0.4.4/humanloop/model/provider_api_keys.pyi
--rw-r--r--   0        0        0     3113 2023-05-26 00:09:33.402163 humanloop-0.4.4/humanloop/model/session_project_response.py
--rw-r--r--   0        0        0     3113 2023-05-26 00:09:33.402305 humanloop-0.4.4/humanloop/model/session_project_response.pyi
--rw-r--r--   0        0        0     6620 2023-05-26 00:09:33.402434 humanloop-0.4.4/humanloop/model/session_response.py
--rw-r--r--   0        0        0     6620 2023-05-26 00:09:33.402574 humanloop-0.4.4/humanloop/model/session_response.pyi
--rw-r--r--   0        0        0     1309 2023-05-26 00:09:33.402724 humanloop-0.4.4/humanloop/model/sort_order.py
--rw-r--r--   0        0        0     1192 2023-05-26 00:09:33.402863 humanloop-0.4.4/humanloop/model/sort_order.pyi
--rw-r--r--   0        0        0     4889 2023-05-26 00:09:33.403027 humanloop-0.4.4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4889 2023-05-26 00:09:33.403174 humanloop-0.4.4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0     4893 2023-05-26 00:09:33.403321 humanloop-0.4.4/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4893 2023-05-26 00:09:33.403485 humanloop-0.4.4/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0     4951 2023-05-26 00:09:33.403637 humanloop-0.4.4/humanloop/model/tool_config_request.py
--rw-r--r--   0        0        0     4788 2023-05-26 00:09:33.403769 humanloop-0.4.4/humanloop/model/tool_config_request.pyi
--rw-r--r--   0        0        0     7064 2023-05-26 00:09:33.403904 humanloop-0.4.4/humanloop/model/tool_config_response.py
--rw-r--r--   0        0        0     7064 2023-05-26 00:09:33.404112 humanloop-0.4.4/humanloop/model/tool_config_response.pyi
--rw-r--r--   0        0        0     4232 2023-05-26 00:09:33.404287 humanloop-0.4.4/humanloop/model/tool_result_response.py
--rw-r--r--   0        0        0     4232 2023-05-26 00:09:33.404431 humanloop-0.4.4/humanloop/model/tool_result_response.pyi
--rw-r--r--   0        0        0    13080 2023-05-26 00:09:33.404593 humanloop-0.4.4/humanloop/model/trace_log_request.py
--rw-r--r--   0        0        0    13080 2023-05-26 00:09:33.404822 humanloop-0.4.4/humanloop/model/trace_log_request.pyi
--rw-r--r--   0        0        0    19510 2023-05-26 00:09:33.405079 humanloop-0.4.4/humanloop/model/trace_model_config_request.py
--rw-r--r--   0        0        0    19345 2023-05-26 00:09:33.405320 humanloop-0.4.4/humanloop/model/trace_model_config_request.pyi
--rw-r--r--   0        0        0     7302 2023-05-26 00:09:33.405538 humanloop-0.4.4/humanloop/model/update_experiment_request.py
--rw-r--r--   0        0        0     7302 2023-05-26 00:09:33.405700 humanloop-0.4.4/humanloop/model/update_experiment_request.pyi
--rw-r--r--   0        0        0     5047 2023-05-26 00:09:33.405854 humanloop-0.4.4/humanloop/model/update_project_request.py
--rw-r--r--   0        0        0     5047 2023-05-26 00:09:33.406011 humanloop-0.4.4/humanloop/model/update_project_request.pyi
--rw-r--r--   0        0        0     4118 2023-05-26 00:09:33.406164 humanloop-0.4.4/humanloop/model/usage.py
--rw-r--r--   0        0        0     4118 2023-05-26 00:09:33.406326 humanloop-0.4.4/humanloop/model/usage.pyi
--rw-r--r--   0        0        0     6805 2023-05-26 00:09:33.406468 humanloop-0.4.4/humanloop/model/validation_error.py
--rw-r--r--   0        0        0     6805 2023-05-26 00:09:33.406614 humanloop-0.4.4/humanloop/model/validation_error.pyi
--rw-r--r--   0        0        0     6379 2023-05-26 00:09:33.406760 humanloop-0.4.4/humanloop/models/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-26 00:09:33.406910 humanloop-0.4.4/humanloop/paths/__init__.py
--rw-r--r--   0        0        0      285 2023-05-26 00:09:33.407046 humanloop-0.4.4/humanloop/paths/chat/__init__.py
--rw-r--r--   0        0        0    17428 2023-05-26 00:09:33.407245 humanloop-0.4.4/humanloop/paths/chat/post.py
--rw-r--r--   0        0        0    17285 2023-05-26 00:09:33.407480 humanloop-0.4.4/humanloop/paths/chat/post.pyi
--rw-r--r--   0        0        0      302 2023-05-26 00:09:33.407684 humanloop-0.4.4/humanloop/paths/chat_deployed/__init__.py
--rw-r--r--   0        0        0    16991 2023-05-26 00:09:33.408384 humanloop-0.4.4/humanloop/paths/chat_deployed/post.py
--rw-r--r--   0        0        0    16848 2023-05-26 00:09:33.408725 humanloop-0.4.4/humanloop/paths/chat_deployed/post.pyi
--rw-r--r--   0        0        0      306 2023-05-26 00:09:33.408939 humanloop-0.4.4/humanloop/paths/chat_experiment/__init__.py
--rw-r--r--   0        0        0    17434 2023-05-26 00:09:33.409140 humanloop-0.4.4/humanloop/paths/chat_experiment/post.py
--rw-r--r--   0        0        0    17291 2023-05-26 00:09:33.409361 humanloop-0.4.4/humanloop/paths/chat_experiment/post.pyi
--rw-r--r--   0        0        0      309 2023-05-26 00:09:33.409537 humanloop-0.4.4/humanloop/paths/chat_model_config/__init__.py
--rw-r--r--   0        0        0    17609 2023-05-26 00:09:33.409718 humanloop-0.4.4/humanloop/paths/chat_model_config/post.py
--rw-r--r--   0        0        0    17466 2023-05-26 00:09:33.409984 humanloop-0.4.4/humanloop/paths/chat_model_config/post.pyi
--rw-r--r--   0        0        0      297 2023-05-26 00:09:33.410169 humanloop-0.4.4/humanloop/paths/completion/__init__.py
--rw-r--r--   0        0        0    17744 2023-05-26 00:09:33.410338 humanloop-0.4.4/humanloop/paths/completion/post.py
--rw-r--r--   0        0        0    17601 2023-05-26 00:09:33.410486 humanloop-0.4.4/humanloop/paths/completion/post.pyi
--rw-r--r--   0        0        0      314 2023-05-26 00:09:33.410662 humanloop-0.4.4/humanloop/paths/completion_deployed/__init__.py
--rw-r--r--   0        0        0    17247 2023-05-26 00:09:33.410830 humanloop-0.4.4/humanloop/paths/completion_deployed/post.py
--rw-r--r--   0        0        0    17104 2023-05-26 00:09:33.411069 humanloop-0.4.4/humanloop/paths/completion_deployed/post.pyi
--rw-r--r--   0        0        0      318 2023-05-26 00:09:33.411316 humanloop-0.4.4/humanloop/paths/completion_experiment/__init__.py
--rw-r--r--   0        0        0    17690 2023-05-26 00:09:33.411495 humanloop-0.4.4/humanloop/paths/completion_experiment/post.py
--rw-r--r--   0        0        0    17547 2023-05-26 00:09:33.411728 humanloop-0.4.4/humanloop/paths/completion_experiment/post.pyi
--rw-r--r--   0        0        0      321 2023-05-26 00:09:33.411961 humanloop-0.4.4/humanloop/paths/completion_model_config/__init__.py
--rw-r--r--   0        0        0    17865 2023-05-26 00:09:33.412136 humanloop-0.4.4/humanloop/paths/completion_model_config/post.py
--rw-r--r--   0        0        0    17722 2023-05-26 00:09:33.412367 humanloop-0.4.4/humanloop/paths/completion_model_config/post.pyi
--rw-r--r--   0        0        0      327 2023-05-26 00:09:33.412566 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/__init__.py
--rw-r--r--   0        0        0    11995 2023-05-26 00:09:33.412728 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/delete.py
--rw-r--r--   0        0        0    11852 2023-05-26 00:09:33.412933 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/delete.pyi
--rw-r--r--   0        0        0    17043 2023-05-26 00:09:33.413163 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/patch.py
--rw-r--r--   0        0        0    16900 2023-05-26 00:09:33.413376 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/patch.pyi
--rw-r--r--   0        0        0      352 2023-05-26 00:09:33.413607 humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/__init__.py
--rw-r--r--   0        0        0    12496 2023-05-26 00:09:33.413778 humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/get.py
--rw-r--r--   0        0        0    12353 2023-05-26 00:09:33.414188 humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/get.pyi
--rw-r--r--   0        0        0      293 2023-05-26 00:09:33.414383 humanloop-0.4.4/humanloop/paths/feedback/__init__.py
--rw-r--r--   0        0        0    15089 2023-05-26 00:09:33.414553 humanloop-0.4.4/humanloop/paths/feedback/post.py
--rw-r--r--   0        0        0    14946 2023-05-26 00:09:33.414768 humanloop-0.4.4/humanloop/paths/feedback/post.pyi
--rw-r--r--   0        0        0      285 2023-05-26 00:09:33.414989 humanloop-0.4.4/humanloop/paths/logs/__init__.py
--rw-r--r--   0        0        0    20891 2023-05-26 00:09:33.415195 humanloop-0.4.4/humanloop/paths/logs/post.py
--rw-r--r--   0        0        0    20748 2023-05-26 00:09:33.415420 humanloop-0.4.4/humanloop/paths/logs/post.pyi
--rw-r--r--   0        0        0      302 2023-05-26 00:09:33.415614 humanloop-0.4.4/humanloop/paths/model_configs/__init__.py
--rw-r--r--   0        0        0    20266 2023-05-26 00:09:33.415801 humanloop-0.4.4/humanloop/paths/model_configs/post.py
--rw-r--r--   0        0        0    20123 2023-05-26 00:09:33.416037 humanloop-0.4.4/humanloop/paths/model_configs/post.pyi
--rw-r--r--   0        0        0      308 2023-05-26 00:09:33.416239 humanloop-0.4.4/humanloop/paths/model_configs_id/__init__.py
--rw-r--r--   0        0        0    12023 2023-05-26 00:09:33.416409 humanloop-0.4.4/humanloop/paths/model_configs_id/get.py
--rw-r--r--   0        0        0    11880 2023-05-26 00:09:33.416832 humanloop-0.4.4/humanloop/paths/model_configs_id/get.pyi
--rw-r--r--   0        0        0      293 2023-05-26 00:09:33.417031 humanloop-0.4.4/humanloop/paths/projects/__init__.py
--rw-r--r--   0        0        0    20518 2023-05-26 00:09:33.417222 humanloop-0.4.4/humanloop/paths/projects/get.py
--rw-r--r--   0        0        0    20375 2023-05-26 00:09:33.417418 humanloop-0.4.4/humanloop/paths/projects/get.pyi
--rw-r--r--   0        0        0    13007 2023-05-26 00:09:33.417605 humanloop-0.4.4/humanloop/paths/projects/post.py
--rw-r--r--   0        0        0    12864 2023-05-26 00:09:33.417827 humanloop-0.4.4/humanloop/paths/projects/post.pyi
--rw-r--r--   0        0        0      299 2023-05-26 00:09:33.418042 humanloop-0.4.4/humanloop/paths/projects_id/__init__.py
--rw-r--r--   0        0        0    11979 2023-05-26 00:09:33.418232 humanloop-0.4.4/humanloop/paths/projects_id/get.py
--rw-r--r--   0        0        0    11836 2023-05-26 00:09:33.418471 humanloop-0.4.4/humanloop/paths/projects_id/get.pyi
--rw-r--r--   0        0        0    16066 2023-05-26 00:09:33.418722 humanloop-0.4.4/humanloop/paths/projects_id/patch.py
--rw-r--r--   0        0        0    15923 2023-05-26 00:09:33.418969 humanloop-0.4.4/humanloop/paths/projects_id/patch.pyi
--rw-r--r--   0        0        0      326 2023-05-26 00:09:33.419195 humanloop-0.4.4/humanloop/paths/projects_id_active_config/__init__.py
--rw-r--r--   0        0        0    12298 2023-05-26 00:09:33.419382 humanloop-0.4.4/humanloop/paths/projects_id_active_config/delete.py
--rw-r--r--   0        0        0    12155 2023-05-26 00:09:33.419618 humanloop-0.4.4/humanloop/paths/projects_id_active_config/delete.pyi
--rw-r--r--   0        0        0    12148 2023-05-26 00:09:33.419838 humanloop-0.4.4/humanloop/paths/projects_id_active_config/get.py
--rw-r--r--   0        0        0    12005 2023-05-26 00:09:33.420056 humanloop-0.4.4/humanloop/paths/projects_id_active_config/get.pyi
--rw-r--r--   0        0        0      334 2023-05-26 00:09:33.420251 humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/__init__.py
--rw-r--r--   0        0        0    12306 2023-05-26 00:09:33.420447 humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/delete.py
--rw-r--r--   0        0        0    12163 2023-05-26 00:09:33.420684 humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/delete.pyi
--rw-r--r--   0        0        0      315 2023-05-26 00:09:33.420881 humanloop-0.4.4/humanloop/paths/projects_id_configs/__init__.py
--rw-r--r--   0        0        0    12182 2023-05-26 00:09:33.421060 humanloop-0.4.4/humanloop/paths/projects_id_configs/get.py
--rw-r--r--   0        0        0    12039 2023-05-26 00:09:33.421323 humanloop-0.4.4/humanloop/paths/projects_id_configs/get.pyi
--rw-r--r--   0        0        0      313 2023-05-26 00:09:33.421557 humanloop-0.4.4/humanloop/paths/projects_id_export/__init__.py
--rw-r--r--   0        0        0    15728 2023-05-26 00:09:33.421736 humanloop-0.4.4/humanloop/paths/projects_id_export/post.py
--rw-r--r--   0        0        0    15585 2023-05-26 00:09:33.421996 humanloop-0.4.4/humanloop/paths/projects_id_export/post.pyi
--rw-r--r--   0        0        0      328 2023-05-26 00:09:33.422193 humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/__init__.py
--rw-r--r--   0        0        0    14798 2023-05-26 00:09:33.422375 humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/patch.py
--rw-r--r--   0        0        0    14655 2023-05-26 00:09:33.422581 humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/patch.pyi
--rw-r--r--   0        0        0      339 2023-05-26 00:09:33.422766 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/__init__.py
--rw-r--r--   0        0        0    12256 2023-05-26 00:09:33.422935 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/get.py
--rw-r--r--   0        0        0    12113 2023-05-26 00:09:33.423152 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/get.pyi
--rw-r--r--   0        0        0    16250 2023-05-26 00:09:33.423350 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/post.py
--rw-r--r--   0        0        0    16107 2023-05-26 00:09:33.423545 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/post.pyi
--rw-r--r--   0        0        0      293 2023-05-26 00:09:33.423731 humanloop-0.4.4/humanloop/paths/sessions/__init__.py
--rw-r--r--   0        0        0    14112 2023-05-26 00:09:33.423900 humanloop-0.4.4/humanloop/paths/sessions/get.py
--rw-r--r--   0        0        0    13969 2023-05-26 00:09:33.424115 humanloop-0.4.4/humanloop/paths/sessions/get.pyi
--rw-r--r--   0        0        0     9192 2023-05-26 00:09:33.424327 humanloop-0.4.4/humanloop/paths/sessions/post.py
--rw-r--r--   0        0        0     9079 2023-05-26 00:09:33.424529 humanloop-0.4.4/humanloop/paths/sessions/post.pyi
--rw-r--r--   0        0        0      299 2023-05-26 00:09:33.424687 humanloop-0.4.4/humanloop/paths/sessions_id/__init__.py
--rw-r--r--   0        0        0    11979 2023-05-26 00:09:33.424816 humanloop-0.4.4/humanloop/paths/sessions_id/get.py
--rw-r--r--   0        0        0    11836 2023-05-26 00:09:33.424933 humanloop-0.4.4/humanloop/paths/sessions_id/get.pyi
--rw-r--r--   0        0        0      289 2023-05-26 00:09:33.425044 humanloop-0.4.4/humanloop/paths/traces/__init__.py
--rw-r--r--   0        0        0    12450 2023-05-26 00:09:33.425152 humanloop-0.4.4/humanloop/paths/traces/post.py
--rw-r--r--   0        0        0    12307 2023-05-26 00:09:33.425308 humanloop-0.4.4/humanloop/paths/traces/post.pyi
--rw-r--r--   0        0        0     1011 2023-05-26 00:09:33.425521 humanloop-0.4.4/humanloop/request_after_hook.py
--rw-r--r--   0        0        0     1783 2023-05-26 00:09:33.461649 humanloop-0.4.4/humanloop/request_before_hook.py
--rw-r--r--   0        0        0    11329 2023-05-26 00:09:33.425845 humanloop-0.4.4/humanloop/rest.py
--rw-r--r--   0        0        0    95913 2023-05-26 00:09:33.426216 humanloop-0.4.4/humanloop/schemas.py
--rw-r--r--   0        0        0        0 2023-05-26 00:09:33.426384 humanloop-0.4.4/humanloop/type/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-26 00:09:33.426580 humanloop-0.4.4/humanloop/type/agent_config_request.py
--rw-r--r--   0        0        0     1608 2023-05-26 00:09:33.426720 humanloop-0.4.4/humanloop/type/agent_config_response.py
--rw-r--r--   0        0        0     1408 2023-05-26 00:09:33.426864 humanloop-0.4.4/humanloop/type/base_metric_response.py
--rw-r--r--   0        0        0     1062 2023-05-26 00:09:33.427008 humanloop-0.4.4/humanloop/type/categorical_feedback_label.py
--rw-r--r--   0        0        0     2183 2023-05-26 00:09:33.427149 humanloop-0.4.4/humanloop/type/chat_data_response.py
--rw-r--r--   0        0        0     1990 2023-05-26 00:09:33.427304 humanloop-0.4.4/humanloop/type/chat_deployed_request.py
--rw-r--r--   0        0        0     2235 2023-05-26 00:09:33.427453 humanloop-0.4.4/humanloop/type/chat_experiment_request.py
--rw-r--r--   0        0        0      919 2023-05-26 00:09:33.427608 humanloop-0.4.4/humanloop/type/chat_message.py
--rw-r--r--   0        0        0     2104 2023-05-26 00:09:33.427759 humanloop-0.4.4/humanloop/type/chat_model_config_request.py
--rw-r--r--   0        0        0     2130 2023-05-26 00:09:33.427911 humanloop-0.4.4/humanloop/type/chat_request.py
--rw-r--r--   0        0        0     1818 2023-05-26 00:09:33.428071 humanloop-0.4.4/humanloop/type/chat_response.py
--rw-r--r--   0        0        0      711 2023-05-26 00:09:33.428224 humanloop-0.4.4/humanloop/type/chat_role.py
--rw-r--r--   0        0        0     2095 2023-05-26 00:09:33.428413 humanloop-0.4.4/humanloop/type/completion_deployed_request.py
--rw-r--r--   0        0        0     2343 2023-05-26 00:09:33.428576 humanloop-0.4.4/humanloop/type/completion_experiment_request.py
--rw-r--r--   0        0        0     2209 2023-05-26 00:09:33.428729 humanloop-0.4.4/humanloop/type/completion_model_config_request.py
--rw-r--r--   0        0        0     2239 2023-05-26 00:09:33.428905 humanloop-0.4.4/humanloop/type/completion_request.py
--rw-r--r--   0        0        0     1864 2023-05-26 00:09:33.429066 humanloop-0.4.4/humanloop/type/completion_response.py
--rw-r--r--   0        0        0     1054 2023-05-26 00:09:33.429226 humanloop-0.4.4/humanloop/type/config_response.py
--rw-r--r--   0        0        0      719 2023-05-26 00:09:33.429407 humanloop-0.4.4/humanloop/type/config_type.py
--rw-r--r--   0        0        0     1362 2023-05-26 00:09:33.429552 humanloop-0.4.4/humanloop/type/create_experiment_request.py
--rw-r--r--   0        0        0     1024 2023-05-26 00:09:33.429724 humanloop-0.4.4/humanloop/type/create_log_response.py
--rw-r--r--   0        0        0     1066 2023-05-26 00:09:33.429874 humanloop-0.4.4/humanloop/type/create_project_request.py
--rw-r--r--   0        0        0      942 2023-05-26 00:09:33.430013 humanloop-0.4.4/humanloop/type/create_session_response.py
--rw-r--r--   0        0        0     1045 2023-05-26 00:09:33.430181 humanloop-0.4.4/humanloop/type/create_trace_request.py
--rw-r--r--   0        0        0      998 2023-05-26 00:09:33.430340 humanloop-0.4.4/humanloop/type/create_trace_response.py
--rw-r--r--   0        0        0     2013 2023-05-26 00:09:33.430502 humanloop-0.4.4/humanloop/type/data_response.py
--rw-r--r--   0        0        0     1677 2023-05-26 00:09:33.430838 humanloop-0.4.4/humanloop/type/experiment_config_response.py
--rw-r--r--   0        0        0     1788 2023-05-26 00:09:33.431062 humanloop-0.4.4/humanloop/type/experiment_response.py
--rw-r--r--   0        0        0      718 2023-05-26 00:09:33.431306 humanloop-0.4.4/humanloop/type/experiment_status.py
--rw-r--r--   0        0        0      785 2023-05-26 00:09:33.431545 humanloop-0.4.4/humanloop/type/experiments_list_response.py
--rw-r--r--   0        0        0     1449 2023-05-26 00:09:33.431838 humanloop-0.4.4/humanloop/type/feedback.py
--rw-r--r--   0        0        0      719 2023-05-26 00:09:33.432126 humanloop-0.4.4/humanloop/type/feedback_class.py
--rw-r--r--   0        0        0      970 2023-05-26 00:09:33.432425 humanloop-0.4.4/humanloop/type/feedback_label_request.py
--rw-r--r--   0        0        0     1546 2023-05-26 00:09:33.432656 humanloop-0.4.4/humanloop/type/feedback_request.py
--rw-r--r--   0        0        0     1578 2023-05-26 00:09:33.432901 humanloop-0.4.4/humanloop/type/feedback_response.py
--rw-r--r--   0        0        0      804 2023-05-26 00:09:33.433105 humanloop-0.4.4/humanloop/type/feedback_submit_request.py
--rw-r--r--   0        0        0      809 2023-05-26 00:09:33.433304 humanloop-0.4.4/humanloop/type/feedback_submit_response.py
--rw-r--r--   0        0        0      738 2023-05-26 00:09:33.433734 humanloop-0.4.4/humanloop/type/feedback_type.py
--rw-r--r--   0        0        0     1307 2023-05-26 00:09:33.434005 humanloop-0.4.4/humanloop/type/feedback_type_model.py
--rw-r--r--   0        0        0     1541 2023-05-26 00:09:33.434262 humanloop-0.4.4/humanloop/type/feedback_type_request.py
--rw-r--r--   0        0        0      773 2023-05-26 00:09:33.434743 humanloop-0.4.4/humanloop/type/feedback_types.py
--rw-r--r--   0        0        0     1064 2023-05-26 00:09:33.435026 humanloop-0.4.4/humanloop/type/generic_config_request.py
--rw-r--r--   0        0        0     1262 2023-05-26 00:09:33.435250 humanloop-0.4.4/humanloop/type/generic_config_response.py
--rw-r--r--   0        0        0     1900 2023-05-26 00:09:33.435468 humanloop-0.4.4/humanloop/type/get_model_config_response.py
--rw-r--r--   0        0        0      972 2023-05-26 00:09:33.435661 humanloop-0.4.4/humanloop/type/http_validation_error.py
--rw-r--r--   0        0        0      730 2023-05-26 00:09:33.435872 humanloop-0.4.4/humanloop/type/label_sentiment.py
--rw-r--r--   0        0        0      782 2023-05-26 00:09:33.436098 humanloop-0.4.4/humanloop/type/log_datapoint_request.py
--rw-r--r--   0        0        0     3033 2023-05-26 00:09:33.436346 humanloop-0.4.4/humanloop/type/log_model_config_request.py
--rw-r--r--   0        0        0     2652 2023-05-26 00:09:33.436549 humanloop-0.4.4/humanloop/type/log_request.py
--rw-r--r--   0        0        0     2961 2023-05-26 00:09:33.436748 humanloop-0.4.4/humanloop/type/log_response.py
--rw-r--r--   0        0        0      807 2023-05-26 00:09:33.436938 humanloop-0.4.4/humanloop/type/logs_log_response.py
--rw-r--r--   0        0        0     2820 2023-05-26 00:09:33.437190 humanloop-0.4.4/humanloop/type/model_config_chat_request.py
--rw-r--r--   0        0        0     2713 2023-05-26 00:09:33.437424 humanloop-0.4.4/humanloop/type/model_config_completion_request.py
--rw-r--r--   0        0        0     3160 2023-05-26 00:09:33.437692 humanloop-0.4.4/humanloop/type/model_config_response.py
--rw-r--r--   0        0        0     3281 2023-05-26 00:09:33.438021 humanloop-0.4.4/humanloop/type/model_config_response2.py
--rw-r--r--   0        0        0      714 2023-05-26 00:09:33.438400 humanloop-0.4.4/humanloop/type/model_endpoints.py
--rw-r--r--   0        0        0      738 2023-05-26 00:09:33.438780 humanloop-0.4.4/humanloop/type/model_providers.py
--rw-r--r--   0        0        0     1032 2023-05-26 00:09:33.439012 humanloop-0.4.4/humanloop/type/paginated_data_log_response.py
--rw-r--r--   0        0        0     1064 2023-05-26 00:09:33.439156 humanloop-0.4.4/humanloop/type/paginated_data_project_response.py
--rw-r--r--   0        0        0     1064 2023-05-26 00:09:33.439314 humanloop-0.4.4/humanloop/type/paginated_data_session_response.py
--rw-r--r--   0        0        0      871 2023-05-26 00:09:33.439484 humanloop-0.4.4/humanloop/type/positive_label.py
--rw-r--r--   0        0        0     1820 2023-05-26 00:09:33.439701 humanloop-0.4.4/humanloop/type/project_config_response.py
--rw-r--r--   0        0        0     3410 2023-05-26 00:09:33.439904 humanloop-0.4.4/humanloop/type/project_model_config_request.py
--rw-r--r--   0        0        0     4053 2023-05-26 00:09:33.440080 humanloop-0.4.4/humanloop/type/project_model_config_response.py
--rw-r--r--   0        0        0     2032 2023-05-26 00:09:33.440251 humanloop-0.4.4/humanloop/type/project_response.py
--rw-r--r--   0        0        0      721 2023-05-26 00:09:33.440413 humanloop-0.4.4/humanloop/type/project_sort_by.py
--rw-r--r--   0        0        0     1022 2023-05-26 00:09:33.440572 humanloop-0.4.4/humanloop/type/project_user_response.py
--rw-r--r--   0        0        0      798 2023-05-26 00:09:33.440762 humanloop-0.4.4/humanloop/type/projects_get_configs_response.py
--rw-r--r--   0        0        0      800 2023-05-26 00:09:33.440947 humanloop-0.4.4/humanloop/type/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0      917 2023-05-26 00:09:33.441099 humanloop-0.4.4/humanloop/type/provider_api_keys.py
--rw-r--r--   0        0        0      985 2023-05-26 00:09:33.441384 humanloop-0.4.4/humanloop/type/session_project_response.py
--rw-r--r--   0        0        0     1442 2023-05-26 00:09:33.442041 humanloop-0.4.4/humanloop/type/session_response.py
--rw-r--r--   0        0        0      696 2023-05-26 00:09:33.442226 humanloop-0.4.4/humanloop/type/sort_order.py
--rw-r--r--   0        0        0     1241 2023-05-26 00:09:33.442401 humanloop-0.4.4/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     1251 2023-05-26 00:09:33.442587 humanloop-0.4.4/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     1066 2023-05-26 00:09:33.442780 humanloop-0.4.4/humanloop/type/tool_config_request.py
--rw-r--r--   0        0        0     1295 2023-05-26 00:09:33.442940 humanloop-0.4.4/humanloop/type/tool_config_response.py
--rw-r--r--   0        0        0      930 2023-05-26 00:09:33.443088 humanloop-0.4.4/humanloop/type/tool_result_response.py
--rw-r--r--   0        0        0     2427 2023-05-26 00:09:33.443226 humanloop-0.4.4/humanloop/type/trace_log_request.py
--rw-r--r--   0        0        0     3095 2023-05-26 00:09:33.443373 humanloop-0.4.4/humanloop/type/trace_model_config_request.py
--rw-r--r--   0        0        0     1361 2023-05-26 00:09:33.443521 humanloop-0.4.4/humanloop/type/update_experiment_request.py
--rw-r--r--   0        0        0     1434 2023-05-26 00:09:33.443664 humanloop-0.4.4/humanloop/type/update_project_request.py
--rw-r--r--   0        0        0     1042 2023-05-26 00:09:33.443809 humanloop-0.4.4/humanloop/type/usage.py
--rw-r--r--   0        0        0      951 2023-05-26 00:09:33.443976 humanloop-0.4.4/humanloop/type/validation_error.py
--rw-r--r--   0        0        0      868 2023-05-26 00:09:33.444124 humanloop-0.4.4/humanloop/type_util.py
--rw-r--r--   0        0        0     3165 2023-05-26 00:09:33.444298 humanloop-0.4.4/humanloop/validation_metadata.py
--rw-r--r--   0        0        0      714 2023-05-26 00:09:33.444959 humanloop-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     9366 1970-01-01 00:00:00.000000 humanloop-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-26 17:11:07.866710 humanloop-0.4.5/LICENSE
+-rw-r--r--   0        0        0     8475 2023-05-26 17:11:07.919690 humanloop-0.4.5/README.md
+-rw-r--r--   0        0        0     1059 2023-05-26 17:11:07.788815 humanloop-0.4.5/humanloop/__init__.py
+-rw-r--r--   0        0        0    73009 2023-05-26 17:11:07.788994 humanloop-0.4.5/humanloop/api_client.py
+-rw-r--r--   0        0        0      663 2023-05-26 17:11:07.789113 humanloop-0.4.5/humanloop/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-26 17:11:07.789224 humanloop-0.4.5/humanloop/apis/__init__.py
+-rw-r--r--   0        0        0     4698 2023-05-26 17:11:07.789316 humanloop-0.4.5/humanloop/apis/path_to_api.py
+-rw-r--r--   0        0        0      236 2023-05-26 17:11:07.789431 humanloop-0.4.5/humanloop/apis/paths/__init__.py
+-rw-r--r--   0        0        0       91 2023-05-26 17:11:07.789537 humanloop-0.4.5/humanloop/apis/paths/chat.py
+-rw-r--r--   0        0        0      108 2023-05-26 17:11:07.789639 humanloop-0.4.5/humanloop/apis/paths/chat_deployed.py
+-rw-r--r--   0        0        0      112 2023-05-26 17:11:07.789762 humanloop-0.4.5/humanloop/apis/paths/chat_experiment.py
+-rw-r--r--   0        0        0      115 2023-05-26 17:11:07.789910 humanloop-0.4.5/humanloop/apis/paths/chat_model_config.py
+-rw-r--r--   0        0        0      103 2023-05-26 17:11:07.790067 humanloop-0.4.5/humanloop/apis/paths/completion.py
+-rw-r--r--   0        0        0      120 2023-05-26 17:11:07.790221 humanloop-0.4.5/humanloop/apis/paths/completion_deployed.py
+-rw-r--r--   0        0        0      124 2023-05-26 17:11:07.790365 humanloop-0.4.5/humanloop/apis/paths/completion_experiment.py
+-rw-r--r--   0        0        0      127 2023-05-26 17:11:07.790490 humanloop-0.4.5/humanloop/apis/paths/completion_model_config.py
+-rw-r--r--   0        0        0      226 2023-05-26 17:11:07.790616 humanloop-0.4.5/humanloop/apis/paths/experiments_experiment_id.py
+-rw-r--r--   0        0        0      152 2023-05-26 17:11:07.790754 humanloop-0.4.5/humanloop/apis/paths/experiments_experiment_id_model_config.py
+-rw-r--r--   0        0        0       99 2023-05-26 17:11:07.790969 humanloop-0.4.5/humanloop/apis/paths/feedback.py
+-rw-r--r--   0        0        0      159 2023-05-26 17:11:07.791130 humanloop-0.4.5/humanloop/apis/paths/logs.py
+-rw-r--r--   0        0        0       99 2023-05-26 17:11:07.791277 humanloop-0.4.5/humanloop/apis/paths/logs_id.py
+-rw-r--r--   0        0        0      108 2023-05-26 17:11:07.791441 humanloop-0.4.5/humanloop/apis/paths/model_configs.py
+-rw-r--r--   0        0        0      110 2023-05-26 17:11:07.791587 humanloop-0.4.5/humanloop/apis/paths/model_configs_id.py
+-rw-r--r--   0        0        0      165 2023-05-26 17:11:07.791710 humanloop-0.4.5/humanloop/apis/paths/projects.py
+-rw-r--r--   0        0        0      176 2023-05-26 17:11:07.791853 humanloop-0.4.5/humanloop/apis/paths/projects_id.py
+-rw-r--r--   0        0        0      219 2023-05-26 17:11:07.792028 humanloop-0.4.5/humanloop/apis/paths/projects_id_active_config.py
+-rw-r--r--   0        0        0      144 2023-05-26 17:11:07.792165 humanloop-0.4.5/humanloop/apis/paths/projects_id_active_experiment.py
+-rw-r--r--   0        0        0      116 2023-05-26 17:11:07.792300 humanloop-0.4.5/humanloop/apis/paths/projects_id_configs.py
+-rw-r--r--   0        0        0      117 2023-05-26 17:11:07.792411 humanloop-0.4.5/humanloop/apis/paths/projects_id_export.py
+-rw-r--r--   0        0        0      135 2023-05-26 17:11:07.792584 humanloop-0.4.5/humanloop/apis/paths/projects_id_feedback_types.py
+-rw-r--r--   0        0        0      231 2023-05-26 17:11:07.792741 humanloop-0.4.5/humanloop/apis/paths/projects_project_id_experiments.py
+-rw-r--r--   0        0        0      165 2023-05-26 17:11:07.792867 humanloop-0.4.5/humanloop/apis/paths/sessions.py
+-rw-r--r--   0        0        0      101 2023-05-26 17:11:07.792984 humanloop-0.4.5/humanloop/apis/paths/sessions_id.py
+-rw-r--r--   0        0        0       95 2023-05-26 17:11:07.793097 humanloop-0.4.5/humanloop/apis/paths/traces.py
+-rw-r--r--   0        0        0     1654 2023-05-26 17:11:07.793219 humanloop-0.4.5/humanloop/apis/tag_to_api.py
+-rw-r--r--   0        0        0      572 2023-05-26 17:11:07.793342 humanloop-0.4.5/humanloop/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1006 2023-05-26 17:11:07.793443 humanloop-0.4.5/humanloop/apis/tags/chats_api.py
+-rw-r--r--   0        0        0     1020 2023-05-26 17:11:07.793539 humanloop-0.4.5/humanloop/apis/tags/completions_api.py
+-rw-r--r--   0        0        0     1091 2023-05-26 17:11:07.793630 humanloop-0.4.5/humanloop/apis/tags/experiments_api.py
+-rw-r--r--   0        0        0      721 2023-05-26 17:11:07.793719 humanloop-0.4.5/humanloop/apis/tags/feedback_api.py
+-rw-r--r--   0        0        0      852 2023-05-26 17:11:07.793839 humanloop-0.4.5/humanloop/apis/tags/logs_api.py
+-rw-r--r--   0        0        0      803 2023-05-26 17:11:07.793964 humanloop-0.4.5/humanloop/apis/tags/model_configurations_api.py
+-rw-r--r--   0        0        0     1486 2023-05-26 17:11:07.794074 humanloop-0.4.5/humanloop/apis/tags/projects_api.py
+-rw-r--r--   0        0        0      834 2023-05-26 17:11:07.794177 humanloop-0.4.5/humanloop/apis/tags/sessions_api.py
+-rw-r--r--   0        0        0      717 2023-05-26 17:11:07.794298 humanloop-0.4.5/humanloop/apis/tags/traces_api.py
+-rw-r--r--   0        0        0    28662 2023-05-26 17:11:07.794427 humanloop-0.4.5/humanloop/client.py
+-rw-r--r--   0        0        0    28662 2023-05-26 17:11:07.794585 humanloop-0.4.5/humanloop/client.pyi
+-rw-r--r--   0        0        0     6780 2023-05-26 17:11:07.866101 humanloop-0.4.5/humanloop/client_custom.py
+-rw-r--r--   0        0        0    18674 2023-05-26 17:11:07.794878 humanloop-0.4.5/humanloop/configuration.py
+-rw-r--r--   0        0        0     7678 2023-05-26 17:11:07.794996 humanloop-0.4.5/humanloop/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-05-26 17:11:07.795097 humanloop-0.4.5/humanloop/exceptions_base.py
+-rw-r--r--   0        0        0      343 2023-05-26 17:11:07.795290 humanloop-0.4.5/humanloop/model/__init__.py
+-rw-r--r--   0        0        0     9140 2023-05-26 17:11:07.795443 humanloop-0.4.5/humanloop/model/agent_config_request.py
+-rw-r--r--   0        0        0     8975 2023-05-26 17:11:07.795663 humanloop-0.4.5/humanloop/model/agent_config_request.pyi
+-rw-r--r--   0        0        0    11140 2023-05-26 17:11:07.795828 humanloop-0.4.5/humanloop/model/agent_config_response.py
+-rw-r--r--   0        0        0    11140 2023-05-26 17:11:07.795993 humanloop-0.4.5/humanloop/model/agent_config_response.pyi
+-rw-r--r--   0        0        0     6379 2023-05-26 17:11:07.796133 humanloop-0.4.5/humanloop/model/base_metric_response.py
+-rw-r--r--   0        0        0     6379 2023-05-26 17:11:07.796248 humanloop-0.4.5/humanloop/model/base_metric_response.pyi
+-rw-r--r--   0        0        0     5150 2023-05-26 17:11:07.796361 humanloop-0.4.5/humanloop/model/categorical_feedback_label.py
+-rw-r--r--   0        0        0     5150 2023-05-26 17:11:07.796474 humanloop-0.4.5/humanloop/model/categorical_feedback_label.pyi
+-rw-r--r--   0        0        0     8957 2023-05-26 17:11:07.796607 humanloop-0.4.5/humanloop/model/chat_data_response.py
+-rw-r--r--   0        0        0     8957 2023-05-26 17:11:07.796786 humanloop-0.4.5/humanloop/model/chat_data_response.pyi
+-rw-r--r--   0        0        0     9998 2023-05-26 17:11:07.796950 humanloop-0.4.5/humanloop/model/chat_deployed_request.py
+-rw-r--r--   0        0        0     9998 2023-05-26 17:11:07.797083 humanloop-0.4.5/humanloop/model/chat_deployed_request.pyi
+-rw-r--r--   0        0        0    10659 2023-05-26 17:11:07.797220 humanloop-0.4.5/humanloop/model/chat_experiment_request.py
+-rw-r--r--   0        0        0    10659 2023-05-26 17:11:07.797398 humanloop-0.4.5/humanloop/model/chat_experiment_request.pyi
+-rw-r--r--   0        0        0     3702 2023-05-26 17:11:07.797528 humanloop-0.4.5/humanloop/model/chat_message.py
+-rw-r--r--   0        0        0     3702 2023-05-26 17:11:07.797639 humanloop-0.4.5/humanloop/model/chat_message.pyi
+-rw-r--r--   0        0        0    10693 2023-05-26 17:11:07.797805 humanloop-0.4.5/humanloop/model/chat_model_config_request.py
+-rw-r--r--   0        0        0    10693 2023-05-26 17:11:07.798002 humanloop-0.4.5/humanloop/model/chat_model_config_request.pyi
+-rw-r--r--   0        0        0    12556 2023-05-26 17:11:07.798117 humanloop-0.4.5/humanloop/model/chat_request.py
+-rw-r--r--   0        0        0    12556 2023-05-26 17:11:07.798255 humanloop-0.4.5/humanloop/model/chat_request.pyi
+-rw-r--r--   0        0        0    11076 2023-05-26 17:11:07.798453 humanloop-0.4.5/humanloop/model/chat_response.py
+-rw-r--r--   0        0        0    11076 2023-05-26 17:11:07.798606 humanloop-0.4.5/humanloop/model/chat_response.pyi
+-rw-r--r--   0        0        0     1446 2023-05-26 17:11:07.798764 humanloop-0.4.5/humanloop/model/chat_role.py
+-rw-r--r--   0        0        0     1285 2023-05-26 17:11:07.798887 humanloop-0.4.5/humanloop/model/chat_role.pyi
+-rw-r--r--   0        0        0     9674 2023-05-26 17:11:07.799039 humanloop-0.4.5/humanloop/model/completion_deployed_request.py
+-rw-r--r--   0        0        0     9674 2023-05-26 17:11:07.799160 humanloop-0.4.5/humanloop/model/completion_deployed_request.pyi
+-rw-r--r--   0        0        0    10340 2023-05-26 17:11:07.799325 humanloop-0.4.5/humanloop/model/completion_experiment_request.py
+-rw-r--r--   0        0        0    10340 2023-05-26 17:11:07.799452 humanloop-0.4.5/humanloop/model/completion_experiment_request.pyi
+-rw-r--r--   0        0        0    10376 2023-05-26 17:11:07.799576 humanloop-0.4.5/humanloop/model/completion_model_config_request.py
+-rw-r--r--   0        0        0    10376 2023-05-26 17:11:07.799763 humanloop-0.4.5/humanloop/model/completion_model_config_request.pyi
+-rw-r--r--   0        0        0    12258 2023-05-26 17:11:07.799933 humanloop-0.4.5/humanloop/model/completion_request.py
+-rw-r--r--   0        0        0    12258 2023-05-26 17:11:07.800132 humanloop-0.4.5/humanloop/model/completion_request.pyi
+-rw-r--r--   0        0        0    11017 2023-05-26 17:11:07.800292 humanloop-0.4.5/humanloop/model/completion_response.py
+-rw-r--r--   0        0        0    11017 2023-05-26 17:11:07.800500 humanloop-0.4.5/humanloop/model/completion_response.pyi
+-rw-r--r--   0        0        0     2672 2023-05-26 17:11:07.800624 humanloop-0.4.5/humanloop/model/config_response.py
+-rw-r--r--   0        0        0     2672 2023-05-26 17:11:07.800783 humanloop-0.4.5/humanloop/model/config_response.pyi
+-rw-r--r--   0        0        0     1546 2023-05-26 17:11:07.800892 humanloop-0.4.5/humanloop/model/config_type.py
+-rw-r--r--   0        0        0     1361 2023-05-26 17:11:07.801013 humanloop-0.4.5/humanloop/model/config_type.pyi
+-rw-r--r--   0        0        0     6196 2023-05-26 17:11:07.801144 humanloop-0.4.5/humanloop/model/create_experiment_request.py
+-rw-r--r--   0        0        0     6196 2023-05-26 17:11:07.801264 humanloop-0.4.5/humanloop/model/create_experiment_request.pyi
+-rw-r--r--   0        0        0     3199 2023-05-26 17:11:07.801515 humanloop-0.4.5/humanloop/model/create_log_response.py
+-rw-r--r--   0        0        0     3199 2023-05-26 17:11:07.801682 humanloop-0.4.5/humanloop/model/create_log_response.pyi
+-rw-r--r--   0        0        0     4266 2023-05-26 17:11:07.801797 humanloop-0.4.5/humanloop/model/create_project_request.py
+-rw-r--r--   0        0        0     4266 2023-05-26 17:11:07.801934 humanloop-0.4.5/humanloop/model/create_project_request.pyi
+-rw-r--r--   0        0        0     2635 2023-05-26 17:11:07.802070 humanloop-0.4.5/humanloop/model/create_session_response.py
+-rw-r--r--   0        0        0     2635 2023-05-26 17:11:07.802170 humanloop-0.4.5/humanloop/model/create_session_response.pyi
+-rw-r--r--   0        0        0     3232 2023-05-26 17:11:07.802312 humanloop-0.4.5/humanloop/model/create_trace_request.py
+-rw-r--r--   0        0        0     3232 2023-05-26 17:11:07.802404 humanloop-0.4.5/humanloop/model/create_trace_request.pyi
+-rw-r--r--   0        0        0     3329 2023-05-26 17:11:07.802541 humanloop-0.4.5/humanloop/model/create_trace_response.py
+-rw-r--r--   0        0        0     3329 2023-05-26 17:11:07.802643 humanloop-0.4.5/humanloop/model/create_trace_response.pyi
+-rw-r--r--   0        0        0     7455 2023-05-26 17:11:07.802776 humanloop-0.4.5/humanloop/model/data_response.py
+-rw-r--r--   0        0        0     7455 2023-05-26 17:11:07.802870 humanloop-0.4.5/humanloop/model/data_response.pyi
+-rw-r--r--   0        0        0     8998 2023-05-26 17:11:07.803013 humanloop-0.4.5/humanloop/model/experiment_config_response.py
+-rw-r--r--   0        0        0     8998 2023-05-26 17:11:07.803160 humanloop-0.4.5/humanloop/model/experiment_config_response.pyi
+-rw-r--r--   0        0        0    12827 2023-05-26 17:11:07.803420 humanloop-0.4.5/humanloop/model/experiment_response.py
+-rw-r--r--   0        0        0    12827 2023-05-26 17:11:07.803599 humanloop-0.4.5/humanloop/model/experiment_response.pyi
+-rw-r--r--   0        0        0     1376 2023-05-26 17:11:07.803739 humanloop-0.4.5/humanloop/model/experiment_status.py
+-rw-r--r--   0        0        0     1229 2023-05-26 17:11:07.803867 humanloop-0.4.5/humanloop/model/experiment_status.pyi
+-rw-r--r--   0        0        0     1685 2023-05-26 17:11:07.803976 humanloop-0.4.5/humanloop/model/experiments_list_response.py
+-rw-r--r--   0        0        0     1685 2023-05-26 17:11:07.804194 humanloop-0.4.5/humanloop/model/experiments_list_response.pyi
+-rw-r--r--   0        0        0     6681 2023-05-26 17:11:07.804306 humanloop-0.4.5/humanloop/model/feedback.py
+-rw-r--r--   0        0        0     6681 2023-05-26 17:11:07.804406 humanloop-0.4.5/humanloop/model/feedback.pyi
+-rw-r--r--   0        0        0     1463 2023-05-26 17:11:07.804498 humanloop-0.4.5/humanloop/model/feedback_class.py
+-rw-r--r--   0        0        0     1296 2023-05-26 17:11:07.804641 humanloop-0.4.5/humanloop/model/feedback_class.pyi
+-rw-r--r--   0        0        0     3334 2023-05-26 17:11:07.804733 humanloop-0.4.5/humanloop/model/feedback_label_request.py
+-rw-r--r--   0        0        0     3334 2023-05-26 17:11:07.804874 humanloop-0.4.5/humanloop/model/feedback_label_request.pyi
+-rw-r--r--   0        0        0     7189 2023-05-26 17:11:07.805025 humanloop-0.4.5/humanloop/model/feedback_request.py
+-rw-r--r--   0        0        0     7189 2023-05-26 17:11:07.805176 humanloop-0.4.5/humanloop/model/feedback_request.pyi
+-rw-r--r--   0        0        0     7141 2023-05-26 17:11:07.805286 humanloop-0.4.5/humanloop/model/feedback_response.py
+-rw-r--r--   0        0        0     7141 2023-05-26 17:11:07.805387 humanloop-0.4.5/humanloop/model/feedback_response.pyi
+-rw-r--r--   0        0        0     3200 2023-05-26 17:11:07.805506 humanloop-0.4.5/humanloop/model/feedback_submit_request.py
+-rw-r--r--   0        0        0     3200 2023-05-26 17:11:07.805613 humanloop-0.4.5/humanloop/model/feedback_submit_request.pyi
+-rw-r--r--   0        0        0     3210 2023-05-26 17:11:07.805720 humanloop-0.4.5/humanloop/model/feedback_submit_response.py
+-rw-r--r--   0        0        0     3210 2023-05-26 17:11:07.805812 humanloop-0.4.5/humanloop/model/feedback_submit_response.pyi
+-rw-r--r--   0        0        0     1690 2023-05-26 17:11:07.805924 humanloop-0.4.5/humanloop/model/feedback_type.py
+-rw-r--r--   0        0        0     1459 2023-05-26 17:11:07.806087 humanloop-0.4.5/humanloop/model/feedback_type.pyi
+-rw-r--r--   0        0        0     6161 2023-05-26 17:11:07.806238 humanloop-0.4.5/humanloop/model/feedback_type_model.py
+-rw-r--r--   0        0        0     6161 2023-05-26 17:11:07.806362 humanloop-0.4.5/humanloop/model/feedback_type_model.pyi
+-rw-r--r--   0        0        0     6289 2023-05-26 17:11:07.806503 humanloop-0.4.5/humanloop/model/feedback_type_request.py
+-rw-r--r--   0        0        0     6289 2023-05-26 17:11:07.806633 humanloop-0.4.5/humanloop/model/feedback_type_request.pyi
+-rw-r--r--   0        0        0     1659 2023-05-26 17:11:07.806767 humanloop-0.4.5/humanloop/model/feedback_types.py
+-rw-r--r--   0        0        0     1659 2023-05-26 17:11:07.806887 humanloop-0.4.5/humanloop/model/feedback_types.pyi
+-rw-r--r--   0        0        0     4407 2023-05-26 17:11:07.807008 humanloop-0.4.5/humanloop/model/generic_config_request.py
+-rw-r--r--   0        0        0     4238 2023-05-26 17:11:07.807147 humanloop-0.4.5/humanloop/model/generic_config_request.pyi
+-rw-r--r--   0        0        0     6562 2023-05-26 17:11:07.807259 humanloop-0.4.5/humanloop/model/generic_config_response.py
+-rw-r--r--   0        0        0     6562 2023-05-26 17:11:07.807372 humanloop-0.4.5/humanloop/model/generic_config_response.pyi
+-rw-r--r--   0        0        0     9619 2023-05-26 17:11:07.807479 humanloop-0.4.5/humanloop/model/get_model_config_response.py
+-rw-r--r--   0        0        0     9619 2023-05-26 17:11:07.807618 humanloop-0.4.5/humanloop/model/get_model_config_response.pyi
+-rw-r--r--   0        0        0     3611 2023-05-26 17:11:07.807730 humanloop-0.4.5/humanloop/model/http_validation_error.py
+-rw-r--r--   0        0        0     3611 2023-05-26 17:11:07.807827 humanloop-0.4.5/humanloop/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     1667 2023-05-26 17:11:07.807914 humanloop-0.4.5/humanloop/model/label_sentiment.py
+-rw-r--r--   0        0        0     1468 2023-05-26 17:11:07.808008 humanloop-0.4.5/humanloop/model/label_sentiment.pyi
+-rw-r--r--   0        0        0     3156 2023-05-26 17:11:07.808107 humanloop-0.4.5/humanloop/model/log_datapoint_request.py
+-rw-r--r--   0        0        0     3156 2023-05-26 17:11:07.808199 humanloop-0.4.5/humanloop/model/log_datapoint_request.pyi
+-rw-r--r--   0        0        0    17219 2023-05-26 17:11:07.808302 humanloop-0.4.5/humanloop/model/log_model_config_request.py
+-rw-r--r--   0        0        0    17219 2023-05-26 17:11:07.808427 humanloop-0.4.5/humanloop/model/log_model_config_request.pyi
+-rw-r--r--   0        0        0    17749 2023-05-26 17:11:07.808544 humanloop-0.4.5/humanloop/model/log_request.py
+-rw-r--r--   0        0        0    17749 2023-05-26 17:11:07.809096 humanloop-0.4.5/humanloop/model/log_request.pyi
+-rw-r--r--   0        0        0    22101 2023-05-26 17:11:07.809251 humanloop-0.4.5/humanloop/model/log_response.py
+-rw-r--r--   0        0        0    22101 2023-05-26 17:11:07.809386 humanloop-0.4.5/humanloop/model/log_response.pyi
+-rw-r--r--   0        0        0     3205 2023-05-26 17:11:07.809503 humanloop-0.4.5/humanloop/model/logs_log_response.py
+-rw-r--r--   0        0        0     3205 2023-05-26 17:11:07.809626 humanloop-0.4.5/humanloop/model/logs_log_response.pyi
+-rw-r--r--   0        0        0    16246 2023-05-26 17:11:07.809743 humanloop-0.4.5/humanloop/model/model_config_chat_request.py
+-rw-r--r--   0        0        0    16246 2023-05-26 17:11:07.809902 humanloop-0.4.5/humanloop/model/model_config_chat_request.pyi
+-rw-r--r--   0        0        0    15386 2023-05-26 17:11:07.810046 humanloop-0.4.5/humanloop/model/model_config_completion_request.py
+-rw-r--r--   0        0        0    15386 2023-05-26 17:11:07.810214 humanloop-0.4.5/humanloop/model/model_config_completion_request.pyi
+-rw-r--r--   0        0        0    17859 2023-05-26 17:11:07.810390 humanloop-0.4.5/humanloop/model/model_config_response.py
+-rw-r--r--   0        0        0    17859 2023-05-26 17:11:07.810560 humanloop-0.4.5/humanloop/model/model_config_response.pyi
+-rw-r--r--   0        0        0    20554 2023-05-26 17:11:07.810727 humanloop-0.4.5/humanloop/model/model_config_response2.py
+-rw-r--r--   0        0        0    20554 2023-05-26 17:11:07.810904 humanloop-0.4.5/humanloop/model/model_config_response2.pyi
+-rw-r--r--   0        0        0     1460 2023-05-26 17:11:07.811049 humanloop-0.4.5/humanloop/model/model_endpoints.py
+-rw-r--r--   0        0        0     1305 2023-05-26 17:11:07.811188 humanloop-0.4.5/humanloop/model/model_endpoints.pyi
+-rw-r--r--   0        0        0     1809 2023-05-26 17:11:07.811314 humanloop-0.4.5/humanloop/model/model_providers.py
+-rw-r--r--   0        0        0     1550 2023-05-26 17:11:07.811445 humanloop-0.4.5/humanloop/model/model_providers.pyi
+-rw-r--r--   0        0        0     5144 2023-05-26 17:11:07.811572 humanloop-0.4.5/humanloop/model/paginated_data_log_response.py
+-rw-r--r--   0        0        0     5144 2023-05-26 17:11:07.811709 humanloop-0.4.5/humanloop/model/paginated_data_log_response.pyi
+-rw-r--r--   0        0        0     5180 2023-05-26 17:11:07.811838 humanloop-0.4.5/humanloop/model/paginated_data_project_response.py
+-rw-r--r--   0        0        0     5180 2023-05-26 17:11:07.811964 humanloop-0.4.5/humanloop/model/paginated_data_project_response.pyi
+-rw-r--r--   0        0        0     5180 2023-05-26 17:11:07.812081 humanloop-0.4.5/humanloop/model/paginated_data_session_response.py
+-rw-r--r--   0        0        0     5180 2023-05-26 17:11:07.812201 humanloop-0.4.5/humanloop/model/paginated_data_session_response.pyi
+-rw-r--r--   0        0        0     3143 2023-05-26 17:11:07.812317 humanloop-0.4.5/humanloop/model/positive_label.py
+-rw-r--r--   0        0        0     3143 2023-05-26 17:11:07.812454 humanloop-0.4.5/humanloop/model/positive_label.pyi
+-rw-r--r--   0        0        0     8900 2023-05-26 17:11:07.812563 humanloop-0.4.5/humanloop/model/project_config_response.py
+-rw-r--r--   0        0        0     8900 2023-05-26 17:11:07.812674 humanloop-0.4.5/humanloop/model/project_config_response.pyi
+-rw-r--r--   0        0        0    18363 2023-05-26 17:11:07.812792 humanloop-0.4.5/humanloop/model/project_model_config_request.py
+-rw-r--r--   0        0        0    18363 2023-05-26 17:11:07.812903 humanloop-0.4.5/humanloop/model/project_model_config_request.pyi
+-rw-r--r--   0        0        0    23968 2023-05-26 17:11:07.813022 humanloop-0.4.5/humanloop/model/project_model_config_response.py
+-rw-r--r--   0        0        0    23968 2023-05-26 17:11:07.813134 humanloop-0.4.5/humanloop/model/project_model_config_response.pyi
+-rw-r--r--   0        0        0    13895 2023-05-26 17:11:07.813238 humanloop-0.4.5/humanloop/model/project_response.py
+-rw-r--r--   0        0        0    13895 2023-05-26 17:11:07.813355 humanloop-0.4.5/humanloop/model/project_response.pyi
+-rw-r--r--   0        0        0     1471 2023-05-26 17:11:07.813462 humanloop-0.4.5/humanloop/model/project_sort_by.py
+-rw-r--r--   0        0        0     1300 2023-05-26 17:11:07.813556 humanloop-0.4.5/humanloop/model/project_sort_by.pyi
+-rw-r--r--   0        0        0     3795 2023-05-26 17:11:07.813647 humanloop-0.4.5/humanloop/model/project_user_response.py
+-rw-r--r--   0        0        0     3795 2023-05-26 17:11:07.813763 humanloop-0.4.5/humanloop/model/project_user_response.pyi
+-rw-r--r--   0        0        0     1713 2023-05-26 17:11:07.813856 humanloop-0.4.5/humanloop/model/projects_get_configs_response.py
+-rw-r--r--   0        0        0     1713 2023-05-26 17:11:07.813963 humanloop-0.4.5/humanloop/model/projects_get_configs_response.pyi
+-rw-r--r--   0        0        0     1715 2023-05-26 17:11:07.814055 humanloop-0.4.5/humanloop/model/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0     1715 2023-05-26 17:11:07.814144 humanloop-0.4.5/humanloop/model/projects_update_feedback_types_request.pyi
+-rw-r--r--   0        0        0     4655 2023-05-26 17:11:07.814231 humanloop-0.4.5/humanloop/model/provider_api_keys.py
+-rw-r--r--   0        0        0     4655 2023-05-26 17:11:07.814337 humanloop-0.4.5/humanloop/model/provider_api_keys.pyi
+-rw-r--r--   0        0        0     3113 2023-05-26 17:11:07.814440 humanloop-0.4.5/humanloop/model/session_project_response.py
+-rw-r--r--   0        0        0     3113 2023-05-26 17:11:07.814529 humanloop-0.4.5/humanloop/model/session_project_response.pyi
+-rw-r--r--   0        0        0     6620 2023-05-26 17:11:07.814652 humanloop-0.4.5/humanloop/model/session_response.py
+-rw-r--r--   0        0        0     6620 2023-05-26 17:11:07.814790 humanloop-0.4.5/humanloop/model/session_response.pyi
+-rw-r--r--   0        0        0     1309 2023-05-26 17:11:07.814902 humanloop-0.4.5/humanloop/model/sort_order.py
+-rw-r--r--   0        0        0     1192 2023-05-26 17:11:07.815013 humanloop-0.4.5/humanloop/model/sort_order.pyi
+-rw-r--r--   0        0        0     4889 2023-05-26 17:11:07.815147 humanloop-0.4.5/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4889 2023-05-26 17:11:07.815271 humanloop-0.4.5/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0     4893 2023-05-26 17:11:07.815404 humanloop-0.4.5/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4893 2023-05-26 17:11:07.815542 humanloop-0.4.5/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0     4948 2023-05-26 17:11:07.815682 humanloop-0.4.5/humanloop/model/tool_config_request.py
+-rw-r--r--   0        0        0     4785 2023-05-26 17:11:07.815820 humanloop-0.4.5/humanloop/model/tool_config_request.pyi
+-rw-r--r--   0        0        0     7061 2023-05-26 17:11:07.815948 humanloop-0.4.5/humanloop/model/tool_config_response.py
+-rw-r--r--   0        0        0     7061 2023-05-26 17:11:07.816084 humanloop-0.4.5/humanloop/model/tool_config_response.pyi
+-rw-r--r--   0        0        0     4232 2023-05-26 17:11:07.816213 humanloop-0.4.5/humanloop/model/tool_result_response.py
+-rw-r--r--   0        0        0     4232 2023-05-26 17:11:07.816347 humanloop-0.4.5/humanloop/model/tool_result_response.pyi
+-rw-r--r--   0        0        0    13077 2023-05-26 17:11:07.816501 humanloop-0.4.5/humanloop/model/trace_log_request.py
+-rw-r--r--   0        0        0    13077 2023-05-26 17:11:07.816669 humanloop-0.4.5/humanloop/model/trace_log_request.pyi
+-rw-r--r--   0        0        0    19510 2023-05-26 17:11:07.816857 humanloop-0.4.5/humanloop/model/trace_model_config_request.py
+-rw-r--r--   0        0        0    19345 2023-05-26 17:11:07.817010 humanloop-0.4.5/humanloop/model/trace_model_config_request.pyi
+-rw-r--r--   0        0        0     7302 2023-05-26 17:11:07.817146 humanloop-0.4.5/humanloop/model/update_experiment_request.py
+-rw-r--r--   0        0        0     7302 2023-05-26 17:11:07.817264 humanloop-0.4.5/humanloop/model/update_experiment_request.pyi
+-rw-r--r--   0        0        0     3142 2023-05-26 17:11:07.817375 humanloop-0.4.5/humanloop/model/update_log_request.py
+-rw-r--r--   0        0        0     3142 2023-05-26 17:11:07.817484 humanloop-0.4.5/humanloop/model/update_log_request.pyi
+-rw-r--r--   0        0        0     5047 2023-05-26 17:11:07.817598 humanloop-0.4.5/humanloop/model/update_project_request.py
+-rw-r--r--   0        0        0     5047 2023-05-26 17:11:07.817706 humanloop-0.4.5/humanloop/model/update_project_request.pyi
+-rw-r--r--   0        0        0     4118 2023-05-26 17:11:07.817810 humanloop-0.4.5/humanloop/model/usage.py
+-rw-r--r--   0        0        0     4118 2023-05-26 17:11:07.817916 humanloop-0.4.5/humanloop/model/usage.pyi
+-rw-r--r--   0        0        0     6805 2023-05-26 17:11:07.818033 humanloop-0.4.5/humanloop/model/validation_error.py
+-rw-r--r--   0        0        0     6805 2023-05-26 17:11:07.818147 humanloop-0.4.5/humanloop/model/validation_error.pyi
+-rw-r--r--   0        0        0     6443 2023-05-26 17:11:07.818270 humanloop-0.4.5/humanloop/models/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-26 17:11:07.818362 humanloop-0.4.5/humanloop/paths/__init__.py
+-rw-r--r--   0        0        0      285 2023-05-26 17:11:07.818454 humanloop-0.4.5/humanloop/paths/chat/__init__.py
+-rw-r--r--   0        0        0    17428 2023-05-26 17:11:07.818554 humanloop-0.4.5/humanloop/paths/chat/post.py
+-rw-r--r--   0        0        0    17285 2023-05-26 17:11:07.818668 humanloop-0.4.5/humanloop/paths/chat/post.pyi
+-rw-r--r--   0        0        0      302 2023-05-26 17:11:07.818772 humanloop-0.4.5/humanloop/paths/chat_deployed/__init__.py
+-rw-r--r--   0        0        0    16991 2023-05-26 17:11:07.818868 humanloop-0.4.5/humanloop/paths/chat_deployed/post.py
+-rw-r--r--   0        0        0    16848 2023-05-26 17:11:07.819116 humanloop-0.4.5/humanloop/paths/chat_deployed/post.pyi
+-rw-r--r--   0        0        0      306 2023-05-26 17:11:07.819300 humanloop-0.4.5/humanloop/paths/chat_experiment/__init__.py
+-rw-r--r--   0        0        0    17434 2023-05-26 17:11:07.819422 humanloop-0.4.5/humanloop/paths/chat_experiment/post.py
+-rw-r--r--   0        0        0    17291 2023-05-26 17:11:07.819573 humanloop-0.4.5/humanloop/paths/chat_experiment/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-26 17:11:07.819777 humanloop-0.4.5/humanloop/paths/chat_model_config/__init__.py
+-rw-r--r--   0        0        0    17609 2023-05-26 17:11:07.819934 humanloop-0.4.5/humanloop/paths/chat_model_config/post.py
+-rw-r--r--   0        0        0    17466 2023-05-26 17:11:07.820193 humanloop-0.4.5/humanloop/paths/chat_model_config/post.pyi
+-rw-r--r--   0        0        0      297 2023-05-26 17:11:07.820429 humanloop-0.4.5/humanloop/paths/completion/__init__.py
+-rw-r--r--   0        0        0    17744 2023-05-26 17:11:07.820561 humanloop-0.4.5/humanloop/paths/completion/post.py
+-rw-r--r--   0        0        0    17601 2023-05-26 17:11:07.820706 humanloop-0.4.5/humanloop/paths/completion/post.pyi
+-rw-r--r--   0        0        0      314 2023-05-26 17:11:07.820822 humanloop-0.4.5/humanloop/paths/completion_deployed/__init__.py
+-rw-r--r--   0        0        0    17247 2023-05-26 17:11:07.820931 humanloop-0.4.5/humanloop/paths/completion_deployed/post.py
+-rw-r--r--   0        0        0    17104 2023-05-26 17:11:07.821156 humanloop-0.4.5/humanloop/paths/completion_deployed/post.pyi
+-rw-r--r--   0        0        0      318 2023-05-26 17:11:07.821285 humanloop-0.4.5/humanloop/paths/completion_experiment/__init__.py
+-rw-r--r--   0        0        0    17690 2023-05-26 17:11:07.821484 humanloop-0.4.5/humanloop/paths/completion_experiment/post.py
+-rw-r--r--   0        0        0    17547 2023-05-26 17:11:07.821648 humanloop-0.4.5/humanloop/paths/completion_experiment/post.pyi
+-rw-r--r--   0        0        0      321 2023-05-26 17:11:07.821833 humanloop-0.4.5/humanloop/paths/completion_model_config/__init__.py
+-rw-r--r--   0        0        0    17865 2023-05-26 17:11:07.822002 humanloop-0.4.5/humanloop/paths/completion_model_config/post.py
+-rw-r--r--   0        0        0    17722 2023-05-26 17:11:07.822155 humanloop-0.4.5/humanloop/paths/completion_model_config/post.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 17:11:07.822350 humanloop-0.4.5/humanloop/paths/experiments_experiment_id/__init__.py
+-rw-r--r--   0        0        0    11995 2023-05-26 17:11:07.822497 humanloop-0.4.5/humanloop/paths/experiments_experiment_id/delete.py
+-rw-r--r--   0        0        0    11852 2023-05-26 17:11:07.822699 humanloop-0.4.5/humanloop/paths/experiments_experiment_id/delete.pyi
+-rw-r--r--   0        0        0    17043 2023-05-26 17:11:07.822826 humanloop-0.4.5/humanloop/paths/experiments_experiment_id/patch.py
+-rw-r--r--   0        0        0    16900 2023-05-26 17:11:07.822999 humanloop-0.4.5/humanloop/paths/experiments_experiment_id/patch.pyi
+-rw-r--r--   0        0        0      352 2023-05-26 17:11:07.823104 humanloop-0.4.5/humanloop/paths/experiments_experiment_id_model_config/__init__.py
+-rw-r--r--   0        0        0    12496 2023-05-26 17:11:07.823225 humanloop-0.4.5/humanloop/paths/experiments_experiment_id_model_config/get.py
+-rw-r--r--   0        0        0    12353 2023-05-26 17:11:07.823405 humanloop-0.4.5/humanloop/paths/experiments_experiment_id_model_config/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-26 17:11:07.823560 humanloop-0.4.5/humanloop/paths/feedback/__init__.py
+-rw-r--r--   0        0        0    15089 2023-05-26 17:11:07.823661 humanloop-0.4.5/humanloop/paths/feedback/post.py
+-rw-r--r--   0        0        0    14946 2023-05-26 17:11:07.823806 humanloop-0.4.5/humanloop/paths/feedback/post.pyi
+-rw-r--r--   0        0        0      285 2023-05-26 17:11:07.823919 humanloop-0.4.5/humanloop/paths/logs/__init__.py
+-rw-r--r--   0        0        0    15728 2023-05-26 17:11:07.824019 humanloop-0.4.5/humanloop/paths/logs/patch.py
+-rw-r--r--   0        0        0    15585 2023-05-26 17:11:07.824128 humanloop-0.4.5/humanloop/paths/logs/patch.pyi
+-rw-r--r--   0        0        0    22622 2023-05-26 17:11:07.824247 humanloop-0.4.5/humanloop/paths/logs/post.py
+-rw-r--r--   0        0        0    22479 2023-05-26 17:11:07.824372 humanloop-0.4.5/humanloop/paths/logs/post.pyi
+-rw-r--r--   0        0        0      291 2023-05-26 17:11:07.824481 humanloop-0.4.5/humanloop/paths/logs_id/__init__.py
+-rw-r--r--   0        0        0    14794 2023-05-26 17:11:07.824578 humanloop-0.4.5/humanloop/paths/logs_id/patch.py
+-rw-r--r--   0        0        0    14651 2023-05-26 17:11:07.824694 humanloop-0.4.5/humanloop/paths/logs_id/patch.pyi
+-rw-r--r--   0        0        0      302 2023-05-26 17:11:07.824812 humanloop-0.4.5/humanloop/paths/model_configs/__init__.py
+-rw-r--r--   0        0        0    20266 2023-05-26 17:11:07.824985 humanloop-0.4.5/humanloop/paths/model_configs/post.py
+-rw-r--r--   0        0        0    20123 2023-05-26 17:11:07.825127 humanloop-0.4.5/humanloop/paths/model_configs/post.pyi
+-rw-r--r--   0        0        0      308 2023-05-26 17:11:07.825267 humanloop-0.4.5/humanloop/paths/model_configs_id/__init__.py
+-rw-r--r--   0        0        0    12023 2023-05-26 17:11:07.825387 humanloop-0.4.5/humanloop/paths/model_configs_id/get.py
+-rw-r--r--   0        0        0    11880 2023-05-26 17:11:07.825538 humanloop-0.4.5/humanloop/paths/model_configs_id/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-26 17:11:07.825687 humanloop-0.4.5/humanloop/paths/projects/__init__.py
+-rw-r--r--   0        0        0    20518 2023-05-26 17:11:07.825810 humanloop-0.4.5/humanloop/paths/projects/get.py
+-rw-r--r--   0        0        0    20375 2023-05-26 17:11:07.826010 humanloop-0.4.5/humanloop/paths/projects/get.pyi
+-rw-r--r--   0        0        0    13007 2023-05-26 17:11:07.826143 humanloop-0.4.5/humanloop/paths/projects/post.py
+-rw-r--r--   0        0        0    12864 2023-05-26 17:11:07.826307 humanloop-0.4.5/humanloop/paths/projects/post.pyi
+-rw-r--r--   0        0        0      299 2023-05-26 17:11:07.826429 humanloop-0.4.5/humanloop/paths/projects_id/__init__.py
+-rw-r--r--   0        0        0    11979 2023-05-26 17:11:07.826605 humanloop-0.4.5/humanloop/paths/projects_id/get.py
+-rw-r--r--   0        0        0    11836 2023-05-26 17:11:07.826765 humanloop-0.4.5/humanloop/paths/projects_id/get.pyi
+-rw-r--r--   0        0        0    16066 2023-05-26 17:11:07.826912 humanloop-0.4.5/humanloop/paths/projects_id/patch.py
+-rw-r--r--   0        0        0    15923 2023-05-26 17:11:07.827078 humanloop-0.4.5/humanloop/paths/projects_id/patch.pyi
+-rw-r--r--   0        0        0      326 2023-05-26 17:11:07.827409 humanloop-0.4.5/humanloop/paths/projects_id_active_config/__init__.py
+-rw-r--r--   0        0        0    12298 2023-05-26 17:11:07.827531 humanloop-0.4.5/humanloop/paths/projects_id_active_config/delete.py
+-rw-r--r--   0        0        0    12155 2023-05-26 17:11:07.827720 humanloop-0.4.5/humanloop/paths/projects_id_active_config/delete.pyi
+-rw-r--r--   0        0        0    12148 2023-05-26 17:11:07.827893 humanloop-0.4.5/humanloop/paths/projects_id_active_config/get.py
+-rw-r--r--   0        0        0    12005 2023-05-26 17:11:07.828039 humanloop-0.4.5/humanloop/paths/projects_id_active_config/get.pyi
+-rw-r--r--   0        0        0      334 2023-05-26 17:11:07.828179 humanloop-0.4.5/humanloop/paths/projects_id_active_experiment/__init__.py
+-rw-r--r--   0        0        0    12306 2023-05-26 17:11:07.828318 humanloop-0.4.5/humanloop/paths/projects_id_active_experiment/delete.py
+-rw-r--r--   0        0        0    12163 2023-05-26 17:11:07.828467 humanloop-0.4.5/humanloop/paths/projects_id_active_experiment/delete.pyi
+-rw-r--r--   0        0        0      315 2023-05-26 17:11:07.828612 humanloop-0.4.5/humanloop/paths/projects_id_configs/__init__.py
+-rw-r--r--   0        0        0    12182 2023-05-26 17:11:07.828723 humanloop-0.4.5/humanloop/paths/projects_id_configs/get.py
+-rw-r--r--   0        0        0    12039 2023-05-26 17:11:07.828851 humanloop-0.4.5/humanloop/paths/projects_id_configs/get.pyi
+-rw-r--r--   0        0        0      313 2023-05-26 17:11:07.828981 humanloop-0.4.5/humanloop/paths/projects_id_export/__init__.py
+-rw-r--r--   0        0        0    15728 2023-05-26 17:11:07.829131 humanloop-0.4.5/humanloop/paths/projects_id_export/post.py
+-rw-r--r--   0        0        0    15585 2023-05-26 17:11:07.829289 humanloop-0.4.5/humanloop/paths/projects_id_export/post.pyi
+-rw-r--r--   0        0        0      328 2023-05-26 17:11:07.829414 humanloop-0.4.5/humanloop/paths/projects_id_feedback_types/__init__.py
+-rw-r--r--   0        0        0    14798 2023-05-26 17:11:07.829519 humanloop-0.4.5/humanloop/paths/projects_id_feedback_types/patch.py
+-rw-r--r--   0        0        0    14655 2023-05-26 17:11:07.829661 humanloop-0.4.5/humanloop/paths/projects_id_feedback_types/patch.pyi
+-rw-r--r--   0        0        0      339 2023-05-26 17:11:07.829791 humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/__init__.py
+-rw-r--r--   0        0        0    12256 2023-05-26 17:11:07.829899 humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/get.py
+-rw-r--r--   0        0        0    12113 2023-05-26 17:11:07.830031 humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/get.pyi
+-rw-r--r--   0        0        0    16250 2023-05-26 17:11:07.830187 humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/post.py
+-rw-r--r--   0        0        0    16107 2023-05-26 17:11:07.830328 humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/post.pyi
+-rw-r--r--   0        0        0      293 2023-05-26 17:11:07.830490 humanloop-0.4.5/humanloop/paths/sessions/__init__.py
+-rw-r--r--   0        0        0    14112 2023-05-26 17:11:07.830608 humanloop-0.4.5/humanloop/paths/sessions/get.py
+-rw-r--r--   0        0        0    13969 2023-05-26 17:11:07.830749 humanloop-0.4.5/humanloop/paths/sessions/get.pyi
+-rw-r--r--   0        0        0     9192 2023-05-26 17:11:07.830947 humanloop-0.4.5/humanloop/paths/sessions/post.py
+-rw-r--r--   0        0        0     9079 2023-05-26 17:11:07.831123 humanloop-0.4.5/humanloop/paths/sessions/post.pyi
+-rw-r--r--   0        0        0      299 2023-05-26 17:11:07.831289 humanloop-0.4.5/humanloop/paths/sessions_id/__init__.py
+-rw-r--r--   0        0        0    11979 2023-05-26 17:11:07.831437 humanloop-0.4.5/humanloop/paths/sessions_id/get.py
+-rw-r--r--   0        0        0    11836 2023-05-26 17:11:07.831609 humanloop-0.4.5/humanloop/paths/sessions_id/get.pyi
+-rw-r--r--   0        0        0      289 2023-05-26 17:11:07.831772 humanloop-0.4.5/humanloop/paths/traces/__init__.py
+-rw-r--r--   0        0        0    12450 2023-05-26 17:11:07.831896 humanloop-0.4.5/humanloop/paths/traces/post.py
+-rw-r--r--   0        0        0    12307 2023-05-26 17:11:07.832045 humanloop-0.4.5/humanloop/paths/traces/post.pyi
+-rw-r--r--   0        0        0     1011 2023-05-26 17:11:07.832184 humanloop-0.4.5/humanloop/request_after_hook.py
+-rw-r--r--   0        0        0     1783 2023-05-26 17:11:07.866300 humanloop-0.4.5/humanloop/request_before_hook.py
+-rw-r--r--   0        0        0    11329 2023-05-26 17:11:07.832376 humanloop-0.4.5/humanloop/rest.py
+-rw-r--r--   0        0        0    95913 2023-05-26 17:11:07.832563 humanloop-0.4.5/humanloop/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-26 17:11:07.832693 humanloop-0.4.5/humanloop/type/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-26 17:11:07.832795 humanloop-0.4.5/humanloop/type/agent_config_request.py
+-rw-r--r--   0        0        0     1608 2023-05-26 17:11:07.832891 humanloop-0.4.5/humanloop/type/agent_config_response.py
+-rw-r--r--   0        0        0     1408 2023-05-26 17:11:07.832982 humanloop-0.4.5/humanloop/type/base_metric_response.py
+-rw-r--r--   0        0        0     1062 2023-05-26 17:11:07.833073 humanloop-0.4.5/humanloop/type/categorical_feedback_label.py
+-rw-r--r--   0        0        0     2183 2023-05-26 17:11:07.833167 humanloop-0.4.5/humanloop/type/chat_data_response.py
+-rw-r--r--   0        0        0     1990 2023-05-26 17:11:07.833276 humanloop-0.4.5/humanloop/type/chat_deployed_request.py
+-rw-r--r--   0        0        0     2235 2023-05-26 17:11:07.833366 humanloop-0.4.5/humanloop/type/chat_experiment_request.py
+-rw-r--r--   0        0        0      919 2023-05-26 17:11:07.833454 humanloop-0.4.5/humanloop/type/chat_message.py
+-rw-r--r--   0        0        0     2104 2023-05-26 17:11:07.833544 humanloop-0.4.5/humanloop/type/chat_model_config_request.py
+-rw-r--r--   0        0        0     2130 2023-05-26 17:11:07.833636 humanloop-0.4.5/humanloop/type/chat_request.py
+-rw-r--r--   0        0        0     1818 2023-05-26 17:11:07.833741 humanloop-0.4.5/humanloop/type/chat_response.py
+-rw-r--r--   0        0        0      711 2023-05-26 17:11:07.833831 humanloop-0.4.5/humanloop/type/chat_role.py
+-rw-r--r--   0        0        0     2095 2023-05-26 17:11:07.833947 humanloop-0.4.5/humanloop/type/completion_deployed_request.py
+-rw-r--r--   0        0        0     2343 2023-05-26 17:11:07.834066 humanloop-0.4.5/humanloop/type/completion_experiment_request.py
+-rw-r--r--   0        0        0     2209 2023-05-26 17:11:07.834186 humanloop-0.4.5/humanloop/type/completion_model_config_request.py
+-rw-r--r--   0        0        0     2239 2023-05-26 17:11:07.834292 humanloop-0.4.5/humanloop/type/completion_request.py
+-rw-r--r--   0        0        0     1864 2023-05-26 17:11:07.834406 humanloop-0.4.5/humanloop/type/completion_response.py
+-rw-r--r--   0        0        0     1054 2023-05-26 17:11:07.834509 humanloop-0.4.5/humanloop/type/config_response.py
+-rw-r--r--   0        0        0      719 2023-05-26 17:11:07.834616 humanloop-0.4.5/humanloop/type/config_type.py
+-rw-r--r--   0        0        0     1362 2023-05-26 17:11:07.834716 humanloop-0.4.5/humanloop/type/create_experiment_request.py
+-rw-r--r--   0        0        0     1024 2023-05-26 17:11:07.834814 humanloop-0.4.5/humanloop/type/create_log_response.py
+-rw-r--r--   0        0        0     1066 2023-05-26 17:11:07.834926 humanloop-0.4.5/humanloop/type/create_project_request.py
+-rw-r--r--   0        0        0      942 2023-05-26 17:11:07.835016 humanloop-0.4.5/humanloop/type/create_session_response.py
+-rw-r--r--   0        0        0     1045 2023-05-26 17:11:07.835134 humanloop-0.4.5/humanloop/type/create_trace_request.py
+-rw-r--r--   0        0        0      998 2023-05-26 17:11:07.835255 humanloop-0.4.5/humanloop/type/create_trace_response.py
+-rw-r--r--   0        0        0     2013 2023-05-26 17:11:07.835364 humanloop-0.4.5/humanloop/type/data_response.py
+-rw-r--r--   0        0        0     1677 2023-05-26 17:11:07.835469 humanloop-0.4.5/humanloop/type/experiment_config_response.py
+-rw-r--r--   0        0        0     1788 2023-05-26 17:11:07.835586 humanloop-0.4.5/humanloop/type/experiment_response.py
+-rw-r--r--   0        0        0      718 2023-05-26 17:11:07.835706 humanloop-0.4.5/humanloop/type/experiment_status.py
+-rw-r--r--   0        0        0      785 2023-05-26 17:11:07.835823 humanloop-0.4.5/humanloop/type/experiments_list_response.py
+-rw-r--r--   0        0        0     1449 2023-05-26 17:11:07.835963 humanloop-0.4.5/humanloop/type/feedback.py
+-rw-r--r--   0        0        0      719 2023-05-26 17:11:07.836091 humanloop-0.4.5/humanloop/type/feedback_class.py
+-rw-r--r--   0        0        0      970 2023-05-26 17:11:07.836218 humanloop-0.4.5/humanloop/type/feedback_label_request.py
+-rw-r--r--   0        0        0     1546 2023-05-26 17:11:07.836334 humanloop-0.4.5/humanloop/type/feedback_request.py
+-rw-r--r--   0        0        0     1578 2023-05-26 17:11:07.836435 humanloop-0.4.5/humanloop/type/feedback_response.py
+-rw-r--r--   0        0        0      804 2023-05-26 17:11:07.836549 humanloop-0.4.5/humanloop/type/feedback_submit_request.py
+-rw-r--r--   0        0        0      809 2023-05-26 17:11:07.836659 humanloop-0.4.5/humanloop/type/feedback_submit_response.py
+-rw-r--r--   0        0        0      738 2023-05-26 17:11:07.838710 humanloop-0.4.5/humanloop/type/feedback_type.py
+-rw-r--r--   0        0        0     1307 2023-05-26 17:11:07.838903 humanloop-0.4.5/humanloop/type/feedback_type_model.py
+-rw-r--r--   0        0        0     1541 2023-05-26 17:11:07.839029 humanloop-0.4.5/humanloop/type/feedback_type_request.py
+-rw-r--r--   0        0        0      773 2023-05-26 17:11:07.839162 humanloop-0.4.5/humanloop/type/feedback_types.py
+-rw-r--r--   0        0        0     1064 2023-05-26 17:11:07.839275 humanloop-0.4.5/humanloop/type/generic_config_request.py
+-rw-r--r--   0        0        0     1262 2023-05-26 17:11:07.839383 humanloop-0.4.5/humanloop/type/generic_config_response.py
+-rw-r--r--   0        0        0     1900 2023-05-26 17:11:07.839494 humanloop-0.4.5/humanloop/type/get_model_config_response.py
+-rw-r--r--   0        0        0      972 2023-05-26 17:11:07.839601 humanloop-0.4.5/humanloop/type/http_validation_error.py
+-rw-r--r--   0        0        0      730 2023-05-26 17:11:07.839698 humanloop-0.4.5/humanloop/type/label_sentiment.py
+-rw-r--r--   0        0        0      782 2023-05-26 17:11:07.839781 humanloop-0.4.5/humanloop/type/log_datapoint_request.py
+-rw-r--r--   0        0        0     3033 2023-05-26 17:11:07.839863 humanloop-0.4.5/humanloop/type/log_model_config_request.py
+-rw-r--r--   0        0        0     3681 2023-05-26 17:11:07.839942 humanloop-0.4.5/humanloop/type/log_request.py
+-rw-r--r--   0        0        0     3872 2023-05-26 17:11:07.840024 humanloop-0.4.5/humanloop/type/log_response.py
+-rw-r--r--   0        0        0      807 2023-05-26 17:11:07.840205 humanloop-0.4.5/humanloop/type/logs_log_response.py
+-rw-r--r--   0        0        0     2820 2023-05-26 17:11:07.840315 humanloop-0.4.5/humanloop/type/model_config_chat_request.py
+-rw-r--r--   0        0        0     2713 2023-05-26 17:11:07.840442 humanloop-0.4.5/humanloop/type/model_config_completion_request.py
+-rw-r--r--   0        0        0     3160 2023-05-26 17:11:07.840646 humanloop-0.4.5/humanloop/type/model_config_response.py
+-rw-r--r--   0        0        0     3281 2023-05-26 17:11:07.840790 humanloop-0.4.5/humanloop/type/model_config_response2.py
+-rw-r--r--   0        0        0      714 2023-05-26 17:11:07.840930 humanloop-0.4.5/humanloop/type/model_endpoints.py
+-rw-r--r--   0        0        0      748 2023-05-26 17:11:07.841076 humanloop-0.4.5/humanloop/type/model_providers.py
+-rw-r--r--   0        0        0     1032 2023-05-26 17:11:07.841202 humanloop-0.4.5/humanloop/type/paginated_data_log_response.py
+-rw-r--r--   0        0        0     1064 2023-05-26 17:11:07.841330 humanloop-0.4.5/humanloop/type/paginated_data_project_response.py
+-rw-r--r--   0        0        0     1064 2023-05-26 17:11:07.841471 humanloop-0.4.5/humanloop/type/paginated_data_session_response.py
+-rw-r--r--   0        0        0      871 2023-05-26 17:11:07.841618 humanloop-0.4.5/humanloop/type/positive_label.py
+-rw-r--r--   0        0        0     1820 2023-05-26 17:11:07.841745 humanloop-0.4.5/humanloop/type/project_config_response.py
+-rw-r--r--   0        0        0     3410 2023-05-26 17:11:07.841904 humanloop-0.4.5/humanloop/type/project_model_config_request.py
+-rw-r--r--   0        0        0     4053 2023-05-26 17:11:07.842030 humanloop-0.4.5/humanloop/type/project_model_config_response.py
+-rw-r--r--   0        0        0     2032 2023-05-26 17:11:07.842153 humanloop-0.4.5/humanloop/type/project_response.py
+-rw-r--r--   0        0        0      721 2023-05-26 17:11:07.842301 humanloop-0.4.5/humanloop/type/project_sort_by.py
+-rw-r--r--   0        0        0     1022 2023-05-26 17:11:07.842430 humanloop-0.4.5/humanloop/type/project_user_response.py
+-rw-r--r--   0        0        0      798 2023-05-26 17:11:07.842590 humanloop-0.4.5/humanloop/type/projects_get_configs_response.py
+-rw-r--r--   0        0        0      800 2023-05-26 17:11:07.842735 humanloop-0.4.5/humanloop/type/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0      934 2023-05-26 17:11:07.842835 humanloop-0.4.5/humanloop/type/provider_api_keys.py
+-rw-r--r--   0        0        0      985 2023-05-26 17:11:07.842938 humanloop-0.4.5/humanloop/type/session_project_response.py
+-rw-r--r--   0        0        0     1442 2023-05-26 17:11:07.843078 humanloop-0.4.5/humanloop/type/session_response.py
+-rw-r--r--   0        0        0      696 2023-05-26 17:11:07.843181 humanloop-0.4.5/humanloop/type/sort_order.py
+-rw-r--r--   0        0        0     1241 2023-05-26 17:11:07.843303 humanloop-0.4.5/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     1251 2023-05-26 17:11:07.843412 humanloop-0.4.5/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     1066 2023-05-26 17:11:07.843500 humanloop-0.4.5/humanloop/type/tool_config_request.py
+-rw-r--r--   0        0        0     1295 2023-05-26 17:11:07.843585 humanloop-0.4.5/humanloop/type/tool_config_response.py
+-rw-r--r--   0        0        0      930 2023-05-26 17:11:07.843709 humanloop-0.4.5/humanloop/type/tool_result_response.py
+-rw-r--r--   0        0        0     2456 2023-05-26 17:11:07.843814 humanloop-0.4.5/humanloop/type/trace_log_request.py
+-rw-r--r--   0        0        0     3095 2023-05-26 17:11:07.843926 humanloop-0.4.5/humanloop/type/trace_model_config_request.py
+-rw-r--r--   0        0        0     1361 2023-05-26 17:11:07.844033 humanloop-0.4.5/humanloop/type/update_experiment_request.py
+-rw-r--r--   0        0        0      996 2023-05-26 17:11:07.844156 humanloop-0.4.5/humanloop/type/update_log_request.py
+-rw-r--r--   0        0        0     1434 2023-05-26 17:11:07.844253 humanloop-0.4.5/humanloop/type/update_project_request.py
+-rw-r--r--   0        0        0     1042 2023-05-26 17:11:07.844387 humanloop-0.4.5/humanloop/type/usage.py
+-rw-r--r--   0        0        0      951 2023-05-26 17:11:07.844481 humanloop-0.4.5/humanloop/type/validation_error.py
+-rw-r--r--   0        0        0      868 2023-05-26 17:11:07.844614 humanloop-0.4.5/humanloop/type_util.py
+-rw-r--r--   0        0        0     3165 2023-05-26 17:11:07.844730 humanloop-0.4.5/humanloop/validation_metadata.py
+-rw-r--r--   0        0        0      714 2023-05-26 17:11:07.845128 humanloop-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     9366 1970-01-01 00:00:00.000000 humanloop-0.4.5/PKG-INFO
```

### Comparing `humanloop-0.4.4/LICENSE` & `humanloop-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/README.md` & `humanloop-0.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# humanloop@0.4.4
+# humanloop@0.4.5
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.4
+pip install humanloop==0.4.5
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
```

### Comparing `humanloop-0.4.4/humanloop/__init__.py` & `humanloop-0.4.5/humanloop/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 # import ApiClient
 from humanloop.api_client import ApiClient
 
 # import Configuration
 from humanloop.configuration import Configuration
```

### Comparing `humanloop-0.4.4/humanloop/api_client.py` & `humanloop-0.4.5/humanloop/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2759,15 +2759,15 @@
 0000ac60: 6164 6572 5f6e 616d 655d 203d 2068 6561  ader_name] = hea
 0000ac70: 6465 725f 7661 6c75 650a 2020 2020 2020  der_value.      
 0000ac80: 2020 7365 6c66 2e63 6f6f 6b69 6520 3d20    self.cookie = 
 0000ac90: 636f 6f6b 6965 0a20 2020 2020 2020 2023  cookie.        #
 0000aca0: 2053 6574 2064 6566 6175 6c74 2055 7365   Set default Use
 0000acb0: 722d 4167 656e 742e 0a20 2020 2020 2020  r-Agent..       
 0000acc0: 2073 656c 662e 7573 6572 5f61 6765 6e74   self.user_agent
-0000acd0: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e34   = 'Konfig/0.4.4
+0000acd0: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e35   = 'Konfig/0.4.5
 0000ace0: 2f70 7974 686f 6e27 0a0a 2020 2020 6465  /python'..    de
 0000acf0: 6620 5f5f 656e 7465 725f 5f28 7365 6c66  f __enter__(self
 0000ad00: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
 0000ad10: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
 0000ad20: 5f5f 6578 6974 5f5f 2873 656c 662c 2065  __exit__(self, e
 0000ad30: 7863 5f74 7970 652c 2065 7863 5f76 616c  xc_type, exc_val
 0000ad40: 7565 2c20 7472 6163 6562 6163 6b29 3a0a  ue, traceback):.
```

### Comparing `humanloop-0.4.4/humanloop/api_response.py` & `humanloop-0.4.5/humanloop/api_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/apis/path_to_api.py` & `humanloop-0.4.5/humanloop/apis/path_to_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from humanloop.apis.paths.completion_experiment import CompletionExperiment
 from humanloop.apis.paths.completion_model_config import CompletionModelConfig
 from humanloop.apis.paths.chat import Chat
 from humanloop.apis.paths.chat_deployed import ChatDeployed
 from humanloop.apis.paths.chat_experiment import ChatExperiment
 from humanloop.apis.paths.chat_model_config import ChatModelConfig
 from humanloop.apis.paths.logs import Logs
+from humanloop.apis.paths.logs_id import LogsId
 from humanloop.apis.paths.feedback import Feedback
 from humanloop.apis.paths.projects import Projects
 from humanloop.apis.paths.projects_id import ProjectsId
 from humanloop.apis.paths.projects_id_configs import ProjectsIdConfigs
 from humanloop.apis.paths.projects_id_active_config import ProjectsIdActiveConfig
 from humanloop.apis.paths.projects_id_active_experiment import ProjectsIdActiveExperiment
 from humanloop.apis.paths.projects_id_feedback_types import ProjectsIdFeedbackTypes
@@ -35,14 +36,15 @@
         PathValues.COMPLETIONEXPERIMENT: CompletionExperiment,
         PathValues.COMPLETIONMODELCONFIG: CompletionModelConfig,
         PathValues.CHAT: Chat,
         PathValues.CHATDEPLOYED: ChatDeployed,
         PathValues.CHATEXPERIMENT: ChatExperiment,
         PathValues.CHATMODELCONFIG: ChatModelConfig,
         PathValues.LOGS: Logs,
+        PathValues.LOGS_ID: LogsId,
         PathValues.FEEDBACK: Feedback,
         PathValues.PROJECTS: Projects,
         PathValues.PROJECTS_ID: ProjectsId,
         PathValues.PROJECTS_ID_CONFIGS: ProjectsIdConfigs,
         PathValues.PROJECTS_ID_ACTIVECONFIG: ProjectsIdActiveConfig,
         PathValues.PROJECTS_ID_ACTIVEEXPERIMENT: ProjectsIdActiveExperiment,
         PathValues.PROJECTS_ID_FEEDBACKTYPES: ProjectsIdFeedbackTypes,
@@ -65,14 +67,15 @@
         PathValues.COMPLETIONEXPERIMENT: CompletionExperiment,
         PathValues.COMPLETIONMODELCONFIG: CompletionModelConfig,
         PathValues.CHAT: Chat,
         PathValues.CHATDEPLOYED: ChatDeployed,
         PathValues.CHATEXPERIMENT: ChatExperiment,
         PathValues.CHATMODELCONFIG: ChatModelConfig,
         PathValues.LOGS: Logs,
+        PathValues.LOGS_ID: LogsId,
         PathValues.FEEDBACK: Feedback,
         PathValues.PROJECTS: Projects,
         PathValues.PROJECTS_ID: ProjectsId,
         PathValues.PROJECTS_ID_CONFIGS: ProjectsIdConfigs,
         PathValues.PROJECTS_ID_ACTIVECONFIG: ProjectsIdActiveConfig,
         PathValues.PROJECTS_ID_ACTIVEEXPERIMENT: ProjectsIdActiveExperiment,
         PathValues.PROJECTS_ID_FEEDBACKTYPES: ProjectsIdFeedbackTypes,
```

### Comparing `humanloop-0.4.4/humanloop/apis/tag_to_api.py` & `humanloop-0.4.5/humanloop/apis/tag_to_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import typing_extensions
 
 from humanloop.apis.tags import TagValues
 from humanloop.apis.tags.projects_api import ProjectsApi
 from humanloop.apis.tags.experiments_api import ExperimentsApi
 from humanloop.apis.tags.completions_api import CompletionsApi
 from humanloop.apis.tags.chats_api import ChatsApi
+from humanloop.apis.tags.logs_api import LogsApi
 from humanloop.apis.tags.sessions_api import SessionsApi
 from humanloop.apis.tags.model_configurations_api import ModelConfigurationsApi
-from humanloop.apis.tags.logs_api import LogsApi
 from humanloop.apis.tags.feedback_api import FeedbackApi
 from humanloop.apis.tags.traces_api import TracesApi
 from humanloop.apis.tags.authentication_api import AuthenticationApi
 
 TagToApi = typing_extensions.TypedDict(
     'TagToApi',
     {
         TagValues.PROJECTS: ProjectsApi,
         TagValues.EXPERIMENTS: ExperimentsApi,
         TagValues.COMPLETIONS: CompletionsApi,
         TagValues.CHATS: ChatsApi,
+        TagValues.LOGS: LogsApi,
         TagValues.SESSIONS: SessionsApi,
         TagValues.MODEL_CONFIGURATIONS: ModelConfigurationsApi,
-        TagValues.LOGS: LogsApi,
         TagValues.FEEDBACK: FeedbackApi,
         TagValues.TRACES: TracesApi,
         TagValues.AUTHENTICATION: AuthenticationApi,
     }
 )
 
 tag_to_api = TagToApi(
     {
         TagValues.PROJECTS: ProjectsApi,
         TagValues.EXPERIMENTS: ExperimentsApi,
         TagValues.COMPLETIONS: CompletionsApi,
         TagValues.CHATS: ChatsApi,
+        TagValues.LOGS: LogsApi,
         TagValues.SESSIONS: SessionsApi,
         TagValues.MODEL_CONFIGURATIONS: ModelConfigurationsApi,
-        TagValues.LOGS: LogsApi,
         TagValues.FEEDBACK: FeedbackApi,
         TagValues.TRACES: TracesApi,
         TagValues.AUTHENTICATION: AuthenticationApi,
     }
 )
```

### Comparing `humanloop-0.4.4/humanloop/apis/tags/__init__.py` & `humanloop-0.4.5/humanloop/apis/tags/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 
 
 class TagValues(str, enum.Enum):
     PROJECTS = "Projects"
     EXPERIMENTS = "Experiments"
     COMPLETIONS = "Completions"
     CHATS = "Chats"
+    LOGS = "Logs"
     SESSIONS = "Sessions"
     MODEL_CONFIGURATIONS = "Model Configurations"
-    LOGS = "Logs"
     FEEDBACK = "Feedback"
     TRACES = "Traces"
     AUTHENTICATION = "Authentication"
```

### Comparing `humanloop-0.4.4/humanloop/apis/tags/chats_api.py` & `humanloop-0.4.5/humanloop/apis/tags/chats_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/apis/tags/completions_api.py` & `humanloop-0.4.5/humanloop/apis/tags/completions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/apis/tags/experiments_api.py` & `humanloop-0.4.5/humanloop/apis/tags/experiments_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/apis/tags/feedback_api.py` & `humanloop-0.4.5/humanloop/apis/tags/feedback_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/apis/tags/logs_api.py` & `humanloop-0.4.5/humanloop/apis/tags/traces_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-from humanloop.paths.logs.post import Log
+from humanloop.paths.traces.post import Create
 
 
-class LogsApi(
-    Log,
+class TracesApi(
+    Create,
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
     pass
```

### Comparing `humanloop-0.4.4/humanloop/apis/tags/model_configurations_api.py` & `humanloop-0.4.5/humanloop/apis/tags/model_configurations_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/apis/tags/projects_api.py` & `humanloop-0.4.5/humanloop/apis/tags/projects_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/apis/tags/sessions_api.py` & `humanloop-0.4.5/humanloop/apis/tags/sessions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/apis/tags/traces_api.py` & `humanloop-0.4.5/humanloop/type/model_endpoints.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-from humanloop.paths.traces.post import Create
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
 
-class TracesApi(
-    Create,
-):
-    """NOTE:
-    This class is auto generated by Konfig (https://konfigthis.com)
-    """
-    pass
+ModelEndpoints = Literal["complete", "chat", "edit"]
```

### Comparing `humanloop-0.4.4/humanloop/client.py` & `humanloop-0.4.5/humanloop/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -580,16 +580,19 @@
         )
 
     @copy_signature(LogsApi.alog)
     async def alog(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -597,16 +600,19 @@
         created_at: typing.Optional[datetime] = None,
         error: typing.Optional[str] = None,
         duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         return await self.logs_api.alog(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
@@ -617,16 +623,19 @@
         )
 
     @copy_signature(LogsApi.log)
     def log(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -634,16 +643,19 @@
         created_at: typing.Optional[datetime] = None,
         error: typing.Optional[str] = None,
         duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         return self.logs_api.log(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
```

### Comparing `humanloop-0.4.4/humanloop/client.pyi` & `humanloop-0.4.5/humanloop/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -580,16 +580,19 @@
         )
 
     @copy_signature(LogsApi.alog)
     async def alog(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -597,16 +600,19 @@
         created_at: typing.Optional[datetime] = None,
         error: typing.Optional[str] = None,
         duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         return await self.logs_api.alog(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
@@ -617,16 +623,19 @@
         )
 
     @copy_signature(LogsApi.log)
     def log(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -634,16 +643,19 @@
         created_at: typing.Optional[datetime] = None,
         error: typing.Optional[str] = None,
         duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         return self.logs_api.log(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
```

### Comparing `humanloop-0.4.4/humanloop/client_custom.py` & `humanloop-0.4.5/humanloop/client_custom.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/configuration.py` & `humanloop-0.4.5/humanloop/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 4.0.0\n"\
-               "SDK Package Version: 0.4.4".\
+               "SDK Package Version: 0.4.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `humanloop-0.4.4/humanloop/exceptions.py` & `humanloop-0.4.5/humanloop/exceptions.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/exceptions_base.py` & `humanloop-0.4.5/humanloop/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/agent_config_request.py` & `humanloop-0.4.5/humanloop/model/agent_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/agent_config_request.pyi` & `humanloop-0.4.5/humanloop/model/agent_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/agent_config_response.py` & `humanloop-0.4.5/humanloop/model/agent_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/agent_config_response.pyi` & `humanloop-0.4.5/humanloop/model/agent_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/base_metric_response.py` & `humanloop-0.4.5/humanloop/model/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/base_metric_response.pyi` & `humanloop-0.4.5/humanloop/model/base_metric_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/categorical_feedback_label.py` & `humanloop-0.4.5/humanloop/model/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/categorical_feedback_label.pyi` & `humanloop-0.4.5/humanloop/model/categorical_feedback_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_data_response.py` & `humanloop-0.4.5/humanloop/model/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_data_response.pyi` & `humanloop-0.4.5/humanloop/model/chat_data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_deployed_request.py` & `humanloop-0.4.5/humanloop/model/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_deployed_request.pyi` & `humanloop-0.4.5/humanloop/model/chat_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_experiment_request.py` & `humanloop-0.4.5/humanloop/model/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_experiment_request.pyi` & `humanloop-0.4.5/humanloop/model/chat_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_message.py` & `humanloop-0.4.5/humanloop/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_message.pyi` & `humanloop-0.4.5/humanloop/model/chat_message.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_model_config_request.py` & `humanloop-0.4.5/humanloop/model/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_model_config_request.pyi` & `humanloop-0.4.5/humanloop/model/chat_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_request.py` & `humanloop-0.4.5/humanloop/model/chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_request.pyi` & `humanloop-0.4.5/humanloop/model/chat_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_response.py` & `humanloop-0.4.5/humanloop/model/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_response.pyi` & `humanloop-0.4.5/humanloop/model/chat_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_role.py` & `humanloop-0.4.5/humanloop/model/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/chat_role.pyi` & `humanloop-0.4.5/humanloop/model/chat_role.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_deployed_request.py` & `humanloop-0.4.5/humanloop/model/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_deployed_request.pyi` & `humanloop-0.4.5/humanloop/model/completion_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_experiment_request.py` & `humanloop-0.4.5/humanloop/model/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_experiment_request.pyi` & `humanloop-0.4.5/humanloop/model/completion_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_model_config_request.py` & `humanloop-0.4.5/humanloop/model/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_model_config_request.pyi` & `humanloop-0.4.5/humanloop/model/completion_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_request.py` & `humanloop-0.4.5/humanloop/model/completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_request.pyi` & `humanloop-0.4.5/humanloop/model/completion_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_response.py` & `humanloop-0.4.5/humanloop/model/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/completion_response.pyi` & `humanloop-0.4.5/humanloop/model/completion_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/config_response.py` & `humanloop-0.4.5/humanloop/model/config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/config_response.pyi` & `humanloop-0.4.5/humanloop/model/config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/config_type.py` & `humanloop-0.4.5/humanloop/model/config_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/config_type.pyi` & `humanloop-0.4.5/humanloop/model/config_type.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_experiment_request.py` & `humanloop-0.4.5/humanloop/model/create_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_experiment_request.pyi` & `humanloop-0.4.5/humanloop/model/create_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_log_response.py` & `humanloop-0.4.5/humanloop/model/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_log_response.pyi` & `humanloop-0.4.5/humanloop/model/create_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_project_request.py` & `humanloop-0.4.5/humanloop/model/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_project_request.pyi` & `humanloop-0.4.5/humanloop/model/create_project_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_session_response.py` & `humanloop-0.4.5/humanloop/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_session_response.pyi` & `humanloop-0.4.5/humanloop/model/create_session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_trace_request.py` & `humanloop-0.4.5/humanloop/model/create_trace_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_trace_request.pyi` & `humanloop-0.4.5/humanloop/model/create_trace_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_trace_response.py` & `humanloop-0.4.5/humanloop/model/create_trace_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/create_trace_response.pyi` & `humanloop-0.4.5/humanloop/model/create_trace_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/data_response.py` & `humanloop-0.4.5/humanloop/model/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/data_response.pyi` & `humanloop-0.4.5/humanloop/model/data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/experiment_config_response.py` & `humanloop-0.4.5/humanloop/model/experiment_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/experiment_config_response.pyi` & `humanloop-0.4.5/humanloop/model/experiment_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/experiment_response.py` & `humanloop-0.4.5/humanloop/model/experiment_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/experiment_response.pyi` & `humanloop-0.4.5/humanloop/model/experiment_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/experiment_status.py` & `humanloop-0.4.5/humanloop/model/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/experiment_status.pyi` & `humanloop-0.4.5/humanloop/model/experiment_status.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/experiments_list_response.py` & `humanloop-0.4.5/humanloop/model/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/experiments_list_response.pyi` & `humanloop-0.4.5/humanloop/model/experiments_list_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback.py` & `humanloop-0.4.5/humanloop/model/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback.pyi` & `humanloop-0.4.5/humanloop/model/feedback.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_class.py` & `humanloop-0.4.5/humanloop/model/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_class.pyi` & `humanloop-0.4.5/humanloop/model/feedback_class.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_label_request.py` & `humanloop-0.4.5/humanloop/model/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_label_request.pyi` & `humanloop-0.4.5/humanloop/model/feedback_label_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_request.py` & `humanloop-0.4.5/humanloop/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_request.pyi` & `humanloop-0.4.5/humanloop/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_response.py` & `humanloop-0.4.5/humanloop/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_response.pyi` & `humanloop-0.4.5/humanloop/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_submit_request.py` & `humanloop-0.4.5/humanloop/model/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_submit_request.pyi` & `humanloop-0.4.5/humanloop/model/feedback_submit_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_submit_response.py` & `humanloop-0.4.5/humanloop/model/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_submit_response.pyi` & `humanloop-0.4.5/humanloop/model/feedback_submit_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_type.py` & `humanloop-0.4.5/humanloop/model/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_type.pyi` & `humanloop-0.4.5/humanloop/model/feedback_type.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_type_model.py` & `humanloop-0.4.5/humanloop/model/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_type_model.pyi` & `humanloop-0.4.5/humanloop/model/feedback_type_model.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_type_request.py` & `humanloop-0.4.5/humanloop/model/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_type_request.pyi` & `humanloop-0.4.5/humanloop/model/feedback_type_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_types.py` & `humanloop-0.4.5/humanloop/model/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/feedback_types.pyi` & `humanloop-0.4.5/humanloop/model/feedback_types.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/generic_config_request.py` & `humanloop-0.4.5/humanloop/model/generic_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/generic_config_request.pyi` & `humanloop-0.4.5/humanloop/model/generic_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/generic_config_response.py` & `humanloop-0.4.5/humanloop/model/generic_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/generic_config_response.pyi` & `humanloop-0.4.5/humanloop/model/generic_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/get_model_config_response.py` & `humanloop-0.4.5/humanloop/model/get_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/get_model_config_response.pyi` & `humanloop-0.4.5/humanloop/model/get_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/http_validation_error.py` & `humanloop-0.4.5/humanloop/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/http_validation_error.pyi` & `humanloop-0.4.5/humanloop/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/label_sentiment.py` & `humanloop-0.4.5/humanloop/model/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/label_sentiment.pyi` & `humanloop-0.4.5/humanloop/model/label_sentiment.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/log_datapoint_request.py` & `humanloop-0.4.5/humanloop/model/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/log_datapoint_request.pyi` & `humanloop-0.4.5/humanloop/model/log_datapoint_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/log_model_config_request.py` & `humanloop-0.4.5/humanloop/model/log_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/log_model_config_request.pyi` & `humanloop-0.4.5/humanloop/model/log_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/log_request.py` & `humanloop-0.4.5/humanloop/model/log_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,23 +28,22 @@
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
-        required = {
-            "output",
-        }
         
         class properties:
-            output = schemas.StrSchema
             project = schemas.StrSchema
+            reference_id = schemas.StrSchema
             session_id = schemas.StrSchema
+            session_reference_id = schemas.StrSchema
             parent_id = schemas.StrSchema
+            parent_reference_id = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
             class messages(
                 schemas.ListSchema
             ):
@@ -65,14 +64,15 @@
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
+            output = schemas.StrSchema
             source = schemas.StrSchema
             
             
             class config(
                 schemas.ComposedSchema,
             ):
             
@@ -173,54 +173,64 @@
                         _configuration=_configuration,
                         **kwargs,
                     )
             created_at = schemas.DateTimeSchema
             error = schemas.StrSchema
             duration = schemas.NumberSchema
             __annotations__ = {
-                "output": output,
                 "project": project,
+                "reference_id": reference_id,
                 "session_id": session_id,
+                "session_reference_id": session_reference_id,
                 "parent_id": parent_id,
+                "parent_reference_id": parent_reference_id,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
+                "output": output,
                 "source": source,
                 "config": config,
                 "metadata": metadata,
                 "feedback": feedback,
                 "created_at": created_at,
                 "error": error,
                 "duration": duration,
             }
     
-    output: MetaOapg.properties.output
-    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def __getitem__(self, name: typing_extensions.Literal["reference_id"]) -> MetaOapg.properties.reference_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["session_reference_id"]) -> MetaOapg.properties.session_reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parent_id"]) -> MetaOapg.properties.parent_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["parent_reference_id"]) -> MetaOapg.properties.parent_reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
@@ -236,41 +246,50 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["output", "project", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "reference_id", "session_id", "session_reference_id", "parent_id", "parent_reference_id", "trial_id", "inputs", "messages", "output", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> typing.Union[MetaOapg.properties.project, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> typing.Union[MetaOapg.properties.project, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["reference_id"]) -> typing.Union[MetaOapg.properties.reference_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> typing.Union[MetaOapg.properties.session_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["session_reference_id"]) -> typing.Union[MetaOapg.properties.session_reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parent_id"]) -> typing.Union[MetaOapg.properties.parent_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["parent_reference_id"]) -> typing.Union[MetaOapg.properties.parent_reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
@@ -286,48 +305,54 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["output", "project", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "reference_id", "session_id", "session_reference_id", "parent_id", "parent_reference_id", "trial_id", "inputs", "messages", "output", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        output: typing.Union[MetaOapg.properties.output, str, ],
         project: typing.Union[MetaOapg.properties.project, str, schemas.Unset] = schemas.unset,
+        reference_id: typing.Union[MetaOapg.properties.reference_id, str, schemas.Unset] = schemas.unset,
         session_id: typing.Union[MetaOapg.properties.session_id, str, schemas.Unset] = schemas.unset,
+        session_reference_id: typing.Union[MetaOapg.properties.session_reference_id, str, schemas.Unset] = schemas.unset,
         parent_id: typing.Union[MetaOapg.properties.parent_id, str, schemas.Unset] = schemas.unset,
+        parent_reference_id: typing.Union[MetaOapg.properties.parent_reference_id, str, schemas.Unset] = schemas.unset,
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
+        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         feedback: typing.Union[MetaOapg.properties.feedback, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
         error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
         duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'LogRequest':
         return super().__new__(
             cls,
             *args,
-            output=output,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
+            output=output,
             source=source,
             config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
             error=error,
             duration=duration,
```

### Comparing `humanloop-0.4.4/humanloop/model/log_request.pyi` & `humanloop-0.4.5/humanloop/model/log_request.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -28,23 +28,22 @@
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
-        required = {
-            "output",
-        }
         
         class properties:
-            output = schemas.StrSchema
             project = schemas.StrSchema
+            reference_id = schemas.StrSchema
             session_id = schemas.StrSchema
+            session_reference_id = schemas.StrSchema
             parent_id = schemas.StrSchema
+            parent_reference_id = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
             class messages(
                 schemas.ListSchema
             ):
@@ -65,14 +64,15 @@
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
+            output = schemas.StrSchema
             source = schemas.StrSchema
             
             
             class config(
                 schemas.ComposedSchema,
             ):
             
@@ -173,54 +173,64 @@
                         _configuration=_configuration,
                         **kwargs,
                     )
             created_at = schemas.DateTimeSchema
             error = schemas.StrSchema
             duration = schemas.NumberSchema
             __annotations__ = {
-                "output": output,
                 "project": project,
+                "reference_id": reference_id,
                 "session_id": session_id,
+                "session_reference_id": session_reference_id,
                 "parent_id": parent_id,
+                "parent_reference_id": parent_reference_id,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
+                "output": output,
                 "source": source,
                 "config": config,
                 "metadata": metadata,
                 "feedback": feedback,
                 "created_at": created_at,
                 "error": error,
                 "duration": duration,
             }
     
-    output: MetaOapg.properties.output
-    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def __getitem__(self, name: typing_extensions.Literal["reference_id"]) -> MetaOapg.properties.reference_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["session_reference_id"]) -> MetaOapg.properties.session_reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parent_id"]) -> MetaOapg.properties.parent_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["parent_reference_id"]) -> MetaOapg.properties.parent_reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
@@ -236,41 +246,50 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["output", "project", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "reference_id", "session_id", "session_reference_id", "parent_id", "parent_reference_id", "trial_id", "inputs", "messages", "output", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> typing.Union[MetaOapg.properties.project, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> typing.Union[MetaOapg.properties.project, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["reference_id"]) -> typing.Union[MetaOapg.properties.reference_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> typing.Union[MetaOapg.properties.session_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["session_reference_id"]) -> typing.Union[MetaOapg.properties.session_reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parent_id"]) -> typing.Union[MetaOapg.properties.parent_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["parent_reference_id"]) -> typing.Union[MetaOapg.properties.parent_reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
@@ -286,48 +305,54 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["output", "project", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "reference_id", "session_id", "session_reference_id", "parent_id", "parent_reference_id", "trial_id", "inputs", "messages", "output", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        output: typing.Union[MetaOapg.properties.output, str, ],
         project: typing.Union[MetaOapg.properties.project, str, schemas.Unset] = schemas.unset,
+        reference_id: typing.Union[MetaOapg.properties.reference_id, str, schemas.Unset] = schemas.unset,
         session_id: typing.Union[MetaOapg.properties.session_id, str, schemas.Unset] = schemas.unset,
+        session_reference_id: typing.Union[MetaOapg.properties.session_reference_id, str, schemas.Unset] = schemas.unset,
         parent_id: typing.Union[MetaOapg.properties.parent_id, str, schemas.Unset] = schemas.unset,
+        parent_reference_id: typing.Union[MetaOapg.properties.parent_reference_id, str, schemas.Unset] = schemas.unset,
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
+        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         feedback: typing.Union[MetaOapg.properties.feedback, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
         error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
         duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'LogRequest':
         return super().__new__(
             cls,
             *args,
-            output=output,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
+            output=output,
             source=source,
             config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
             error=error,
             duration=duration,
```

### Comparing `humanloop-0.4.4/humanloop/model/log_response.py` & `humanloop-0.4.5/humanloop/model/log_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,32 +29,33 @@
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "output",
             "project_id",
             "project",
             "id",
             "config",
         }
         
         class properties:
             project = schemas.StrSchema
-            output = schemas.StrSchema
         
             @staticmethod
             def config() -> typing.Type['ConfigResponse']:
                 return ConfigResponse
             id = schemas.StrSchema
             project_id = schemas.StrSchema
+            reference_id = schemas.StrSchema
             session_id = schemas.StrSchema
+            session_reference_id = schemas.StrSchema
             parent_id = schemas.StrSchema
+            parent_reference_id = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
             class messages(
                 schemas.ListSchema
             ):
@@ -75,14 +76,15 @@
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
+            output = schemas.StrSchema
             source = schemas.StrSchema
             metadata = schemas.DictSchema
             
             
             class feedback(
                 schemas.ComposedSchema,
             ):
@@ -186,74 +188,85 @@
             user = schemas.StrSchema
             provider_response = schemas.DictSchema
             provider_latency = schemas.NumberSchema
             raw_output = schemas.StrSchema
             finish_reason = schemas.StrSchema
             __annotations__ = {
                 "project": project,
-                "output": output,
                 "config": config,
                 "id": id,
                 "project_id": project_id,
+                "reference_id": reference_id,
                 "session_id": session_id,
+                "session_reference_id": session_reference_id,
                 "parent_id": parent_id,
+                "parent_reference_id": parent_reference_id,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
+                "output": output,
                 "source": source,
                 "metadata": metadata,
                 "feedback": feedback,
                 "created_at": created_at,
                 "error": error,
                 "duration": duration,
                 "model_config": model_config,
                 "user": user,
                 "provider_response": provider_response,
                 "provider_latency": provider_latency,
                 "raw_output": raw_output,
                 "finish_reason": finish_reason,
             }
     
-    output: MetaOapg.properties.output
     project_id: MetaOapg.properties.project_id
     project: MetaOapg.properties.project
     id: MetaOapg.properties.id
     config: 'ConfigResponse'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["config"]) -> 'ConfigResponse': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["reference_id"]) -> MetaOapg.properties.reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["session_reference_id"]) -> MetaOapg.properties.session_reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parent_id"]) -> MetaOapg.properties.parent_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["parent_reference_id"]) -> MetaOapg.properties.parent_reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["feedback"]) -> MetaOapg.properties.feedback: ...
@@ -284,50 +297,59 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["finish_reason"]) -> MetaOapg.properties.finish_reason: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "output", "config", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "config", "id", "project_id", "reference_id", "session_id", "session_reference_id", "parent_id", "parent_reference_id", "trial_id", "inputs", "messages", "output", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> 'ConfigResponse': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["reference_id"]) -> typing.Union[MetaOapg.properties.reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> typing.Union[MetaOapg.properties.session_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["session_reference_id"]) -> typing.Union[MetaOapg.properties.session_reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parent_id"]) -> typing.Union[MetaOapg.properties.parent_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["parent_reference_id"]) -> typing.Union[MetaOapg.properties.parent_reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["feedback"]) -> typing.Union[MetaOapg.properties.feedback, schemas.Unset]: ...
@@ -358,31 +380,34 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["finish_reason"]) -> typing.Union[MetaOapg.properties.finish_reason, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "output", "config", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "config", "id", "project_id", "reference_id", "session_id", "session_reference_id", "parent_id", "parent_reference_id", "trial_id", "inputs", "messages", "output", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        output: typing.Union[MetaOapg.properties.output, str, ],
         project_id: typing.Union[MetaOapg.properties.project_id, str, ],
         project: typing.Union[MetaOapg.properties.project, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         config: 'ConfigResponse',
+        reference_id: typing.Union[MetaOapg.properties.reference_id, str, schemas.Unset] = schemas.unset,
         session_id: typing.Union[MetaOapg.properties.session_id, str, schemas.Unset] = schemas.unset,
+        session_reference_id: typing.Union[MetaOapg.properties.session_reference_id, str, schemas.Unset] = schemas.unset,
         parent_id: typing.Union[MetaOapg.properties.parent_id, str, schemas.Unset] = schemas.unset,
+        parent_reference_id: typing.Union[MetaOapg.properties.parent_reference_id, str, schemas.Unset] = schemas.unset,
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
+        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         feedback: typing.Union[MetaOapg.properties.feedback, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
         error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
         duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -393,24 +418,27 @@
         finish_reason: typing.Union[MetaOapg.properties.finish_reason, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'LogResponse':
         return super().__new__(
             cls,
             *args,
-            output=output,
             project_id=project_id,
             project=project,
             id=id,
             config=config,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
+            output=output,
             source=source,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
             error=error,
             duration=duration,
             model_config=model_config,
```

### Comparing `humanloop-0.4.4/humanloop/model/log_response.pyi` & `humanloop-0.4.5/humanloop/model/log_response.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,32 +29,33 @@
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "output",
             "project_id",
             "project",
             "id",
             "config",
         }
         
         class properties:
             project = schemas.StrSchema
-            output = schemas.StrSchema
         
             @staticmethod
             def config() -> typing.Type['ConfigResponse']:
                 return ConfigResponse
             id = schemas.StrSchema
             project_id = schemas.StrSchema
+            reference_id = schemas.StrSchema
             session_id = schemas.StrSchema
+            session_reference_id = schemas.StrSchema
             parent_id = schemas.StrSchema
+            parent_reference_id = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
             class messages(
                 schemas.ListSchema
             ):
@@ -75,14 +76,15 @@
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
+            output = schemas.StrSchema
             source = schemas.StrSchema
             metadata = schemas.DictSchema
             
             
             class feedback(
                 schemas.ComposedSchema,
             ):
@@ -186,74 +188,85 @@
             user = schemas.StrSchema
             provider_response = schemas.DictSchema
             provider_latency = schemas.NumberSchema
             raw_output = schemas.StrSchema
             finish_reason = schemas.StrSchema
             __annotations__ = {
                 "project": project,
-                "output": output,
                 "config": config,
                 "id": id,
                 "project_id": project_id,
+                "reference_id": reference_id,
                 "session_id": session_id,
+                "session_reference_id": session_reference_id,
                 "parent_id": parent_id,
+                "parent_reference_id": parent_reference_id,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
+                "output": output,
                 "source": source,
                 "metadata": metadata,
                 "feedback": feedback,
                 "created_at": created_at,
                 "error": error,
                 "duration": duration,
                 "model_config": model_config,
                 "user": user,
                 "provider_response": provider_response,
                 "provider_latency": provider_latency,
                 "raw_output": raw_output,
                 "finish_reason": finish_reason,
             }
     
-    output: MetaOapg.properties.output
     project_id: MetaOapg.properties.project_id
     project: MetaOapg.properties.project
     id: MetaOapg.properties.id
     config: 'ConfigResponse'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["config"]) -> 'ConfigResponse': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["reference_id"]) -> MetaOapg.properties.reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["session_reference_id"]) -> MetaOapg.properties.session_reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parent_id"]) -> MetaOapg.properties.parent_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["parent_reference_id"]) -> MetaOapg.properties.parent_reference_id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["feedback"]) -> MetaOapg.properties.feedback: ...
@@ -284,50 +297,59 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["finish_reason"]) -> MetaOapg.properties.finish_reason: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "output", "config", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "config", "id", "project_id", "reference_id", "session_id", "session_reference_id", "parent_id", "parent_reference_id", "trial_id", "inputs", "messages", "output", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> 'ConfigResponse': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["reference_id"]) -> typing.Union[MetaOapg.properties.reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> typing.Union[MetaOapg.properties.session_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["session_reference_id"]) -> typing.Union[MetaOapg.properties.session_reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parent_id"]) -> typing.Union[MetaOapg.properties.parent_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["parent_reference_id"]) -> typing.Union[MetaOapg.properties.parent_reference_id, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["feedback"]) -> typing.Union[MetaOapg.properties.feedback, schemas.Unset]: ...
@@ -358,31 +380,34 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["finish_reason"]) -> typing.Union[MetaOapg.properties.finish_reason, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "output", "config", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "config", "id", "project_id", "reference_id", "session_id", "session_reference_id", "parent_id", "parent_reference_id", "trial_id", "inputs", "messages", "output", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        output: typing.Union[MetaOapg.properties.output, str, ],
         project_id: typing.Union[MetaOapg.properties.project_id, str, ],
         project: typing.Union[MetaOapg.properties.project, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         config: 'ConfigResponse',
+        reference_id: typing.Union[MetaOapg.properties.reference_id, str, schemas.Unset] = schemas.unset,
         session_id: typing.Union[MetaOapg.properties.session_id, str, schemas.Unset] = schemas.unset,
+        session_reference_id: typing.Union[MetaOapg.properties.session_reference_id, str, schemas.Unset] = schemas.unset,
         parent_id: typing.Union[MetaOapg.properties.parent_id, str, schemas.Unset] = schemas.unset,
+        parent_reference_id: typing.Union[MetaOapg.properties.parent_reference_id, str, schemas.Unset] = schemas.unset,
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
+        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         feedback: typing.Union[MetaOapg.properties.feedback, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
         error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
         duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -393,24 +418,27 @@
         finish_reason: typing.Union[MetaOapg.properties.finish_reason, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'LogResponse':
         return super().__new__(
             cls,
             *args,
-            output=output,
             project_id=project_id,
             project=project,
             id=id,
             config=config,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
+            output=output,
             source=source,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
             error=error,
             duration=duration,
             model_config=model_config,
```

### Comparing `humanloop-0.4.4/humanloop/model/logs_log_response.py` & `humanloop-0.4.5/humanloop/model/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/logs_log_response.pyi` & `humanloop-0.4.5/humanloop/model/logs_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_config_chat_request.py` & `humanloop-0.4.5/humanloop/model/model_config_chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_config_chat_request.pyi` & `humanloop-0.4.5/humanloop/model/model_config_chat_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_config_completion_request.py` & `humanloop-0.4.5/humanloop/model/model_config_completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_config_completion_request.pyi` & `humanloop-0.4.5/humanloop/model/model_config_completion_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_config_response.py` & `humanloop-0.4.5/humanloop/model/model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_config_response.pyi` & `humanloop-0.4.5/humanloop/model/model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_config_response2.py` & `humanloop-0.4.5/humanloop/model/model_config_response2.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_config_response2.pyi` & `humanloop-0.4.5/humanloop/model/model_config_response2.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_endpoints.py` & `humanloop-0.4.5/humanloop/model/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_endpoints.pyi` & `humanloop-0.4.5/humanloop/model/model_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/model_providers.py` & `humanloop-0.4.5/humanloop/model/model_providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     class MetaOapg:
         enum_value_to_name = {
             "openai": "OPENAI",
             "ai21": "AI21",
             "mock": "MOCK",
             "anthropic": "ANTHROPIC",
             "langchain": "LANGCHAIN",
+            "cohere": "COHERE",
         }
     
     @schemas.classproperty
     def OPENAI(cls):
         return cls("openai")
     
     @schemas.classproperty
@@ -58,7 +59,11 @@
     @schemas.classproperty
     def ANTHROPIC(cls):
         return cls("anthropic")
     
     @schemas.classproperty
     def LANGCHAIN(cls):
         return cls("langchain")
+    
+    @schemas.classproperty
+    def COHERE(cls):
+        return cls("cohere")
```

### Comparing `humanloop-0.4.4/humanloop/model/model_providers.pyi` & `humanloop-0.4.5/humanloop/model/model_providers.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -48,7 +48,11 @@
     @schemas.classproperty
     def ANTHROPIC(cls):
         return cls("anthropic")
     
     @schemas.classproperty
     def LANGCHAIN(cls):
         return cls("langchain")
+    
+    @schemas.classproperty
+    def COHERE(cls):
+        return cls("cohere")
```

### Comparing `humanloop-0.4.4/humanloop/model/paginated_data_log_response.py` & `humanloop-0.4.5/humanloop/model/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/paginated_data_log_response.pyi` & `humanloop-0.4.5/humanloop/model/paginated_data_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/paginated_data_project_response.py` & `humanloop-0.4.5/humanloop/model/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/paginated_data_project_response.pyi` & `humanloop-0.4.5/humanloop/model/paginated_data_project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/paginated_data_session_response.py` & `humanloop-0.4.5/humanloop/model/paginated_data_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/paginated_data_session_response.pyi` & `humanloop-0.4.5/humanloop/model/paginated_data_session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/positive_label.py` & `humanloop-0.4.5/humanloop/model/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/positive_label.pyi` & `humanloop-0.4.5/humanloop/model/positive_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_config_response.py` & `humanloop-0.4.5/humanloop/model/project_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_config_response.pyi` & `humanloop-0.4.5/humanloop/model/project_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_model_config_request.py` & `humanloop-0.4.5/humanloop/model/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_model_config_request.pyi` & `humanloop-0.4.5/humanloop/model/project_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_model_config_response.py` & `humanloop-0.4.5/humanloop/model/project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_model_config_response.pyi` & `humanloop-0.4.5/humanloop/model/project_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_response.py` & `humanloop-0.4.5/humanloop/model/project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_response.pyi` & `humanloop-0.4.5/humanloop/model/project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_sort_by.py` & `humanloop-0.4.5/humanloop/model/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_sort_by.pyi` & `humanloop-0.4.5/humanloop/model/project_sort_by.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_user_response.py` & `humanloop-0.4.5/humanloop/model/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/project_user_response.pyi` & `humanloop-0.4.5/humanloop/model/project_user_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/projects_get_configs_response.py` & `humanloop-0.4.5/humanloop/model/projects_get_configs_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/projects_get_configs_response.pyi` & `humanloop-0.4.5/humanloop/model/projects_get_configs_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/projects_update_feedback_types_request.py` & `humanloop-0.4.5/humanloop/model/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/projects_update_feedback_types_request.pyi` & `humanloop-0.4.5/humanloop/model/projects_update_feedback_types_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/provider_api_keys.py` & `humanloop-0.4.5/humanloop/model/provider_api_keys.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,19 +34,21 @@
     class MetaOapg:
         
         class properties:
             openai = schemas.StrSchema
             ai21 = schemas.StrSchema
             mock = schemas.StrSchema
             anthropic = schemas.StrSchema
+            cohere = schemas.StrSchema
             __annotations__ = {
                 "openai": openai,
                 "ai21": ai21,
                 "mock": mock,
                 "anthropic": anthropic,
+                "cohere": cohere,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["openai"]) -> MetaOapg.properties.openai: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ai21"]) -> MetaOapg.properties.ai21: ...
@@ -54,17 +56,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["mock"]) -> MetaOapg.properties.mock: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["anthropic"]) -> MetaOapg.properties.anthropic: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["cohere"]) -> MetaOapg.properties.cohere: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["openai", "ai21", "mock", "anthropic", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["openai", "ai21", "mock", "anthropic", "cohere", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["openai"]) -> typing.Union[MetaOapg.properties.openai, schemas.Unset]: ...
     
@@ -74,33 +79,38 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["mock"]) -> typing.Union[MetaOapg.properties.mock, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["anthropic"]) -> typing.Union[MetaOapg.properties.anthropic, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["cohere"]) -> typing.Union[MetaOapg.properties.cohere, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["openai", "ai21", "mock", "anthropic", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["openai", "ai21", "mock", "anthropic", "cohere", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         openai: typing.Union[MetaOapg.properties.openai, str, schemas.Unset] = schemas.unset,
         ai21: typing.Union[MetaOapg.properties.ai21, str, schemas.Unset] = schemas.unset,
         mock: typing.Union[MetaOapg.properties.mock, str, schemas.Unset] = schemas.unset,
         anthropic: typing.Union[MetaOapg.properties.anthropic, str, schemas.Unset] = schemas.unset,
+        cohere: typing.Union[MetaOapg.properties.cohere, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ProviderApiKeys':
         return super().__new__(
             cls,
             *args,
             openai=openai,
             ai21=ai21,
             mock=mock,
             anthropic=anthropic,
+            cohere=cohere,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `humanloop-0.4.4/humanloop/model/provider_api_keys.pyi` & `humanloop-0.4.5/humanloop/model/provider_api_keys.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -34,19 +34,21 @@
     class MetaOapg:
         
         class properties:
             openai = schemas.StrSchema
             ai21 = schemas.StrSchema
             mock = schemas.StrSchema
             anthropic = schemas.StrSchema
+            cohere = schemas.StrSchema
             __annotations__ = {
                 "openai": openai,
                 "ai21": ai21,
                 "mock": mock,
                 "anthropic": anthropic,
+                "cohere": cohere,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["openai"]) -> MetaOapg.properties.openai: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ai21"]) -> MetaOapg.properties.ai21: ...
@@ -54,17 +56,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["mock"]) -> MetaOapg.properties.mock: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["anthropic"]) -> MetaOapg.properties.anthropic: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["cohere"]) -> MetaOapg.properties.cohere: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["openai", "ai21", "mock", "anthropic", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["openai", "ai21", "mock", "anthropic", "cohere", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["openai"]) -> typing.Union[MetaOapg.properties.openai, schemas.Unset]: ...
     
@@ -74,33 +79,38 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["mock"]) -> typing.Union[MetaOapg.properties.mock, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["anthropic"]) -> typing.Union[MetaOapg.properties.anthropic, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["cohere"]) -> typing.Union[MetaOapg.properties.cohere, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["openai", "ai21", "mock", "anthropic", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["openai", "ai21", "mock", "anthropic", "cohere", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         openai: typing.Union[MetaOapg.properties.openai, str, schemas.Unset] = schemas.unset,
         ai21: typing.Union[MetaOapg.properties.ai21, str, schemas.Unset] = schemas.unset,
         mock: typing.Union[MetaOapg.properties.mock, str, schemas.Unset] = schemas.unset,
         anthropic: typing.Union[MetaOapg.properties.anthropic, str, schemas.Unset] = schemas.unset,
+        cohere: typing.Union[MetaOapg.properties.cohere, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ProviderApiKeys':
         return super().__new__(
             cls,
             *args,
             openai=openai,
             ai21=ai21,
             mock=mock,
             anthropic=anthropic,
+            cohere=cohere,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `humanloop-0.4.4/humanloop/model/session_project_response.py` & `humanloop-0.4.5/humanloop/model/session_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/session_project_response.pyi` & `humanloop-0.4.5/humanloop/model/session_project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/session_response.py` & `humanloop-0.4.5/humanloop/model/session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/session_response.pyi` & `humanloop-0.4.5/humanloop/model/session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/sort_order.py` & `humanloop-0.4.5/humanloop/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/sort_order.pyi` & `humanloop-0.4.5/humanloop/model/sort_order.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.5/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.5/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.5/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.5/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/tool_config_request.py` & `humanloop-0.4.5/humanloop/model/tool_config_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,18 @@
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "source",
             "type",
         }
         
         class properties:
-            source = schemas.StrSchema
             
             
             class type(
                 schemas.EnumBase,
                 schemas.StrSchema
             ):
             
@@ -53,77 +51,77 @@
                     }
                 
                 @schemas.classproperty
                 def TOOL(cls):
                     return cls("tool")
             description = schemas.StrSchema
             name = schemas.StrSchema
+            source = schemas.StrSchema
             other = schemas.DictSchema
             __annotations__ = {
-                "source": source,
                 "type": type,
                 "description": description,
                 "name": name,
+                "source": source,
                 "other": other,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
-    source: MetaOapg.properties.source
     type: MetaOapg.properties.type
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["source"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["other"], ]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["source"], typing_extensions.Literal["other"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["source"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["other"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["source"], typing_extensions.Literal["other"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        source: typing.Union[MetaOapg.properties.source, str, ],
         type: typing.Union[MetaOapg.properties.type, str, ],
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
+        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
     ) -> 'ToolConfigRequest':
         return super().__new__(
             cls,
             *args,
-            source=source,
             type=type,
             description=description,
             name=name,
+            source=source,
             other=other,
             _configuration=_configuration,
         )
```

### Comparing `humanloop-0.4.4/humanloop/model/tool_config_request.pyi` & `humanloop-0.4.5/humanloop/model/tool_config_request.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -29,95 +29,93 @@
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "source",
             "type",
         }
         
         class properties:
-            source = schemas.StrSchema
             
             
             class type(
                 schemas.EnumBase,
                 schemas.StrSchema
             ):
                 
                 @schemas.classproperty
                 def TOOL(cls):
                     return cls("tool")
             description = schemas.StrSchema
             name = schemas.StrSchema
+            source = schemas.StrSchema
             other = schemas.DictSchema
             __annotations__ = {
-                "source": source,
                 "type": type,
                 "description": description,
                 "name": name,
+                "source": source,
                 "other": other,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
-    source: MetaOapg.properties.source
     type: MetaOapg.properties.type
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["source"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["other"], ]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["source"], typing_extensions.Literal["other"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["source"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["other"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["source"], typing_extensions.Literal["other"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        source: typing.Union[MetaOapg.properties.source, str, ],
         type: typing.Union[MetaOapg.properties.type, str, ],
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
+        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
     ) -> 'ToolConfigRequest':
         return super().__new__(
             cls,
             *args,
-            source=source,
             type=type,
             description=description,
             name=name,
+            source=source,
             other=other,
             _configuration=_configuration,
         )
```

### Comparing `humanloop-0.4.4/humanloop/model/tool_config_response.py` & `humanloop-0.4.5/humanloop/model/tool_config_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     """
 
 
     class MetaOapg:
         required = {
             "name",
             "id",
-            "source",
             "type",
         }
         
         class properties:
             id = schemas.StrSchema
             
             
@@ -74,101 +73,100 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             name = schemas.StrSchema
-            source = schemas.StrSchema
             description = schemas.StrSchema
             other = schemas.DictSchema
+            source = schemas.StrSchema
             __annotations__ = {
                 "id": id,
                 "type": type,
                 "name": name,
-                "source": source,
                 "description": description,
                 "other": other,
+                "source": source,
             }
     
     name: MetaOapg.properties.name
     id: MetaOapg.properties.id
-    source: MetaOapg.properties.source
     type: MetaOapg.properties.type
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "source", "description", "other", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", "source", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "source", "description", "other", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", "source", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
-        source: typing.Union[MetaOapg.properties.source, str, ],
         type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ToolConfigResponse':
         return super().__new__(
             cls,
             *args,
             name=name,
             id=id,
-            source=source,
             type=type,
             description=description,
             other=other,
+            source=source,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.config_type import ConfigType
```

### Comparing `humanloop-0.4.4/humanloop/model/tool_config_response.pyi` & `humanloop-0.4.5/humanloop/model/tool_config_response.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     """
 
 
     class MetaOapg:
         required = {
             "name",
             "id",
-            "source",
             "type",
         }
         
         class properties:
             id = schemas.StrSchema
             
             
@@ -74,101 +73,100 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             name = schemas.StrSchema
-            source = schemas.StrSchema
             description = schemas.StrSchema
             other = schemas.DictSchema
+            source = schemas.StrSchema
             __annotations__ = {
                 "id": id,
                 "type": type,
                 "name": name,
-                "source": source,
                 "description": description,
                 "other": other,
+                "source": source,
             }
     
     name: MetaOapg.properties.name
     id: MetaOapg.properties.id
-    source: MetaOapg.properties.source
     type: MetaOapg.properties.type
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "source", "description", "other", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", "source", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "source", "description", "other", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", "source", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
-        source: typing.Union[MetaOapg.properties.source, str, ],
         type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ToolConfigResponse':
         return super().__new__(
             cls,
             *args,
             name=name,
             id=id,
-            source=source,
             type=type,
             description=description,
             other=other,
+            source=source,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.config_type import ConfigType
```

### Comparing `humanloop-0.4.4/humanloop/model/tool_result_response.py` & `humanloop-0.4.5/humanloop/model/tool_result_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/tool_result_response.pyi` & `humanloop-0.4.5/humanloop/model/tool_result_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/trace_log_request.py` & `humanloop-0.4.5/humanloop/model/trace_log_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,19 @@
 Changes:
     - Renamed `project` to `function_name`. TODO: Allow either `function_name` or `function_id`.
     """
 
 
     class MetaOapg:
         required = {
-            "output",
             "function_name",
         }
         
         class properties:
             function_name = schemas.StrSchema
-            output = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
             class messages(
                 schemas.ListSchema
             ):
@@ -69,14 +67,15 @@
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
+            output = schemas.StrSchema
             source = schemas.StrSchema
             
             
             class config(
                 schemas.ComposedSchema,
             ):
             
@@ -141,47 +140,46 @@
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'TraceLogRequest':
                     return super().__getitem__(i)
             __annotations__ = {
                 "function_name": function_name,
-                "output": output,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
+                "output": output,
                 "source": source,
                 "config": config,
                 "metadata": metadata,
                 "error": error,
                 "duration": duration,
                 "created_at": created_at,
                 "children": children,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
-    output: MetaOapg.properties.output
     function_name: MetaOapg.properties.function_name
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
@@ -194,34 +192,34 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["children"]) -> MetaOapg.properties.children: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["output"], typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
@@ -234,42 +232,42 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["children"]) -> typing.Union[MetaOapg.properties.children, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["output"], typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        output: typing.Union[MetaOapg.properties.output, str, ],
         function_name: typing.Union[MetaOapg.properties.function_name, str, ],
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
+        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
         duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
         children: typing.Union[MetaOapg.properties.children, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
     ) -> 'TraceLogRequest':
         return super().__new__(
             cls,
             *args,
-            output=output,
             function_name=function_name,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
+            output=output,
             source=source,
             config=config,
             metadata=metadata,
             error=error,
             duration=duration,
             created_at=created_at,
             children=children,
```

### Comparing `humanloop-0.4.4/humanloop/model/trace_log_request.pyi` & `humanloop-0.4.5/humanloop/model/trace_log_request.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,19 @@
 Changes:
     - Renamed `project` to `function_name`. TODO: Allow either `function_name` or `function_id`.
     """
 
 
     class MetaOapg:
         required = {
-            "output",
             "function_name",
         }
         
         class properties:
             function_name = schemas.StrSchema
-            output = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
             class messages(
                 schemas.ListSchema
             ):
@@ -69,14 +67,15 @@
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
+            output = schemas.StrSchema
             source = schemas.StrSchema
             
             
             class config(
                 schemas.ComposedSchema,
             ):
             
@@ -141,47 +140,46 @@
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'TraceLogRequest':
                     return super().__getitem__(i)
             __annotations__ = {
                 "function_name": function_name,
-                "output": output,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
+                "output": output,
                 "source": source,
                 "config": config,
                 "metadata": metadata,
                 "error": error,
                 "duration": duration,
                 "created_at": created_at,
                 "children": children,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
-    output: MetaOapg.properties.output
     function_name: MetaOapg.properties.function_name
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
@@ -194,34 +192,34 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["children"]) -> MetaOapg.properties.children: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["output"], typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
@@ -234,42 +232,42 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["children"]) -> typing.Union[MetaOapg.properties.children, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["output"], typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        output: typing.Union[MetaOapg.properties.output, str, ],
         function_name: typing.Union[MetaOapg.properties.function_name, str, ],
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
+        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
         duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
         children: typing.Union[MetaOapg.properties.children, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
     ) -> 'TraceLogRequest':
         return super().__new__(
             cls,
             *args,
-            output=output,
             function_name=function_name,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
+            output=output,
             source=source,
             config=config,
             metadata=metadata,
             error=error,
             duration=duration,
             created_at=created_at,
             children=children,
```

### Comparing `humanloop-0.4.4/humanloop/model/trace_model_config_request.py` & `humanloop-0.4.5/humanloop/model/trace_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/trace_model_config_request.pyi` & `humanloop-0.4.5/humanloop/model/trace_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/update_experiment_request.py` & `humanloop-0.4.5/humanloop/model/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/update_experiment_request.pyi` & `humanloop-0.4.5/humanloop/model/update_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/update_project_request.py` & `humanloop-0.4.5/humanloop/model/update_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/update_project_request.pyi` & `humanloop-0.4.5/humanloop/model/update_project_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/usage.py` & `humanloop-0.4.5/humanloop/model/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/usage.pyi` & `humanloop-0.4.5/humanloop/model/usage.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/validation_error.py` & `humanloop-0.4.5/humanloop/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/model/validation_error.pyi` & `humanloop-0.4.5/humanloop/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/models/__init__.py` & `humanloop-0.4.5/humanloop/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,10 +88,11 @@
 from humanloop.model.src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV4ProjectConfigsProjectModelConfigFeedbackStatsResponse
 from humanloop.model.tool_config_request import ToolConfigRequest
 from humanloop.model.tool_config_response import ToolConfigResponse
 from humanloop.model.tool_result_response import ToolResultResponse
 from humanloop.model.trace_log_request import TraceLogRequest
 from humanloop.model.trace_model_config_request import TraceModelConfigRequest
 from humanloop.model.update_experiment_request import UpdateExperimentRequest
+from humanloop.model.update_log_request import UpdateLogRequest
 from humanloop.model.update_project_request import UpdateProjectRequest
 from humanloop.model.usage import Usage
 from humanloop.model.validation_error import ValidationError
```

### Comparing `humanloop-0.4.4/humanloop/paths/__init__.py` & `humanloop-0.4.5/humanloop/paths/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     COMPLETIONEXPERIMENT = "/completion-experiment"
     COMPLETIONMODELCONFIG = "/completion-model-config"
     CHAT = "/chat"
     CHATDEPLOYED = "/chat-deployed"
     CHATEXPERIMENT = "/chat-experiment"
     CHATMODELCONFIG = "/chat-model-config"
     LOGS = "/logs"
+    LOGS_ID = "/logs/{id}"
     FEEDBACK = "/feedback"
     PROJECTS = "/projects"
     PROJECTS_ID = "/projects/{id}"
     PROJECTS_ID_CONFIGS = "/projects/{id}/configs"
     PROJECTS_ID_ACTIVECONFIG = "/projects/{id}/active-config"
     PROJECTS_ID_ACTIVEEXPERIMENT = "/projects/{id}/active-experiment"
     PROJECTS_ID_FEEDBACKTYPES = "/projects/{id}/feedback-types"
```

### Comparing `humanloop-0.4.4/humanloop/paths/chat/post.py` & `humanloop-0.4.5/humanloop/paths/chat/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/chat/post.pyi` & `humanloop-0.4.5/humanloop/paths/chat/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/chat_deployed/post.py` & `humanloop-0.4.5/humanloop/paths/chat_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/chat_deployed/post.pyi` & `humanloop-0.4.5/humanloop/paths/chat_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/chat_experiment/post.py` & `humanloop-0.4.5/humanloop/paths/chat_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/chat_experiment/post.pyi` & `humanloop-0.4.5/humanloop/paths/chat_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/chat_model_config/post.py` & `humanloop-0.4.5/humanloop/paths/chat_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/chat_model_config/post.pyi` & `humanloop-0.4.5/humanloop/paths/chat_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/completion/post.py` & `humanloop-0.4.5/humanloop/paths/completion/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/completion/post.pyi` & `humanloop-0.4.5/humanloop/paths/completion/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/completion_deployed/post.py` & `humanloop-0.4.5/humanloop/paths/completion_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/completion_deployed/post.pyi` & `humanloop-0.4.5/humanloop/paths/completion_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/completion_experiment/post.py` & `humanloop-0.4.5/humanloop/paths/completion_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/completion_experiment/post.pyi` & `humanloop-0.4.5/humanloop/paths/completion_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/completion_model_config/post.py` & `humanloop-0.4.5/humanloop/paths/completion_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/completion_model_config/post.pyi` & `humanloop-0.4.5/humanloop/paths/completion_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/experiments_experiment_id/delete.py` & `humanloop-0.4.5/humanloop/paths/experiments_experiment_id/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/experiments_experiment_id/delete.pyi` & `humanloop-0.4.5/humanloop/paths/experiments_experiment_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/experiments_experiment_id/patch.py` & `humanloop-0.4.5/humanloop/paths/experiments_experiment_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/experiments_experiment_id/patch.pyi` & `humanloop-0.4.5/humanloop/paths/experiments_experiment_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/get.py` & `humanloop-0.4.5/humanloop/paths/experiments_experiment_id_model_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/get.pyi` & `humanloop-0.4.5/humanloop/paths/experiments_experiment_id_model_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/feedback/post.py` & `humanloop-0.4.5/humanloop/paths/feedback/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/feedback/post.pyi` & `humanloop-0.4.5/humanloop/paths/feedback/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/logs/post.py` & `humanloop-0.4.5/humanloop/paths/logs/post.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -46,30 +46,25 @@
 from humanloop.type.generic_config_request import GenericConfigRequest
 from humanloop.type.tool_config_request import ToolConfigRequest
 from humanloop.type.logs_log_response import LogsLogResponse
 from humanloop.type.trace_model_config_request import TraceModelConfigRequest
 from humanloop.type.log_datapoint_request import LogDatapointRequest
 from humanloop.type.http_validation_error import HTTPValidationError
 
-from . import path
-
 # body param
 SchemaForRequestBodyApplicationJson = LogDatapointRequestSchema
 
 
 request_body_log_datapoint_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
 SchemaFor200ResponseBodyApplicationJson = LogsLogResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: LogsLogResponse
 
@@ -104,31 +99,30 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
     def _log_mapped_args(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -137,18 +131,24 @@
         error: typing.Optional[str] = None,
         duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if project is not None:
             _body["project"] = project
+        if reference_id is not None:
+            _body["reference_id"] = reference_id
         if session_id is not None:
             _body["session_id"] = session_id
+        if session_reference_id is not None:
+            _body["session_reference_id"] = session_reference_id
         if parent_id is not None:
             _body["parent_id"] = parent_id
+        if parent_reference_id is not None:
+            _body["parent_reference_id"] = parent_reference_id
         if trial_id is not None:
             _body["trial_id"] = trial_id
         if inputs is not None:
             _body["inputs"] = inputs
         if messages is not None:
             _body["messages"] = messages
         if output is not None:
@@ -338,16 +338,19 @@
 class Log(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def alog(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -359,16 +362,19 @@
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
@@ -381,16 +387,19 @@
             body=args.body,
         )
     
     def log(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -401,16 +410,19 @@
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
@@ -426,16 +438,19 @@
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -447,16 +462,19 @@
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
@@ -469,16 +487,19 @@
             body=args.body,
         )
     
     def post(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -489,16 +510,19 @@
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
```

### Comparing `humanloop-0.4.4/humanloop/paths/logs/post.pyi` & `humanloop-0.4.5/humanloop/paths/logs/post.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,25 +46,30 @@
 from humanloop.type.generic_config_request import GenericConfigRequest
 from humanloop.type.tool_config_request import ToolConfigRequest
 from humanloop.type.logs_log_response import LogsLogResponse
 from humanloop.type.trace_model_config_request import TraceModelConfigRequest
 from humanloop.type.log_datapoint_request import LogDatapointRequest
 from humanloop.type.http_validation_error import HTTPValidationError
 
+from . import path
+
 # body param
 SchemaForRequestBodyApplicationJson = LogDatapointRequestSchema
 
 
 request_body_log_datapoint_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
+_auth = [
+    'APIKeyHeader',
+]
 SchemaFor200ResponseBodyApplicationJson = LogsLogResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: LogsLogResponse
 
@@ -99,27 +104,34 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
     def _log_mapped_args(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -128,18 +140,24 @@
         error: typing.Optional[str] = None,
         duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if project is not None:
             _body["project"] = project
+        if reference_id is not None:
+            _body["reference_id"] = reference_id
         if session_id is not None:
             _body["session_id"] = session_id
+        if session_reference_id is not None:
+            _body["session_reference_id"] = session_reference_id
         if parent_id is not None:
             _body["parent_id"] = parent_id
+        if parent_reference_id is not None:
+            _body["parent_reference_id"] = parent_reference_id
         if trial_id is not None:
             _body["trial_id"] = trial_id
         if inputs is not None:
             _body["inputs"] = inputs
         if messages is not None:
             _body["messages"] = messages
         if output is not None:
@@ -329,16 +347,19 @@
 class Log(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def alog(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -350,16 +371,19 @@
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
@@ -372,16 +396,19 @@
             body=args.body,
         )
     
     def log(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -392,16 +419,19 @@
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
@@ -417,16 +447,19 @@
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -438,16 +471,19 @@
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
@@ -460,16 +496,19 @@
             body=args.body,
         )
     
     def post(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
+        reference_id: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
+        session_reference_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
+        parent_reference_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
         config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
@@ -480,16 +519,19 @@
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
+            reference_id=reference_id,
             session_id=session_id,
+            session_reference_id=session_reference_id,
             parent_id=parent_id,
+            parent_reference_id=parent_reference_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
             config=config,
             metadata=metadata,
```

### Comparing `humanloop-0.4.4/humanloop/paths/model_configs/post.py` & `humanloop-0.4.5/humanloop/paths/model_configs/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/model_configs/post.pyi` & `humanloop-0.4.5/humanloop/paths/model_configs/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/model_configs_id/get.py` & `humanloop-0.4.5/humanloop/paths/model_configs_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/model_configs_id/get.pyi` & `humanloop-0.4.5/humanloop/paths/model_configs_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects/get.py` & `humanloop-0.4.5/humanloop/paths/projects/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects/get.pyi` & `humanloop-0.4.5/humanloop/paths/projects/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects/post.py` & `humanloop-0.4.5/humanloop/paths/projects/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects/post.pyi` & `humanloop-0.4.5/humanloop/paths/projects/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id/get.py` & `humanloop-0.4.5/humanloop/paths/projects_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id/get.pyi` & `humanloop-0.4.5/humanloop/paths/projects_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id/patch.py` & `humanloop-0.4.5/humanloop/paths/projects_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id/patch.pyi` & `humanloop-0.4.5/humanloop/paths/projects_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_active_config/delete.py` & `humanloop-0.4.5/humanloop/paths/projects_id_active_config/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_active_config/delete.pyi` & `humanloop-0.4.5/humanloop/paths/projects_id_active_config/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_active_config/get.py` & `humanloop-0.4.5/humanloop/paths/projects_id_active_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_active_config/get.pyi` & `humanloop-0.4.5/humanloop/paths/projects_id_active_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/delete.py` & `humanloop-0.4.5/humanloop/paths/projects_id_active_experiment/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/delete.pyi` & `humanloop-0.4.5/humanloop/paths/projects_id_active_experiment/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_configs/get.py` & `humanloop-0.4.5/humanloop/paths/projects_id_configs/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_configs/get.pyi` & `humanloop-0.4.5/humanloop/paths/projects_id_configs/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_export/post.py` & `humanloop-0.4.5/humanloop/paths/projects_id_export/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_export/post.pyi` & `humanloop-0.4.5/humanloop/paths/projects_id_export/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/patch.py` & `humanloop-0.4.5/humanloop/paths/projects_id_feedback_types/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/patch.pyi` & `humanloop-0.4.5/humanloop/paths/projects_id_feedback_types/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/get.py` & `humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/get.pyi` & `humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/post.py` & `humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/post.pyi` & `humanloop-0.4.5/humanloop/paths/projects_project_id_experiments/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/sessions/get.py` & `humanloop-0.4.5/humanloop/paths/sessions/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/sessions/get.pyi` & `humanloop-0.4.5/humanloop/paths/sessions/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/sessions/post.py` & `humanloop-0.4.5/humanloop/paths/sessions/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/sessions/post.pyi` & `humanloop-0.4.5/humanloop/paths/sessions/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/sessions_id/get.py` & `humanloop-0.4.5/humanloop/paths/sessions_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/sessions_id/get.pyi` & `humanloop-0.4.5/humanloop/paths/sessions_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/traces/post.py` & `humanloop-0.4.5/humanloop/paths/traces/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/paths/traces/post.pyi` & `humanloop-0.4.5/humanloop/paths/traces/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/request_after_hook.py` & `humanloop-0.4.5/humanloop/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/request_before_hook.py` & `humanloop-0.4.5/humanloop/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/rest.py` & `humanloop-0.4.5/humanloop/rest.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/schemas.py` & `humanloop-0.4.5/humanloop/schemas.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/agent_config_request.py` & `humanloop-0.4.5/humanloop/type/agent_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/agent_config_response.py` & `humanloop-0.4.5/humanloop/type/agent_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/base_metric_response.py` & `humanloop-0.4.5/humanloop/type/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/categorical_feedback_label.py` & `humanloop-0.4.5/humanloop/type/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/chat_data_response.py` & `humanloop-0.4.5/humanloop/type/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/chat_deployed_request.py` & `humanloop-0.4.5/humanloop/type/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/chat_experiment_request.py` & `humanloop-0.4.5/humanloop/type/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/chat_message.py` & `humanloop-0.4.5/humanloop/type/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/chat_model_config_request.py` & `humanloop-0.4.5/humanloop/type/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/chat_request.py` & `humanloop-0.4.5/humanloop/type/chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/chat_response.py` & `humanloop-0.4.5/humanloop/type/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/chat_role.py` & `humanloop-0.4.5/humanloop/type/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/completion_deployed_request.py` & `humanloop-0.4.5/humanloop/type/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/completion_experiment_request.py` & `humanloop-0.4.5/humanloop/type/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/completion_model_config_request.py` & `humanloop-0.4.5/humanloop/type/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/completion_request.py` & `humanloop-0.4.5/humanloop/type/completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/completion_response.py` & `humanloop-0.4.5/humanloop/type/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/config_response.py` & `humanloop-0.4.5/humanloop/type/config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/config_type.py` & `humanloop-0.4.5/humanloop/type/config_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/create_experiment_request.py` & `humanloop-0.4.5/humanloop/type/create_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/create_log_response.py` & `humanloop-0.4.5/humanloop/type/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/create_project_request.py` & `humanloop-0.4.5/humanloop/type/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/create_session_response.py` & `humanloop-0.4.5/humanloop/type/create_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/create_trace_request.py` & `humanloop-0.4.5/humanloop/type/create_trace_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/create_trace_response.py` & `humanloop-0.4.5/humanloop/type/create_trace_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/data_response.py` & `humanloop-0.4.5/humanloop/type/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/experiment_config_response.py` & `humanloop-0.4.5/humanloop/type/experiment_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/experiment_response.py` & `humanloop-0.4.5/humanloop/type/experiment_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/experiment_status.py` & `humanloop-0.4.5/humanloop/type/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/experiments_list_response.py` & `humanloop-0.4.5/humanloop/type/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback.py` & `humanloop-0.4.5/humanloop/type/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_class.py` & `humanloop-0.4.5/humanloop/type/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_label_request.py` & `humanloop-0.4.5/humanloop/type/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_request.py` & `humanloop-0.4.5/humanloop/type/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_response.py` & `humanloop-0.4.5/humanloop/type/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_submit_request.py` & `humanloop-0.4.5/humanloop/type/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_submit_response.py` & `humanloop-0.4.5/humanloop/type/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_type.py` & `humanloop-0.4.5/humanloop/type/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_type_model.py` & `humanloop-0.4.5/humanloop/type/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_type_request.py` & `humanloop-0.4.5/humanloop/type/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/feedback_types.py` & `humanloop-0.4.5/humanloop/type/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/generic_config_request.py` & `humanloop-0.4.5/humanloop/type/generic_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/generic_config_response.py` & `humanloop-0.4.5/humanloop/type/generic_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/get_model_config_response.py` & `humanloop-0.4.5/humanloop/type/get_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/http_validation_error.py` & `humanloop-0.4.5/humanloop/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/label_sentiment.py` & `humanloop-0.4.5/humanloop/type/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/log_datapoint_request.py` & `humanloop-0.4.5/humanloop/type/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/log_model_config_request.py` & `humanloop-0.4.5/humanloop/type/log_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/log_request.py` & `humanloop-0.4.5/humanloop/type/trace_log_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,58 +12,51 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.agent_config_request import AgentConfigRequest
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.feedback import Feedback
 from humanloop.type.generic_config_request import GenericConfigRequest
 from humanloop.type.tool_config_request import ToolConfigRequest
 from humanloop.type.trace_model_config_request import TraceModelConfigRequest
 
-class RequiredLogRequest(TypedDict):
-    # Generated output from your model for the provided inputs.
-    output: str
-
-class OptionalLogRequest(TypedDict, total=False):
+class RequiredTraceLogRequest(TypedDict):
     # Unique function name. If no function exists with this name, a new function will be created.
-    project: str
-
-    # ID of the session to associate the datapoint.
-    session_id: str
-
-    # ID associated to the parent datapoint in a session.
-    parent_id: str
+    function_name: str
 
+class OptionalTraceLogRequest(TypedDict, total=False):
     # Unique ID of an experiment trial to associate to the log.
     trial_id: str
 
     # The inputs passed to the prompt template.
     inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # The messages passed to the to provider chat endpoint.
     messages: typing.List[ChatMessage]
 
+    # Generated output from your model for the provided inputs. Can be `None` if logging an error.
+    output: str
+
     # Identifies where the model was called from.
     source: str
 
-    # The model config used for this generation. Required unless `trial_id` is provided.
+    # The config used for this generation. Required unless `trial_id` is provided.
     config: typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]
 
     # Any additional metadata to record.
     metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-    # Optional parameter to provide feedback with your logged datapoint.
-    feedback: typing.Union[Feedback, typing.List[Feedback]]
-
-    # User defined timestamp for when the log was created. 
-    created_at: datetime
-
     # Error message if the log is an error.
     error: str
 
     # Duration of the logged event in seconds.
     duration: typing.Union[int, float]
 
-class LogRequest(RequiredLogRequest, OptionalLogRequest):
+    # User-defined timestamp for when the log was created.
+    created_at: datetime
+
+    # List of children logs.
+    children: typing.List["TraceLogRequest"]
+
+class TraceLogRequest(RequiredTraceLogRequest, OptionalTraceLogRequest):
     pass
```

### Comparing `humanloop-0.4.4/humanloop/type/log_response.py` & `humanloop-0.4.5/humanloop/type/log_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,41 +19,50 @@
 from humanloop.type.feedback import Feedback
 from humanloop.type.project_config_response import ProjectConfigResponse
 
 class RequiredLogResponse(TypedDict):
     # Function name. If it does not exist, a new function will be created.
     project: str
 
-    # Generated output from your model for the provided inputs.
-    output: str
-
     config: ConfigResponse
 
     # String ID of logged datapoint. Starts with `data_`.
     id: str
 
     # String ID of project the datapoint belongs to. Starts with `pr_`.
     project_id: str
 
 class OptionalLogResponse(TypedDict, total=False):
+    # A unique string to reference the datapoint. Allows you to log nested datapoints with your internal system IDs by passing the same reference ID as `parent_id` in a subsequent log request.
+    reference_id: str
+
     # Session ID.
     session_id: str
 
+    # A unique string identifying the session to associate the datapoint to. Allows you to log multiple datapoints to a session (using an ID kept by your internal systems) by passing the same `session_reference_id` in subsequent log requests. Specify at most one of this or `session_id`.
+    session_reference_id: str
+
     # Id associated to the parent datapoint. Useful when providing a trace from a chain.
     parent_id: str
 
+    # A unique string identifying the previously-logged parent datapoint in a session. Allows you to log nested datapoints with your internal system IDs by passing the same reference ID as `parent_id` in a prior log request. Specify at most one of this or `parent_id`. Note that this cannot refer to a datapoint being logged in the same request.
+    parent_reference_id: str
+
     # Unique ID of an experiment trial to associate to the log.
     trial_id: str
 
     # The inputs passed to the prompt template.
     inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # The messages passed to the to provider chat endpoint.
     messages: typing.List[ChatMessage]
 
+    # Generated output from your model for the provided inputs.
+    output: str
+
     # Identifies where the model was called from.
     source: str
 
     # Additional metadata logged for reference.
     metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # Feedback associated to the datapoint.
```

### Comparing `humanloop-0.4.4/humanloop/type/logs_log_response.py` & `humanloop-0.4.5/humanloop/type/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/model_config_chat_request.py` & `humanloop-0.4.5/humanloop/type/model_config_chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/model_config_completion_request.py` & `humanloop-0.4.5/humanloop/type/model_config_completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/model_config_response.py` & `humanloop-0.4.5/humanloop/type/model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/model_config_response2.py` & `humanloop-0.4.5/humanloop/type/model_config_response2.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/model_endpoints.py` & `humanloop-0.4.5/humanloop/type/projects_get_configs_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from humanloop.type.project_config_response import ProjectConfigResponse
 
-ModelEndpoints = Literal["complete", "chat", "edit"]
+ProjectsGetConfigsResponse = typing.List[ProjectConfigResponse]
```

### Comparing `humanloop-0.4.4/humanloop/type/model_providers.py` & `humanloop-0.4.5/humanloop/type/model_providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 
-ModelProviders = Literal["openai", "ai21", "mock", "anthropic", "langchain"]
+ModelProviders = Literal["openai", "ai21", "mock", "anthropic", "langchain", "cohere"]
```

### Comparing `humanloop-0.4.4/humanloop/type/paginated_data_log_response.py` & `humanloop-0.4.5/humanloop/type/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/paginated_data_project_response.py` & `humanloop-0.4.5/humanloop/type/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/paginated_data_session_response.py` & `humanloop-0.4.5/humanloop/type/paginated_data_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/positive_label.py` & `humanloop-0.4.5/humanloop/type/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/project_config_response.py` & `humanloop-0.4.5/humanloop/type/project_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/project_model_config_request.py` & `humanloop-0.4.5/humanloop/type/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/project_model_config_response.py` & `humanloop-0.4.5/humanloop/type/project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/project_response.py` & `humanloop-0.4.5/humanloop/type/project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/project_sort_by.py` & `humanloop-0.4.5/humanloop/type/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/project_user_response.py` & `humanloop-0.4.5/humanloop/type/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/projects_get_configs_response.py` & `humanloop-0.4.5/humanloop/type/tool_result_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,10 +10,22 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.project_config_response import ProjectConfigResponse
 
-ProjectsGetConfigsResponse = typing.List[ProjectConfigResponse]
+class RequiredToolResultResponse(TypedDict):
+    id: str
+
+    name: str
+
+    signature: str
+
+    result: str
+
+class OptionalToolResultResponse(TypedDict, total=False):
+    pass
+
+class ToolResultResponse(RequiredToolResultResponse, OptionalToolResultResponse):
+    pass
```

### Comparing `humanloop-0.4.4/humanloop/type/projects_update_feedback_types_request.py` & `humanloop-0.4.5/humanloop/type/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/provider_api_keys.py` & `humanloop-0.4.5/humanloop/type/provider_api_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,9 +23,11 @@
 
     ai21: str
 
     mock: str
 
     anthropic: str
 
+    cohere: str
+
 class ProviderApiKeys(RequiredProviderApiKeys, OptionalProviderApiKeys):
     pass
```

### Comparing `humanloop-0.4.4/humanloop/type/session_project_response.py` & `humanloop-0.4.5/humanloop/type/session_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/session_response.py` & `humanloop-0.4.5/humanloop/type/session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/sort_order.py` & `humanloop-0.4.5/humanloop/type/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.5/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.5/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/tool_config_request.py` & `humanloop-0.4.5/humanloop/type/tool_config_request.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 
 class RequiredToolConfigRequest(TypedDict):
-    source: str
-
     type: str
 
 class OptionalToolConfigRequest(TypedDict, total=False):
     description: str
 
     name: str
 
+    source: str
+
     # Other parameters that define the config.
     other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
 class ToolConfigRequest(RequiredToolConfigRequest, OptionalToolConfigRequest):
     pass
```

### Comparing `humanloop-0.4.4/humanloop/type/tool_config_response.py` & `humanloop-0.4.5/humanloop/type/tool_config_response.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
     # Type of config.
     type: ConfigType
 
     # Name of config.
     name: str
 
-    # Code source of the tool.
-    source: str
-
 class OptionalToolConfigResponse(TypedDict, total=False):
     # Description of config.
     description: str
 
     # Other parameters that define the config.
     other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
+    # Code source of the tool.
+    source: str
+
 class ToolConfigResponse(RequiredToolConfigResponse, OptionalToolConfigResponse):
     pass
```

### Comparing `humanloop-0.4.4/humanloop/type/trace_log_request.py` & `humanloop-0.4.5/humanloop/type/trace_model_config_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,53 +10,57 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.agent_config_request import AgentConfigRequest
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.generic_config_request import GenericConfigRequest
-from humanloop.type.tool_config_request import ToolConfigRequest
-from humanloop.type.trace_model_config_request import TraceModelConfigRequest
+from humanloop.type.model_endpoints import ModelEndpoints
+from humanloop.type.model_providers import ModelProviders
 
-class RequiredTraceLogRequest(TypedDict):
-    # Unique function name. If no function exists with this name, a new function will be created.
-    function_name: str
+class RequiredTraceModelConfigRequest(TypedDict):
+    # The model instance used. E.g. text-davinci-002.
+    model: str
 
-    # Generated output from your model for the provided inputs.
-    output: str
+    type: str
 
-class OptionalTraceLogRequest(TypedDict, total=False):
-    # Unique ID of an experiment trial to associate to the log.
-    trial_id: str
+class OptionalTraceModelConfigRequest(TypedDict, total=False):
+    description: str
 
-    # The inputs passed to the prompt template.
-    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    name: str
 
-    # The messages passed to the to provider chat endpoint.
-    messages: typing.List[ChatMessage]
+    # The company providing the underlying model service.
+    provider: ModelProviders
 
-    # Identifies where the model was called from.
-    source: str
+    # The maximum number of tokens to generate. Provide max_tokens=-1 to dynamically calculate the maximum number of tokens to generate given the length of the prompt
+    max_tokens: int
 
-    # The model config used for this generation. Required unless `trial_id` is provided.
-    config: typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]
+    # What sampling temperature to use when making a generation. Higher values means the model will be more creative.
+    temperature: typing.Union[int, float]
 
-    # Any additional metadata to record.
-    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    # An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
+    top_p: typing.Union[int, float]
 
-    # Error message if the log is an error.
-    error: str
+    # The string (or list of strings) after which the model will stop generating. The returned text will not contain the stop sequence.
+    stop: typing.Union[str, typing.List[str]]
 
-    # Duration of the logged event in seconds.
-    duration: typing.Union[int, float]
+    # Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the generation so far.
+    presence_penalty: typing.Union[int, float]
 
-    # User-defined timestamp for when the log was created.
-    created_at: datetime
+    # Number between -2.0 and 2.0. Positive values penalize new tokens based on how frequently they appear in the generation so far.
+    frequency_penalty: typing.Union[int, float]
 
-    # List of children logs.
-    children: typing.List["TraceLogRequest"]
+    # Other parameter values to be passed to the provider call.
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-class TraceLogRequest(RequiredTraceLogRequest, OptionalTraceLogRequest):
+    # The provider model endpoint used.
+    endpoint: ModelEndpoints
+
+    # Prompt template that will take your specified inputs to form your final request to the model. Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
+    prompt_template: str
+
+    # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. Input variables within the template should be specified with syntax: {{INPUT_NAME}}.
+    chat_template: typing.List[ChatMessage]
+
+class TraceModelConfigRequest(RequiredTraceModelConfigRequest, OptionalTraceModelConfigRequest):
     pass
```

### Comparing `humanloop-0.4.4/humanloop/type/update_experiment_request.py` & `humanloop-0.4.5/humanloop/type/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/update_project_request.py` & `humanloop-0.4.5/humanloop/type/update_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/usage.py` & `humanloop-0.4.5/humanloop/type/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type/validation_error.py` & `humanloop-0.4.5/humanloop/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/type_util.py` & `humanloop-0.4.5/humanloop/type_util.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/humanloop/validation_metadata.py` & `humanloop-0.4.5/humanloop/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.4/pyproject.toml` & `humanloop-0.4.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "humanloop"
-version = "0.4.4"
+version = "0.4.5"
 description = "Client for Humanloop API"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "humanloop"}]
 
 [tool.poetry.dependencies]
```

### Comparing `humanloop-0.4.4/PKG-INFO` & `humanloop-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanloop
-Version: 0.4.4
+Version: 0.4.5
 Summary: Client for Humanloop API
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,25 +18,25 @@
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
-# humanloop@0.4.4
+# humanloop@0.4.5
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.4
+pip install humanloop==0.4.5
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
```


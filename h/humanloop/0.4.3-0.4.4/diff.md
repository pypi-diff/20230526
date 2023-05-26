# Comparing `tmp/humanloop-0.4.3.tar.gz` & `tmp/humanloop-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanloop-0.4.3.tar", max compression
+gzip compressed data, was "humanloop-0.4.4.tar", max compression
```

## Comparing `humanloop-0.4.3.tar` & `humanloop-0.4.4.tar`

### file list

```diff
@@ -1,401 +1,401 @@
--rw-r--r--   0        0        0     1081 2023-05-24 22:06:03.788313 humanloop-0.4.3/LICENSE
--rw-r--r--   0        0        0     8475 2023-05-24 22:06:03.847069 humanloop-0.4.3/README.md
--rw-r--r--   0        0        0     1059 2023-05-24 22:06:03.698102 humanloop-0.4.3/humanloop/__init__.py
--rw-r--r--   0        0        0    73009 2023-05-24 22:06:03.698441 humanloop-0.4.3/humanloop/api_client.py
--rw-r--r--   0        0        0      663 2023-05-24 22:06:03.698616 humanloop-0.4.3/humanloop/api_response.py
--rw-r--r--   0        0        0      214 2023-05-24 22:06:03.698783 humanloop-0.4.3/humanloop/apis/__init__.py
--rw-r--r--   0        0        0     4578 2023-05-24 22:06:03.698925 humanloop-0.4.3/humanloop/apis/path_to_api.py
--rw-r--r--   0        0        0      236 2023-05-24 22:06:03.699095 humanloop-0.4.3/humanloop/apis/paths/__init__.py
--rw-r--r--   0        0        0       91 2023-05-24 22:06:03.699244 humanloop-0.4.3/humanloop/apis/paths/chat.py
--rw-r--r--   0        0        0      108 2023-05-24 22:06:03.699392 humanloop-0.4.3/humanloop/apis/paths/chat_deployed.py
--rw-r--r--   0        0        0      112 2023-05-24 22:06:03.699552 humanloop-0.4.3/humanloop/apis/paths/chat_experiment.py
--rw-r--r--   0        0        0      115 2023-05-24 22:06:03.699709 humanloop-0.4.3/humanloop/apis/paths/chat_model_config.py
--rw-r--r--   0        0        0      103 2023-05-24 22:06:03.699869 humanloop-0.4.3/humanloop/apis/paths/completion.py
--rw-r--r--   0        0        0      120 2023-05-24 22:06:03.700519 humanloop-0.4.3/humanloop/apis/paths/completion_deployed.py
--rw-r--r--   0        0        0      124 2023-05-24 22:06:03.700621 humanloop-0.4.3/humanloop/apis/paths/completion_experiment.py
--rw-r--r--   0        0        0      127 2023-05-24 22:06:03.700710 humanloop-0.4.3/humanloop/apis/paths/completion_model_config.py
--rw-r--r--   0        0        0      226 2023-05-24 22:06:03.700822 humanloop-0.4.3/humanloop/apis/paths/experiments_experiment_id.py
--rw-r--r--   0        0        0      152 2023-05-24 22:06:03.700965 humanloop-0.4.3/humanloop/apis/paths/experiments_experiment_id_model_config.py
--rw-r--r--   0        0        0       99 2023-05-24 22:06:03.701106 humanloop-0.4.3/humanloop/apis/paths/feedback.py
--rw-r--r--   0        0        0       91 2023-05-24 22:06:03.701240 humanloop-0.4.3/humanloop/apis/paths/logs.py
--rw-r--r--   0        0        0      108 2023-05-24 22:06:03.701367 humanloop-0.4.3/humanloop/apis/paths/model_configs.py
--rw-r--r--   0        0        0      110 2023-05-24 22:06:03.701456 humanloop-0.4.3/humanloop/apis/paths/model_configs_id.py
--rw-r--r--   0        0        0      165 2023-05-24 22:06:03.701592 humanloop-0.4.3/humanloop/apis/paths/projects.py
--rw-r--r--   0        0        0      176 2023-05-24 22:06:03.701725 humanloop-0.4.3/humanloop/apis/paths/projects_id.py
--rw-r--r--   0        0        0      219 2023-05-24 22:06:03.701864 humanloop-0.4.3/humanloop/apis/paths/projects_id_active_config.py
--rw-r--r--   0        0        0      144 2023-05-24 22:06:03.702005 humanloop-0.4.3/humanloop/apis/paths/projects_id_active_experiment.py
--rw-r--r--   0        0        0      116 2023-05-24 22:06:03.702133 humanloop-0.4.3/humanloop/apis/paths/projects_id_configs.py
--rw-r--r--   0        0        0      117 2023-05-24 22:06:03.702273 humanloop-0.4.3/humanloop/apis/paths/projects_id_export.py
--rw-r--r--   0        0        0      135 2023-05-24 22:06:03.702432 humanloop-0.4.3/humanloop/apis/paths/projects_id_feedback_types.py
--rw-r--r--   0        0        0      231 2023-05-24 22:06:03.702973 humanloop-0.4.3/humanloop/apis/paths/projects_project_id_experiments.py
--rw-r--r--   0        0        0      165 2023-05-24 22:06:03.703230 humanloop-0.4.3/humanloop/apis/paths/sessions.py
--rw-r--r--   0        0        0      101 2023-05-24 22:06:03.703487 humanloop-0.4.3/humanloop/apis/paths/sessions_id.py
--rw-r--r--   0        0        0       95 2023-05-24 22:06:03.703696 humanloop-0.4.3/humanloop/apis/paths/traces.py
--rw-r--r--   0        0        0     1654 2023-05-24 22:06:03.703840 humanloop-0.4.3/humanloop/apis/tag_to_api.py
--rw-r--r--   0        0        0      572 2023-05-24 22:06:03.703959 humanloop-0.4.3/humanloop/apis/tags/__init__.py
--rw-r--r--   0        0        0     1006 2023-05-24 22:06:03.704067 humanloop-0.4.3/humanloop/apis/tags/chats_api.py
--rw-r--r--   0        0        0     1020 2023-05-24 22:06:03.704208 humanloop-0.4.3/humanloop/apis/tags/completions_api.py
--rw-r--r--   0        0        0     1091 2023-05-24 22:06:03.704352 humanloop-0.4.3/humanloop/apis/tags/experiments_api.py
--rw-r--r--   0        0        0      721 2023-05-24 22:06:03.704504 humanloop-0.4.3/humanloop/apis/tags/feedback_api.py
--rw-r--r--   0        0        0      707 2023-05-24 22:06:03.704671 humanloop-0.4.3/humanloop/apis/tags/logs_api.py
--rw-r--r--   0        0        0      803 2023-05-24 22:06:03.704948 humanloop-0.4.3/humanloop/apis/tags/model_configurations_api.py
--rw-r--r--   0        0        0     1486 2023-05-24 22:06:03.705091 humanloop-0.4.3/humanloop/apis/tags/projects_api.py
--rw-r--r--   0        0        0      834 2023-05-24 22:06:03.705260 humanloop-0.4.3/humanloop/apis/tags/sessions_api.py
--rw-r--r--   0        0        0      717 2023-05-24 22:06:03.705450 humanloop-0.4.3/humanloop/apis/tags/traces_api.py
--rw-r--r--   0        0        0    28032 2023-05-24 22:06:03.705692 humanloop-0.4.3/humanloop/client.py
--rw-r--r--   0        0        0    28032 2023-05-24 22:06:03.706024 humanloop-0.4.3/humanloop/client.pyi
--rw-r--r--   0        0        0     7186 2023-05-18 09:14:14.289106 humanloop-0.4.3/humanloop/client_custom.py
--rw-r--r--   0        0        0    18674 2023-05-24 22:06:03.706348 humanloop-0.4.3/humanloop/configuration.py
--rw-r--r--   0        0        0     7678 2023-05-24 22:06:03.706602 humanloop-0.4.3/humanloop/exceptions.py
--rw-r--r--   0        0        0     2274 2023-05-24 22:06:03.706771 humanloop-0.4.3/humanloop/exceptions_base.py
--rw-r--r--   0        0        0      343 2023-05-24 22:06:03.707079 humanloop-0.4.3/humanloop/model/__init__.py
--rw-r--r--   0        0        0     9140 2023-05-24 22:06:03.707324 humanloop-0.4.3/humanloop/model/agent_config_request.py
--rw-r--r--   0        0        0     8975 2023-05-24 22:06:03.707953 humanloop-0.4.3/humanloop/model/agent_config_request.pyi
--rw-r--r--   0        0        0    11140 2023-05-24 22:06:03.712785 humanloop-0.4.3/humanloop/model/agent_config_response.py
--rw-r--r--   0        0        0    11140 2023-05-24 22:06:03.713182 humanloop-0.4.3/humanloop/model/agent_config_response.pyi
--rw-r--r--   0        0        0     6379 2023-05-24 22:06:03.713516 humanloop-0.4.3/humanloop/model/base_metric_response.py
--rw-r--r--   0        0        0     6379 2023-05-24 22:06:03.713738 humanloop-0.4.3/humanloop/model/base_metric_response.pyi
--rw-r--r--   0        0        0     5150 2023-05-24 22:06:03.713962 humanloop-0.4.3/humanloop/model/categorical_feedback_label.py
--rw-r--r--   0        0        0     5150 2023-05-24 22:06:03.714167 humanloop-0.4.3/humanloop/model/categorical_feedback_label.pyi
--rw-r--r--   0        0        0     8957 2023-05-24 22:06:03.714373 humanloop-0.4.3/humanloop/model/chat_data_response.py
--rw-r--r--   0        0        0     8957 2023-05-24 22:06:03.714596 humanloop-0.4.3/humanloop/model/chat_data_response.pyi
--rw-r--r--   0        0        0     9998 2023-05-24 22:06:03.714836 humanloop-0.4.3/humanloop/model/chat_deployed_request.py
--rw-r--r--   0        0        0     9998 2023-05-24 22:06:03.715159 humanloop-0.4.3/humanloop/model/chat_deployed_request.pyi
--rw-r--r--   0        0        0    10659 2023-05-24 22:06:03.715423 humanloop-0.4.3/humanloop/model/chat_experiment_request.py
--rw-r--r--   0        0        0    10659 2023-05-24 22:06:03.715671 humanloop-0.4.3/humanloop/model/chat_experiment_request.pyi
--rw-r--r--   0        0        0     3702 2023-05-24 22:06:03.715885 humanloop-0.4.3/humanloop/model/chat_message.py
--rw-r--r--   0        0        0     3702 2023-05-24 22:06:03.716094 humanloop-0.4.3/humanloop/model/chat_message.pyi
--rw-r--r--   0        0        0    10693 2023-05-24 22:06:03.716302 humanloop-0.4.3/humanloop/model/chat_model_config_request.py
--rw-r--r--   0        0        0    10693 2023-05-24 22:06:03.716560 humanloop-0.4.3/humanloop/model/chat_model_config_request.pyi
--rw-r--r--   0        0        0    12556 2023-05-24 22:06:03.716796 humanloop-0.4.3/humanloop/model/chat_request.py
--rw-r--r--   0        0        0    12556 2023-05-24 22:06:03.717010 humanloop-0.4.3/humanloop/model/chat_request.pyi
--rw-r--r--   0        0        0    11076 2023-05-24 22:06:03.717221 humanloop-0.4.3/humanloop/model/chat_response.py
--rw-r--r--   0        0        0    11076 2023-05-24 22:06:03.717435 humanloop-0.4.3/humanloop/model/chat_response.pyi
--rw-r--r--   0        0        0     1446 2023-05-24 22:06:03.717633 humanloop-0.4.3/humanloop/model/chat_role.py
--rw-r--r--   0        0        0     1285 2023-05-24 22:06:03.717800 humanloop-0.4.3/humanloop/model/chat_role.pyi
--rw-r--r--   0        0        0     9674 2023-05-24 22:06:03.717994 humanloop-0.4.3/humanloop/model/completion_deployed_request.py
--rw-r--r--   0        0        0     9674 2023-05-24 22:06:03.718221 humanloop-0.4.3/humanloop/model/completion_deployed_request.pyi
--rw-r--r--   0        0        0    10340 2023-05-24 22:06:03.718476 humanloop-0.4.3/humanloop/model/completion_experiment_request.py
--rw-r--r--   0        0        0    10340 2023-05-24 22:06:03.718727 humanloop-0.4.3/humanloop/model/completion_experiment_request.pyi
--rw-r--r--   0        0        0    10376 2023-05-24 22:06:03.718968 humanloop-0.4.3/humanloop/model/completion_model_config_request.py
--rw-r--r--   0        0        0    10376 2023-05-24 22:06:03.719186 humanloop-0.4.3/humanloop/model/completion_model_config_request.pyi
--rw-r--r--   0        0        0    12258 2023-05-24 22:06:03.719396 humanloop-0.4.3/humanloop/model/completion_request.py
--rw-r--r--   0        0        0    12258 2023-05-24 22:06:03.719624 humanloop-0.4.3/humanloop/model/completion_request.pyi
--rw-r--r--   0        0        0    11017 2023-05-24 22:06:03.719855 humanloop-0.4.3/humanloop/model/completion_response.py
--rw-r--r--   0        0        0    11017 2023-05-24 22:06:03.720071 humanloop-0.4.3/humanloop/model/completion_response.pyi
--rw-r--r--   0        0        0     2672 2023-05-24 22:06:03.720251 humanloop-0.4.3/humanloop/model/config_response.py
--rw-r--r--   0        0        0     2672 2023-05-24 22:06:03.720399 humanloop-0.4.3/humanloop/model/config_response.pyi
--rw-r--r--   0        0        0     1546 2023-05-24 22:06:03.720543 humanloop-0.4.3/humanloop/model/config_type.py
--rw-r--r--   0        0        0     1361 2023-05-24 22:06:03.720704 humanloop-0.4.3/humanloop/model/config_type.pyi
--rw-r--r--   0        0        0     6196 2023-05-24 22:06:03.720853 humanloop-0.4.3/humanloop/model/create_experiment_request.py
--rw-r--r--   0        0        0     6196 2023-05-24 22:06:03.720990 humanloop-0.4.3/humanloop/model/create_experiment_request.pyi
--rw-r--r--   0        0        0     3199 2023-05-24 22:06:03.721141 humanloop-0.4.3/humanloop/model/create_log_response.py
--rw-r--r--   0        0        0     3199 2023-05-24 22:06:03.721287 humanloop-0.4.3/humanloop/model/create_log_response.pyi
--rw-r--r--   0        0        0     4266 2023-05-24 22:06:03.721447 humanloop-0.4.3/humanloop/model/create_project_request.py
--rw-r--r--   0        0        0     4266 2023-05-24 22:06:03.721584 humanloop-0.4.3/humanloop/model/create_project_request.pyi
--rw-r--r--   0        0        0     2635 2023-05-24 22:06:03.721725 humanloop-0.4.3/humanloop/model/create_session_response.py
--rw-r--r--   0        0        0     2635 2023-05-24 22:06:03.721847 humanloop-0.4.3/humanloop/model/create_session_response.pyi
--rw-r--r--   0        0        0     3232 2023-05-24 22:06:03.722010 humanloop-0.4.3/humanloop/model/create_trace_request.py
--rw-r--r--   0        0        0     3232 2023-05-24 22:06:03.722170 humanloop-0.4.3/humanloop/model/create_trace_request.pyi
--rw-r--r--   0        0        0     3329 2023-05-24 22:06:03.722305 humanloop-0.4.3/humanloop/model/create_trace_response.py
--rw-r--r--   0        0        0     3329 2023-05-24 22:06:03.722448 humanloop-0.4.3/humanloop/model/create_trace_response.pyi
--rw-r--r--   0        0        0     7455 2023-05-24 22:06:03.722611 humanloop-0.4.3/humanloop/model/data_response.py
--rw-r--r--   0        0        0     7455 2023-05-24 22:06:03.722795 humanloop-0.4.3/humanloop/model/data_response.pyi
--rw-r--r--   0        0        0     8998 2023-05-24 22:06:03.722964 humanloop-0.4.3/humanloop/model/experiment_config_response.py
--rw-r--r--   0        0        0     8998 2023-05-24 22:06:03.723181 humanloop-0.4.3/humanloop/model/experiment_config_response.pyi
--rw-r--r--   0        0        0    12827 2023-05-24 22:06:03.723386 humanloop-0.4.3/humanloop/model/experiment_response.py
--rw-r--r--   0        0        0    12827 2023-05-24 22:06:03.723646 humanloop-0.4.3/humanloop/model/experiment_response.pyi
--rw-r--r--   0        0        0     1376 2023-05-24 22:06:03.723851 humanloop-0.4.3/humanloop/model/experiment_status.py
--rw-r--r--   0        0        0     1229 2023-05-24 22:06:03.724015 humanloop-0.4.3/humanloop/model/experiment_status.pyi
--rw-r--r--   0        0        0     1685 2023-05-24 22:06:03.724177 humanloop-0.4.3/humanloop/model/experiments_list_response.py
--rw-r--r--   0        0        0     1685 2023-05-24 22:06:03.724320 humanloop-0.4.3/humanloop/model/experiments_list_response.pyi
--rw-r--r--   0        0        0     6681 2023-05-24 22:06:03.724485 humanloop-0.4.3/humanloop/model/feedback.py
--rw-r--r--   0        0        0     6681 2023-05-24 22:06:03.724632 humanloop-0.4.3/humanloop/model/feedback.pyi
--rw-r--r--   0        0        0     1463 2023-05-24 22:06:03.724799 humanloop-0.4.3/humanloop/model/feedback_class.py
--rw-r--r--   0        0        0     1296 2023-05-24 22:06:03.724961 humanloop-0.4.3/humanloop/model/feedback_class.pyi
--rw-r--r--   0        0        0     3334 2023-05-24 22:06:03.725270 humanloop-0.4.3/humanloop/model/feedback_label_request.py
--rw-r--r--   0        0        0     3334 2023-05-24 22:06:03.725442 humanloop-0.4.3/humanloop/model/feedback_label_request.pyi
--rw-r--r--   0        0        0     7189 2023-05-24 22:06:03.725583 humanloop-0.4.3/humanloop/model/feedback_request.py
--rw-r--r--   0        0        0     7189 2023-05-24 22:06:03.725820 humanloop-0.4.3/humanloop/model/feedback_request.pyi
--rw-r--r--   0        0        0     7141 2023-05-24 22:06:03.726014 humanloop-0.4.3/humanloop/model/feedback_response.py
--rw-r--r--   0        0        0     7141 2023-05-24 22:06:03.726184 humanloop-0.4.3/humanloop/model/feedback_response.pyi
--rw-r--r--   0        0        0     3200 2023-05-24 22:06:03.726345 humanloop-0.4.3/humanloop/model/feedback_submit_request.py
--rw-r--r--   0        0        0     3200 2023-05-24 22:06:03.726522 humanloop-0.4.3/humanloop/model/feedback_submit_request.pyi
--rw-r--r--   0        0        0     3210 2023-05-24 22:06:03.726701 humanloop-0.4.3/humanloop/model/feedback_submit_response.py
--rw-r--r--   0        0        0     3210 2023-05-24 22:06:03.726874 humanloop-0.4.3/humanloop/model/feedback_submit_response.pyi
--rw-r--r--   0        0        0     1690 2023-05-24 22:06:03.727066 humanloop-0.4.3/humanloop/model/feedback_type.py
--rw-r--r--   0        0        0     1459 2023-05-24 22:06:03.727243 humanloop-0.4.3/humanloop/model/feedback_type.pyi
--rw-r--r--   0        0        0     6161 2023-05-24 22:06:03.727420 humanloop-0.4.3/humanloop/model/feedback_type_model.py
--rw-r--r--   0        0        0     6161 2023-05-24 22:06:03.727586 humanloop-0.4.3/humanloop/model/feedback_type_model.pyi
--rw-r--r--   0        0        0     6289 2023-05-24 22:06:03.727734 humanloop-0.4.3/humanloop/model/feedback_type_request.py
--rw-r--r--   0        0        0     6289 2023-05-24 22:06:03.727899 humanloop-0.4.3/humanloop/model/feedback_type_request.pyi
--rw-r--r--   0        0        0     1659 2023-05-24 22:06:03.728106 humanloop-0.4.3/humanloop/model/feedback_types.py
--rw-r--r--   0        0        0     1659 2023-05-24 22:06:03.728425 humanloop-0.4.3/humanloop/model/feedback_types.pyi
--rw-r--r--   0        0        0     4407 2023-05-24 22:06:03.728613 humanloop-0.4.3/humanloop/model/generic_config_request.py
--rw-r--r--   0        0        0     4238 2023-05-24 22:06:03.728780 humanloop-0.4.3/humanloop/model/generic_config_request.pyi
--rw-r--r--   0        0        0     6562 2023-05-24 22:06:03.728933 humanloop-0.4.3/humanloop/model/generic_config_response.py
--rw-r--r--   0        0        0     6562 2023-05-24 22:06:03.729098 humanloop-0.4.3/humanloop/model/generic_config_response.pyi
--rw-r--r--   0        0        0     9619 2023-05-24 22:06:03.729296 humanloop-0.4.3/humanloop/model/get_model_config_response.py
--rw-r--r--   0        0        0     9619 2023-05-24 22:06:03.729546 humanloop-0.4.3/humanloop/model/get_model_config_response.pyi
--rw-r--r--   0        0        0     3611 2023-05-24 22:06:03.729728 humanloop-0.4.3/humanloop/model/http_validation_error.py
--rw-r--r--   0        0        0     3611 2023-05-24 22:06:03.729880 humanloop-0.4.3/humanloop/model/http_validation_error.pyi
--rw-r--r--   0        0        0     1667 2023-05-24 22:06:03.730032 humanloop-0.4.3/humanloop/model/label_sentiment.py
--rw-r--r--   0        0        0     1468 2023-05-24 22:06:03.730188 humanloop-0.4.3/humanloop/model/label_sentiment.pyi
--rw-r--r--   0        0        0     3156 2023-05-24 22:06:03.730336 humanloop-0.4.3/humanloop/model/log_datapoint_request.py
--rw-r--r--   0        0        0     3156 2023-05-24 22:06:03.730502 humanloop-0.4.3/humanloop/model/log_datapoint_request.pyi
--rw-r--r--   0        0        0    17219 2023-05-24 22:06:03.730707 humanloop-0.4.3/humanloop/model/log_model_config_request.py
--rw-r--r--   0        0        0    17219 2023-05-24 22:06:03.730945 humanloop-0.4.3/humanloop/model/log_model_config_request.pyi
--rw-r--r--   0        0        0    15844 2023-05-24 22:06:03.731183 humanloop-0.4.3/humanloop/model/log_request.py
--rw-r--r--   0        0        0    15844 2023-05-24 22:06:03.731400 humanloop-0.4.3/humanloop/model/log_request.pyi
--rw-r--r--   0        0        0    20160 2023-05-24 22:06:03.731655 humanloop-0.4.3/humanloop/model/log_response.py
--rw-r--r--   0        0        0    20160 2023-05-24 22:06:03.731908 humanloop-0.4.3/humanloop/model/log_response.pyi
--rw-r--r--   0        0        0     3205 2023-05-24 22:06:03.732126 humanloop-0.4.3/humanloop/model/logs_log_response.py
--rw-r--r--   0        0        0     3205 2023-05-24 22:06:03.732274 humanloop-0.4.3/humanloop/model/logs_log_response.pyi
--rw-r--r--   0        0        0    16246 2023-05-24 22:06:03.732446 humanloop-0.4.3/humanloop/model/model_config_chat_request.py
--rw-r--r--   0        0        0    16246 2023-05-24 22:06:03.732691 humanloop-0.4.3/humanloop/model/model_config_chat_request.pyi
--rw-r--r--   0        0        0    15386 2023-05-24 22:06:03.732906 humanloop-0.4.3/humanloop/model/model_config_completion_request.py
--rw-r--r--   0        0        0    15386 2023-05-24 22:06:03.733108 humanloop-0.4.3/humanloop/model/model_config_completion_request.pyi
--rw-r--r--   0        0        0    17859 2023-05-24 22:06:03.733276 humanloop-0.4.3/humanloop/model/model_config_response.py
--rw-r--r--   0        0        0    17859 2023-05-24 22:06:03.733423 humanloop-0.4.3/humanloop/model/model_config_response.pyi
--rw-r--r--   0        0        0    20554 2023-05-24 22:06:03.733574 humanloop-0.4.3/humanloop/model/model_config_response2.py
--rw-r--r--   0        0        0    20554 2023-05-24 22:06:03.733716 humanloop-0.4.3/humanloop/model/model_config_response2.pyi
--rw-r--r--   0        0        0     1460 2023-05-24 22:06:03.733826 humanloop-0.4.3/humanloop/model/model_endpoints.py
--rw-r--r--   0        0        0     1305 2023-05-24 22:06:03.733948 humanloop-0.4.3/humanloop/model/model_endpoints.pyi
--rw-r--r--   0        0        0     1695 2023-05-24 22:06:03.734084 humanloop-0.4.3/humanloop/model/model_providers.py
--rw-r--r--   0        0        0     1468 2023-05-24 22:06:03.734183 humanloop-0.4.3/humanloop/model/model_providers.pyi
--rw-r--r--   0        0        0     5144 2023-05-24 22:06:03.734269 humanloop-0.4.3/humanloop/model/paginated_data_log_response.py
--rw-r--r--   0        0        0     5144 2023-05-24 22:06:03.734394 humanloop-0.4.3/humanloop/model/paginated_data_log_response.pyi
--rw-r--r--   0        0        0     5180 2023-05-24 22:06:03.734507 humanloop-0.4.3/humanloop/model/paginated_data_project_response.py
--rw-r--r--   0        0        0     5180 2023-05-24 22:06:03.734604 humanloop-0.4.3/humanloop/model/paginated_data_project_response.pyi
--rw-r--r--   0        0        0     5180 2023-05-24 22:06:03.734706 humanloop-0.4.3/humanloop/model/paginated_data_session_response.py
--rw-r--r--   0        0        0     5180 2023-05-24 22:06:03.734798 humanloop-0.4.3/humanloop/model/paginated_data_session_response.pyi
--rw-r--r--   0        0        0     3143 2023-05-24 22:06:03.734891 humanloop-0.4.3/humanloop/model/positive_label.py
--rw-r--r--   0        0        0     3143 2023-05-24 22:06:03.734994 humanloop-0.4.3/humanloop/model/positive_label.pyi
--rw-r--r--   0        0        0     8900 2023-05-24 22:06:03.735098 humanloop-0.4.3/humanloop/model/project_config_response.py
--rw-r--r--   0        0        0     8900 2023-05-24 22:06:03.735217 humanloop-0.4.3/humanloop/model/project_config_response.pyi
--rw-r--r--   0        0        0    18363 2023-05-24 22:06:03.735353 humanloop-0.4.3/humanloop/model/project_model_config_request.py
--rw-r--r--   0        0        0    18363 2023-05-24 22:06:03.735479 humanloop-0.4.3/humanloop/model/project_model_config_request.pyi
--rw-r--r--   0        0        0    23968 2023-05-24 22:06:03.735623 humanloop-0.4.3/humanloop/model/project_model_config_response.py
--rw-r--r--   0        0        0    23968 2023-05-24 22:06:03.735787 humanloop-0.4.3/humanloop/model/project_model_config_response.pyi
--rw-r--r--   0        0        0    13895 2023-05-24 22:06:03.735934 humanloop-0.4.3/humanloop/model/project_response.py
--rw-r--r--   0        0        0    13895 2023-05-24 22:06:03.736095 humanloop-0.4.3/humanloop/model/project_response.pyi
--rw-r--r--   0        0        0     1471 2023-05-24 22:06:03.736234 humanloop-0.4.3/humanloop/model/project_sort_by.py
--rw-r--r--   0        0        0     1300 2023-05-24 22:06:03.736456 humanloop-0.4.3/humanloop/model/project_sort_by.pyi
--rw-r--r--   0        0        0     3795 2023-05-24 22:06:03.736848 humanloop-0.4.3/humanloop/model/project_user_response.py
--rw-r--r--   0        0        0     3795 2023-05-24 22:06:03.737012 humanloop-0.4.3/humanloop/model/project_user_response.pyi
--rw-r--r--   0        0        0     1713 2023-05-24 22:06:03.737157 humanloop-0.4.3/humanloop/model/projects_get_configs_response.py
--rw-r--r--   0        0        0     1713 2023-05-24 22:06:03.737389 humanloop-0.4.3/humanloop/model/projects_get_configs_response.pyi
--rw-r--r--   0        0        0     1715 2023-05-24 22:06:03.737571 humanloop-0.4.3/humanloop/model/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0     1715 2023-05-24 22:06:03.737840 humanloop-0.4.3/humanloop/model/projects_update_feedback_types_request.pyi
--rw-r--r--   0        0        0     4150 2023-05-24 22:06:03.738021 humanloop-0.4.3/humanloop/model/provider_api_keys.py
--rw-r--r--   0        0        0     4150 2023-05-24 22:06:03.738178 humanloop-0.4.3/humanloop/model/provider_api_keys.pyi
--rw-r--r--   0        0        0     3113 2023-05-24 22:06:03.738338 humanloop-0.4.3/humanloop/model/session_project_response.py
--rw-r--r--   0        0        0     3113 2023-05-24 22:06:03.738509 humanloop-0.4.3/humanloop/model/session_project_response.pyi
--rw-r--r--   0        0        0     6620 2023-05-24 22:06:03.738724 humanloop-0.4.3/humanloop/model/session_response.py
--rw-r--r--   0        0        0     6620 2023-05-24 22:06:03.738903 humanloop-0.4.3/humanloop/model/session_response.pyi
--rw-r--r--   0        0        0     1309 2023-05-24 22:06:03.739070 humanloop-0.4.3/humanloop/model/sort_order.py
--rw-r--r--   0        0        0     1192 2023-05-24 22:06:03.739222 humanloop-0.4.3/humanloop/model/sort_order.pyi
--rw-r--r--   0        0        0     4889 2023-05-24 22:06:03.739409 humanloop-0.4.3/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4889 2023-05-24 22:06:03.739606 humanloop-0.4.3/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0     4893 2023-05-24 22:06:03.739757 humanloop-0.4.3/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4893 2023-05-24 22:06:03.739894 humanloop-0.4.3/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0     4951 2023-05-24 22:06:03.740032 humanloop-0.4.3/humanloop/model/tool_config_request.py
--rw-r--r--   0        0        0     4788 2023-05-24 22:06:03.740154 humanloop-0.4.3/humanloop/model/tool_config_request.pyi
--rw-r--r--   0        0        0     7064 2023-05-24 22:06:03.740291 humanloop-0.4.3/humanloop/model/tool_config_response.py
--rw-r--r--   0        0        0     7064 2023-05-24 22:06:03.740430 humanloop-0.4.3/humanloop/model/tool_config_response.pyi
--rw-r--r--   0        0        0     4232 2023-05-24 22:06:03.740574 humanloop-0.4.3/humanloop/model/tool_result_response.py
--rw-r--r--   0        0        0     4232 2023-05-24 22:06:03.740681 humanloop-0.4.3/humanloop/model/tool_result_response.pyi
--rw-r--r--   0        0        0    13080 2023-05-24 22:06:03.740805 humanloop-0.4.3/humanloop/model/trace_log_request.py
--rw-r--r--   0        0        0    13080 2023-05-24 22:06:03.740968 humanloop-0.4.3/humanloop/model/trace_log_request.pyi
--rw-r--r--   0        0        0    19510 2023-05-24 22:06:03.741143 humanloop-0.4.3/humanloop/model/trace_model_config_request.py
--rw-r--r--   0        0        0    19345 2023-05-24 22:06:03.741282 humanloop-0.4.3/humanloop/model/trace_model_config_request.pyi
--rw-r--r--   0        0        0     7302 2023-05-24 22:06:03.741393 humanloop-0.4.3/humanloop/model/update_experiment_request.py
--rw-r--r--   0        0        0     7302 2023-05-24 22:06:03.741496 humanloop-0.4.3/humanloop/model/update_experiment_request.pyi
--rw-r--r--   0        0        0     5047 2023-05-24 22:06:03.741604 humanloop-0.4.3/humanloop/model/update_project_request.py
--rw-r--r--   0        0        0     5047 2023-05-24 22:06:03.741696 humanloop-0.4.3/humanloop/model/update_project_request.pyi
--rw-r--r--   0        0        0     4118 2023-05-24 22:06:03.741793 humanloop-0.4.3/humanloop/model/usage.py
--rw-r--r--   0        0        0     4118 2023-05-24 22:06:03.741900 humanloop-0.4.3/humanloop/model/usage.pyi
--rw-r--r--   0        0        0     6805 2023-05-24 22:06:03.742006 humanloop-0.4.3/humanloop/model/validation_error.py
--rw-r--r--   0        0        0     6805 2023-05-24 22:06:03.742112 humanloop-0.4.3/humanloop/model/validation_error.pyi
--rw-r--r--   0        0        0     6379 2023-05-24 22:06:03.742226 humanloop-0.4.3/humanloop/models/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-24 22:06:03.742335 humanloop-0.4.3/humanloop/paths/__init__.py
--rw-r--r--   0        0        0      285 2023-05-24 22:06:03.742439 humanloop-0.4.3/humanloop/paths/chat/__init__.py
--rw-r--r--   0        0        0    17428 2023-05-24 22:06:03.742552 humanloop-0.4.3/humanloop/paths/chat/post.py
--rw-r--r--   0        0        0    17285 2023-05-24 22:06:03.742714 humanloop-0.4.3/humanloop/paths/chat/post.pyi
--rw-r--r--   0        0        0      302 2023-05-24 22:06:03.742828 humanloop-0.4.3/humanloop/paths/chat_deployed/__init__.py
--rw-r--r--   0        0        0    16991 2023-05-24 22:06:03.742949 humanloop-0.4.3/humanloop/paths/chat_deployed/post.py
--rw-r--r--   0        0        0    16848 2023-05-24 22:06:03.743075 humanloop-0.4.3/humanloop/paths/chat_deployed/post.pyi
--rw-r--r--   0        0        0      306 2023-05-24 22:06:03.743190 humanloop-0.4.3/humanloop/paths/chat_experiment/__init__.py
--rw-r--r--   0        0        0    17434 2023-05-24 22:06:03.743305 humanloop-0.4.3/humanloop/paths/chat_experiment/post.py
--rw-r--r--   0        0        0    17291 2023-05-24 22:06:03.743442 humanloop-0.4.3/humanloop/paths/chat_experiment/post.pyi
--rw-r--r--   0        0        0      309 2023-05-24 22:06:03.743557 humanloop-0.4.3/humanloop/paths/chat_model_config/__init__.py
--rw-r--r--   0        0        0    17609 2023-05-24 22:06:03.743675 humanloop-0.4.3/humanloop/paths/chat_model_config/post.py
--rw-r--r--   0        0        0    17466 2023-05-24 22:06:03.743800 humanloop-0.4.3/humanloop/paths/chat_model_config/post.pyi
--rw-r--r--   0        0        0      297 2023-05-24 22:06:03.743915 humanloop-0.4.3/humanloop/paths/completion/__init__.py
--rw-r--r--   0        0        0    17744 2023-05-24 22:06:03.744028 humanloop-0.4.3/humanloop/paths/completion/post.py
--rw-r--r--   0        0        0    17601 2023-05-24 22:06:03.744151 humanloop-0.4.3/humanloop/paths/completion/post.pyi
--rw-r--r--   0        0        0      314 2023-05-24 22:06:03.744266 humanloop-0.4.3/humanloop/paths/completion_deployed/__init__.py
--rw-r--r--   0        0        0    17247 2023-05-24 22:06:03.744375 humanloop-0.4.3/humanloop/paths/completion_deployed/post.py
--rw-r--r--   0        0        0    17104 2023-05-24 22:06:03.744497 humanloop-0.4.3/humanloop/paths/completion_deployed/post.pyi
--rw-r--r--   0        0        0      318 2023-05-24 22:06:03.744603 humanloop-0.4.3/humanloop/paths/completion_experiment/__init__.py
--rw-r--r--   0        0        0    17690 2023-05-24 22:06:03.744719 humanloop-0.4.3/humanloop/paths/completion_experiment/post.py
--rw-r--r--   0        0        0    17547 2023-05-24 22:06:03.744839 humanloop-0.4.3/humanloop/paths/completion_experiment/post.pyi
--rw-r--r--   0        0        0      321 2023-05-24 22:06:03.744954 humanloop-0.4.3/humanloop/paths/completion_model_config/__init__.py
--rw-r--r--   0        0        0    17865 2023-05-24 22:06:03.745072 humanloop-0.4.3/humanloop/paths/completion_model_config/post.py
--rw-r--r--   0        0        0    17722 2023-05-24 22:06:03.745197 humanloop-0.4.3/humanloop/paths/completion_model_config/post.pyi
--rw-r--r--   0        0        0      327 2023-05-24 22:06:03.745313 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/__init__.py
--rw-r--r--   0        0        0    11995 2023-05-24 22:06:03.745433 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/delete.py
--rw-r--r--   0        0        0    11852 2023-05-24 22:06:03.745596 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/delete.pyi
--rw-r--r--   0        0        0    17043 2023-05-24 22:06:03.745746 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/patch.py
--rw-r--r--   0        0        0    16900 2023-05-24 22:06:03.745904 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/patch.pyi
--rw-r--r--   0        0        0      352 2023-05-24 22:06:03.746050 humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/__init__.py
--rw-r--r--   0        0        0    12496 2023-05-24 22:06:03.746196 humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/get.py
--rw-r--r--   0        0        0    12353 2023-05-24 22:06:03.746363 humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/get.pyi
--rw-r--r--   0        0        0      293 2023-05-24 22:06:03.746521 humanloop-0.4.3/humanloop/paths/feedback/__init__.py
--rw-r--r--   0        0        0    15089 2023-05-24 22:06:03.746635 humanloop-0.4.3/humanloop/paths/feedback/post.py
--rw-r--r--   0        0        0    14946 2023-05-24 22:06:03.746751 humanloop-0.4.3/humanloop/paths/feedback/post.pyi
--rw-r--r--   0        0        0      285 2023-05-24 22:06:03.746882 humanloop-0.4.3/humanloop/paths/logs/__init__.py
--rw-r--r--   0        0        0    20891 2023-05-24 22:06:03.746991 humanloop-0.4.3/humanloop/paths/logs/post.py
--rw-r--r--   0        0        0    20748 2023-05-24 22:06:03.747118 humanloop-0.4.3/humanloop/paths/logs/post.pyi
--rw-r--r--   0        0        0      302 2023-05-24 22:06:03.747236 humanloop-0.4.3/humanloop/paths/model_configs/__init__.py
--rw-r--r--   0        0        0    20266 2023-05-24 22:06:03.747345 humanloop-0.4.3/humanloop/paths/model_configs/post.py
--rw-r--r--   0        0        0    20123 2023-05-24 22:06:03.747469 humanloop-0.4.3/humanloop/paths/model_configs/post.pyi
--rw-r--r--   0        0        0      308 2023-05-24 22:06:03.747607 humanloop-0.4.3/humanloop/paths/model_configs_id/__init__.py
--rw-r--r--   0        0        0    12023 2023-05-24 22:06:03.747716 humanloop-0.4.3/humanloop/paths/model_configs_id/get.py
--rw-r--r--   0        0        0    11880 2023-05-24 22:06:03.747848 humanloop-0.4.3/humanloop/paths/model_configs_id/get.pyi
--rw-r--r--   0        0        0      293 2023-05-24 22:06:03.748006 humanloop-0.4.3/humanloop/paths/projects/__init__.py
--rw-r--r--   0        0        0    20518 2023-05-24 22:06:03.748148 humanloop-0.4.3/humanloop/paths/projects/get.py
--rw-r--r--   0        0        0    20375 2023-05-24 22:06:03.748310 humanloop-0.4.3/humanloop/paths/projects/get.pyi
--rw-r--r--   0        0        0    13007 2023-05-24 22:06:03.748466 humanloop-0.4.3/humanloop/paths/projects/post.py
--rw-r--r--   0        0        0    12864 2023-05-24 22:06:03.748695 humanloop-0.4.3/humanloop/paths/projects/post.pyi
--rw-r--r--   0        0        0      299 2023-05-24 22:06:03.748985 humanloop-0.4.3/humanloop/paths/projects_id/__init__.py
--rw-r--r--   0        0        0    11979 2023-05-24 22:06:03.749157 humanloop-0.4.3/humanloop/paths/projects_id/get.py
--rw-r--r--   0        0        0    11836 2023-05-24 22:06:03.749353 humanloop-0.4.3/humanloop/paths/projects_id/get.pyi
--rw-r--r--   0        0        0    16066 2023-05-24 22:06:03.749512 humanloop-0.4.3/humanloop/paths/projects_id/patch.py
--rw-r--r--   0        0        0    15923 2023-05-24 22:06:03.749708 humanloop-0.4.3/humanloop/paths/projects_id/patch.pyi
--rw-r--r--   0        0        0      326 2023-05-24 22:06:03.749882 humanloop-0.4.3/humanloop/paths/projects_id_active_config/__init__.py
--rw-r--r--   0        0        0    12298 2023-05-24 22:06:03.750004 humanloop-0.4.3/humanloop/paths/projects_id_active_config/delete.py
--rw-r--r--   0        0        0    12155 2023-05-24 22:06:03.750137 humanloop-0.4.3/humanloop/paths/projects_id_active_config/delete.pyi
--rw-r--r--   0        0        0    12148 2023-05-24 22:06:03.750271 humanloop-0.4.3/humanloop/paths/projects_id_active_config/get.py
--rw-r--r--   0        0        0    12005 2023-05-24 22:06:03.750392 humanloop-0.4.3/humanloop/paths/projects_id_active_config/get.pyi
--rw-r--r--   0        0        0      334 2023-05-24 22:06:03.750516 humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/__init__.py
--rw-r--r--   0        0        0    12306 2023-05-24 22:06:03.750628 humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/delete.py
--rw-r--r--   0        0        0    12163 2023-05-24 22:06:03.750767 humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/delete.pyi
--rw-r--r--   0        0        0      315 2023-05-24 22:06:03.750894 humanloop-0.4.3/humanloop/paths/projects_id_configs/__init__.py
--rw-r--r--   0        0        0    12182 2023-05-24 22:06:03.751001 humanloop-0.4.3/humanloop/paths/projects_id_configs/get.py
--rw-r--r--   0        0        0    12039 2023-05-24 22:06:03.751129 humanloop-0.4.3/humanloop/paths/projects_id_configs/get.pyi
--rw-r--r--   0        0        0      313 2023-05-24 22:06:03.751265 humanloop-0.4.3/humanloop/paths/projects_id_export/__init__.py
--rw-r--r--   0        0        0    15728 2023-05-24 22:06:03.751382 humanloop-0.4.3/humanloop/paths/projects_id_export/post.py
--rw-r--r--   0        0        0    15585 2023-05-24 22:06:03.751582 humanloop-0.4.3/humanloop/paths/projects_id_export/post.pyi
--rw-r--r--   0        0        0      328 2023-05-24 22:06:03.751786 humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/__init__.py
--rw-r--r--   0        0        0    14798 2023-05-24 22:06:03.751939 humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/patch.py
--rw-r--r--   0        0        0    14655 2023-05-24 22:06:03.752106 humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/patch.pyi
--rw-r--r--   0        0        0      339 2023-05-24 22:06:03.752249 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/__init__.py
--rw-r--r--   0        0        0    12256 2023-05-24 22:06:03.752365 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/get.py
--rw-r--r--   0        0        0    12113 2023-05-24 22:06:03.752514 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/get.pyi
--rw-r--r--   0        0        0    16250 2023-05-24 22:06:03.752654 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/post.py
--rw-r--r--   0        0        0    16107 2023-05-24 22:06:03.752805 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/post.pyi
--rw-r--r--   0        0        0      293 2023-05-24 22:06:03.752947 humanloop-0.4.3/humanloop/paths/sessions/__init__.py
--rw-r--r--   0        0        0    14112 2023-05-24 22:06:03.753066 humanloop-0.4.3/humanloop/paths/sessions/get.py
--rw-r--r--   0        0        0    13969 2023-05-24 22:06:03.753213 humanloop-0.4.3/humanloop/paths/sessions/get.pyi
--rw-r--r--   0        0        0     9192 2023-05-24 22:06:03.753373 humanloop-0.4.3/humanloop/paths/sessions/post.py
--rw-r--r--   0        0        0     9079 2023-05-24 22:06:03.753520 humanloop-0.4.3/humanloop/paths/sessions/post.pyi
--rw-r--r--   0        0        0      299 2023-05-24 22:06:03.753632 humanloop-0.4.3/humanloop/paths/sessions_id/__init__.py
--rw-r--r--   0        0        0    11979 2023-05-24 22:06:03.753726 humanloop-0.4.3/humanloop/paths/sessions_id/get.py
--rw-r--r--   0        0        0    11836 2023-05-24 22:06:03.753835 humanloop-0.4.3/humanloop/paths/sessions_id/get.pyi
--rw-r--r--   0        0        0      289 2023-05-24 22:06:03.753950 humanloop-0.4.3/humanloop/paths/traces/__init__.py
--rw-r--r--   0        0        0    12450 2023-05-24 22:06:03.754045 humanloop-0.4.3/humanloop/paths/traces/post.py
--rw-r--r--   0        0        0    12307 2023-05-24 22:06:03.754172 humanloop-0.4.3/humanloop/paths/traces/post.pyi
--rw-r--r--   0        0        0     1011 2023-05-24 22:06:03.754339 humanloop-0.4.3/humanloop/request_after_hook.py
--rw-r--r--   0        0        0     1783 2023-05-18 18:32:32.791241 humanloop-0.4.3/humanloop/request_before_hook.py
--rw-r--r--   0        0        0    11329 2023-05-24 22:06:03.754495 humanloop-0.4.3/humanloop/rest.py
--rw-r--r--   0        0        0    95913 2023-05-24 22:06:03.754835 humanloop-0.4.3/humanloop/schemas.py
--rw-r--r--   0        0        0        0 2023-05-24 22:06:03.755019 humanloop-0.4.3/humanloop/type/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-24 22:06:03.755158 humanloop-0.4.3/humanloop/type/agent_config_request.py
--rw-r--r--   0        0        0     1608 2023-05-24 22:06:03.755284 humanloop-0.4.3/humanloop/type/agent_config_response.py
--rw-r--r--   0        0        0     1408 2023-05-24 22:06:03.755421 humanloop-0.4.3/humanloop/type/base_metric_response.py
--rw-r--r--   0        0        0     1062 2023-05-24 22:06:03.755561 humanloop-0.4.3/humanloop/type/categorical_feedback_label.py
--rw-r--r--   0        0        0     2183 2023-05-24 22:06:03.755696 humanloop-0.4.3/humanloop/type/chat_data_response.py
--rw-r--r--   0        0        0     1990 2023-05-24 22:06:03.755854 humanloop-0.4.3/humanloop/type/chat_deployed_request.py
--rw-r--r--   0        0        0     2235 2023-05-24 22:06:03.756004 humanloop-0.4.3/humanloop/type/chat_experiment_request.py
--rw-r--r--   0        0        0      919 2023-05-24 22:06:03.756134 humanloop-0.4.3/humanloop/type/chat_message.py
--rw-r--r--   0        0        0     2104 2023-05-24 22:06:03.756259 humanloop-0.4.3/humanloop/type/chat_model_config_request.py
--rw-r--r--   0        0        0     2130 2023-05-24 22:06:03.756382 humanloop-0.4.3/humanloop/type/chat_request.py
--rw-r--r--   0        0        0     1818 2023-05-24 22:06:03.756494 humanloop-0.4.3/humanloop/type/chat_response.py
--rw-r--r--   0        0        0      711 2023-05-24 22:06:03.756615 humanloop-0.4.3/humanloop/type/chat_role.py
--rw-r--r--   0        0        0     2095 2023-05-24 22:06:03.756732 humanloop-0.4.3/humanloop/type/completion_deployed_request.py
--rw-r--r--   0        0        0     2343 2023-05-24 22:06:03.756847 humanloop-0.4.3/humanloop/type/completion_experiment_request.py
--rw-r--r--   0        0        0     2209 2023-05-24 22:06:03.756957 humanloop-0.4.3/humanloop/type/completion_model_config_request.py
--rw-r--r--   0        0        0     2239 2023-05-24 22:06:03.757075 humanloop-0.4.3/humanloop/type/completion_request.py
--rw-r--r--   0        0        0     1864 2023-05-24 22:06:03.757193 humanloop-0.4.3/humanloop/type/completion_response.py
--rw-r--r--   0        0        0     1054 2023-05-24 22:06:03.757293 humanloop-0.4.3/humanloop/type/config_response.py
--rw-r--r--   0        0        0      719 2023-05-24 22:06:03.757420 humanloop-0.4.3/humanloop/type/config_type.py
--rw-r--r--   0        0        0     1362 2023-05-24 22:06:03.757542 humanloop-0.4.3/humanloop/type/create_experiment_request.py
--rw-r--r--   0        0        0     1024 2023-05-24 22:06:03.757663 humanloop-0.4.3/humanloop/type/create_log_response.py
--rw-r--r--   0        0        0     1066 2023-05-24 22:06:03.757780 humanloop-0.4.3/humanloop/type/create_project_request.py
--rw-r--r--   0        0        0      942 2023-05-24 22:06:03.757897 humanloop-0.4.3/humanloop/type/create_session_response.py
--rw-r--r--   0        0        0     1045 2023-05-24 22:06:03.757998 humanloop-0.4.3/humanloop/type/create_trace_request.py
--rw-r--r--   0        0        0      998 2023-05-24 22:06:03.758100 humanloop-0.4.3/humanloop/type/create_trace_response.py
--rw-r--r--   0        0        0     2013 2023-05-24 22:06:03.758199 humanloop-0.4.3/humanloop/type/data_response.py
--rw-r--r--   0        0        0     1677 2023-05-24 22:06:03.758296 humanloop-0.4.3/humanloop/type/experiment_config_response.py
--rw-r--r--   0        0        0     1788 2023-05-24 22:06:03.758394 humanloop-0.4.3/humanloop/type/experiment_response.py
--rw-r--r--   0        0        0      718 2023-05-24 22:06:03.758484 humanloop-0.4.3/humanloop/type/experiment_status.py
--rw-r--r--   0        0        0      785 2023-05-24 22:06:03.758608 humanloop-0.4.3/humanloop/type/experiments_list_response.py
--rw-r--r--   0        0        0     1449 2023-05-24 22:06:03.758837 humanloop-0.4.3/humanloop/type/feedback.py
--rw-r--r--   0        0        0      719 2023-05-24 22:06:03.759458 humanloop-0.4.3/humanloop/type/feedback_class.py
--rw-r--r--   0        0        0      970 2023-05-24 22:06:03.759997 humanloop-0.4.3/humanloop/type/feedback_label_request.py
--rw-r--r--   0        0        0     1546 2023-05-24 22:06:03.762133 humanloop-0.4.3/humanloop/type/feedback_request.py
--rw-r--r--   0        0        0     1578 2023-05-24 22:06:03.762307 humanloop-0.4.3/humanloop/type/feedback_response.py
--rw-r--r--   0        0        0      804 2023-05-24 22:06:03.762411 humanloop-0.4.3/humanloop/type/feedback_submit_request.py
--rw-r--r--   0        0        0      809 2023-05-24 22:06:03.762504 humanloop-0.4.3/humanloop/type/feedback_submit_response.py
--rw-r--r--   0        0        0      738 2023-05-24 22:06:03.762594 humanloop-0.4.3/humanloop/type/feedback_type.py
--rw-r--r--   0        0        0     1307 2023-05-24 22:06:03.762689 humanloop-0.4.3/humanloop/type/feedback_type_model.py
--rw-r--r--   0        0        0     1541 2023-05-24 22:06:03.762785 humanloop-0.4.3/humanloop/type/feedback_type_request.py
--rw-r--r--   0        0        0      773 2023-05-24 22:06:03.762880 humanloop-0.4.3/humanloop/type/feedback_types.py
--rw-r--r--   0        0        0     1064 2023-05-24 22:06:03.762973 humanloop-0.4.3/humanloop/type/generic_config_request.py
--rw-r--r--   0        0        0     1262 2023-05-24 22:06:03.763058 humanloop-0.4.3/humanloop/type/generic_config_response.py
--rw-r--r--   0        0        0     1900 2023-05-24 22:06:03.763147 humanloop-0.4.3/humanloop/type/get_model_config_response.py
--rw-r--r--   0        0        0      972 2023-05-24 22:06:03.763244 humanloop-0.4.3/humanloop/type/http_validation_error.py
--rw-r--r--   0        0        0      730 2023-05-24 22:06:03.763332 humanloop-0.4.3/humanloop/type/label_sentiment.py
--rw-r--r--   0        0        0      782 2023-05-24 22:06:03.763422 humanloop-0.4.3/humanloop/type/log_datapoint_request.py
--rw-r--r--   0        0        0     3033 2023-05-24 22:06:03.763511 humanloop-0.4.3/humanloop/type/log_model_config_request.py
--rw-r--r--   0        0        0     2652 2023-05-24 22:06:03.763609 humanloop-0.4.3/humanloop/type/log_request.py
--rw-r--r--   0        0        0     2961 2023-05-24 22:06:03.763734 humanloop-0.4.3/humanloop/type/log_response.py
--rw-r--r--   0        0        0      807 2023-05-24 22:06:03.763827 humanloop-0.4.3/humanloop/type/logs_log_response.py
--rw-r--r--   0        0        0     2820 2023-05-24 22:06:03.763975 humanloop-0.4.3/humanloop/type/model_config_chat_request.py
--rw-r--r--   0        0        0     2713 2023-05-24 22:06:03.764081 humanloop-0.4.3/humanloop/type/model_config_completion_request.py
--rw-r--r--   0        0        0     3160 2023-05-24 22:06:03.764178 humanloop-0.4.3/humanloop/type/model_config_response.py
--rw-r--r--   0        0        0     3281 2023-05-24 22:06:03.764276 humanloop-0.4.3/humanloop/type/model_config_response2.py
--rw-r--r--   0        0        0      714 2023-05-24 22:06:03.764381 humanloop-0.4.3/humanloop/type/model_endpoints.py
--rw-r--r--   0        0        0      738 2023-05-24 22:06:03.764475 humanloop-0.4.3/humanloop/type/model_providers.py
--rw-r--r--   0        0        0     1032 2023-05-24 22:06:03.764575 humanloop-0.4.3/humanloop/type/paginated_data_log_response.py
--rw-r--r--   0        0        0     1064 2023-05-24 22:06:03.764679 humanloop-0.4.3/humanloop/type/paginated_data_project_response.py
--rw-r--r--   0        0        0     1064 2023-05-24 22:06:03.764787 humanloop-0.4.3/humanloop/type/paginated_data_session_response.py
--rw-r--r--   0        0        0      871 2023-05-24 22:06:03.764902 humanloop-0.4.3/humanloop/type/positive_label.py
--rw-r--r--   0        0        0     1820 2023-05-24 22:06:03.765015 humanloop-0.4.3/humanloop/type/project_config_response.py
--rw-r--r--   0        0        0     3410 2023-05-24 22:06:03.765111 humanloop-0.4.3/humanloop/type/project_model_config_request.py
--rw-r--r--   0        0        0     4053 2023-05-24 22:06:03.765205 humanloop-0.4.3/humanloop/type/project_model_config_response.py
--rw-r--r--   0        0        0     2032 2023-05-24 22:06:03.765293 humanloop-0.4.3/humanloop/type/project_response.py
--rw-r--r--   0        0        0      721 2023-05-24 22:06:03.765388 humanloop-0.4.3/humanloop/type/project_sort_by.py
--rw-r--r--   0        0        0     1022 2023-05-24 22:06:03.765485 humanloop-0.4.3/humanloop/type/project_user_response.py
--rw-r--r--   0        0        0      798 2023-05-24 22:06:03.765580 humanloop-0.4.3/humanloop/type/projects_get_configs_response.py
--rw-r--r--   0        0        0      800 2023-05-24 22:06:03.765682 humanloop-0.4.3/humanloop/type/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0      917 2023-05-24 22:06:03.765798 humanloop-0.4.3/humanloop/type/provider_api_keys.py
--rw-r--r--   0        0        0      985 2023-05-24 22:06:03.765927 humanloop-0.4.3/humanloop/type/session_project_response.py
--rw-r--r--   0        0        0     1442 2023-05-24 22:06:03.766058 humanloop-0.4.3/humanloop/type/session_response.py
--rw-r--r--   0        0        0      696 2023-05-24 22:06:03.766171 humanloop-0.4.3/humanloop/type/sort_order.py
--rw-r--r--   0        0        0     1241 2023-05-24 22:06:03.766286 humanloop-0.4.3/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     1251 2023-05-24 22:06:03.766402 humanloop-0.4.3/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     1066 2023-05-24 22:06:03.766520 humanloop-0.4.3/humanloop/type/tool_config_request.py
--rw-r--r--   0        0        0     1295 2023-05-24 22:06:03.766635 humanloop-0.4.3/humanloop/type/tool_config_response.py
--rw-r--r--   0        0        0      930 2023-05-24 22:06:03.766746 humanloop-0.4.3/humanloop/type/tool_result_response.py
--rw-r--r--   0        0        0     2427 2023-05-24 22:06:03.766879 humanloop-0.4.3/humanloop/type/trace_log_request.py
--rw-r--r--   0        0        0     3095 2023-05-24 22:06:03.767004 humanloop-0.4.3/humanloop/type/trace_model_config_request.py
--rw-r--r--   0        0        0     1361 2023-05-24 22:06:03.767116 humanloop-0.4.3/humanloop/type/update_experiment_request.py
--rw-r--r--   0        0        0     1434 2023-05-24 22:06:03.767212 humanloop-0.4.3/humanloop/type/update_project_request.py
--rw-r--r--   0        0        0     1042 2023-05-24 22:06:03.767315 humanloop-0.4.3/humanloop/type/usage.py
--rw-r--r--   0        0        0      951 2023-05-24 22:06:03.767416 humanloop-0.4.3/humanloop/type/validation_error.py
--rw-r--r--   0        0        0      868 2023-05-24 22:06:03.767517 humanloop-0.4.3/humanloop/type_util.py
--rw-r--r--   0        0        0     3165 2023-05-24 22:06:03.767629 humanloop-0.4.3/humanloop/validation_metadata.py
--rw-r--r--   0        0        0      714 2023-05-24 22:06:03.768046 humanloop-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     9366 1970-01-01 00:00:00.000000 humanloop-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-26 00:09:33.462092 humanloop-0.4.4/LICENSE
+-rw-r--r--   0        0        0     8475 2023-05-26 00:09:33.509250 humanloop-0.4.4/README.md
+-rw-r--r--   0        0        0     1059 2023-05-26 00:09:33.370349 humanloop-0.4.4/humanloop/__init__.py
+-rw-r--r--   0        0        0    73009 2023-05-26 00:09:33.370543 humanloop-0.4.4/humanloop/api_client.py
+-rw-r--r--   0        0        0      663 2023-05-26 00:09:33.370741 humanloop-0.4.4/humanloop/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-26 00:09:33.370909 humanloop-0.4.4/humanloop/apis/__init__.py
+-rw-r--r--   0        0        0     4578 2023-05-26 00:09:33.371066 humanloop-0.4.4/humanloop/apis/path_to_api.py
+-rw-r--r--   0        0        0      236 2023-05-26 00:09:33.371192 humanloop-0.4.4/humanloop/apis/paths/__init__.py
+-rw-r--r--   0        0        0       91 2023-05-26 00:09:33.371287 humanloop-0.4.4/humanloop/apis/paths/chat.py
+-rw-r--r--   0        0        0      108 2023-05-26 00:09:33.371416 humanloop-0.4.4/humanloop/apis/paths/chat_deployed.py
+-rw-r--r--   0        0        0      112 2023-05-26 00:09:33.371553 humanloop-0.4.4/humanloop/apis/paths/chat_experiment.py
+-rw-r--r--   0        0        0      115 2023-05-26 00:09:33.371727 humanloop-0.4.4/humanloop/apis/paths/chat_model_config.py
+-rw-r--r--   0        0        0      103 2023-05-26 00:09:33.371884 humanloop-0.4.4/humanloop/apis/paths/completion.py
+-rw-r--r--   0        0        0      120 2023-05-26 00:09:33.372030 humanloop-0.4.4/humanloop/apis/paths/completion_deployed.py
+-rw-r--r--   0        0        0      124 2023-05-26 00:09:33.372167 humanloop-0.4.4/humanloop/apis/paths/completion_experiment.py
+-rw-r--r--   0        0        0      127 2023-05-26 00:09:33.372312 humanloop-0.4.4/humanloop/apis/paths/completion_model_config.py
+-rw-r--r--   0        0        0      226 2023-05-26 00:09:33.372517 humanloop-0.4.4/humanloop/apis/paths/experiments_experiment_id.py
+-rw-r--r--   0        0        0      152 2023-05-26 00:09:33.372689 humanloop-0.4.4/humanloop/apis/paths/experiments_experiment_id_model_config.py
+-rw-r--r--   0        0        0       99 2023-05-26 00:09:33.372846 humanloop-0.4.4/humanloop/apis/paths/feedback.py
+-rw-r--r--   0        0        0       91 2023-05-26 00:09:33.373002 humanloop-0.4.4/humanloop/apis/paths/logs.py
+-rw-r--r--   0        0        0      108 2023-05-26 00:09:33.373160 humanloop-0.4.4/humanloop/apis/paths/model_configs.py
+-rw-r--r--   0        0        0      110 2023-05-26 00:09:33.373327 humanloop-0.4.4/humanloop/apis/paths/model_configs_id.py
+-rw-r--r--   0        0        0      165 2023-05-26 00:09:33.373484 humanloop-0.4.4/humanloop/apis/paths/projects.py
+-rw-r--r--   0        0        0      176 2023-05-26 00:09:33.373645 humanloop-0.4.4/humanloop/apis/paths/projects_id.py
+-rw-r--r--   0        0        0      219 2023-05-26 00:09:33.373795 humanloop-0.4.4/humanloop/apis/paths/projects_id_active_config.py
+-rw-r--r--   0        0        0      144 2023-05-26 00:09:33.373947 humanloop-0.4.4/humanloop/apis/paths/projects_id_active_experiment.py
+-rw-r--r--   0        0        0      116 2023-05-26 00:09:33.374084 humanloop-0.4.4/humanloop/apis/paths/projects_id_configs.py
+-rw-r--r--   0        0        0      117 2023-05-26 00:09:33.374234 humanloop-0.4.4/humanloop/apis/paths/projects_id_export.py
+-rw-r--r--   0        0        0      135 2023-05-26 00:09:33.374375 humanloop-0.4.4/humanloop/apis/paths/projects_id_feedback_types.py
+-rw-r--r--   0        0        0      231 2023-05-26 00:09:33.374528 humanloop-0.4.4/humanloop/apis/paths/projects_project_id_experiments.py
+-rw-r--r--   0        0        0      165 2023-05-26 00:09:33.374683 humanloop-0.4.4/humanloop/apis/paths/sessions.py
+-rw-r--r--   0        0        0      101 2023-05-26 00:09:33.375006 humanloop-0.4.4/humanloop/apis/paths/sessions_id.py
+-rw-r--r--   0        0        0       95 2023-05-26 00:09:33.375225 humanloop-0.4.4/humanloop/apis/paths/traces.py
+-rw-r--r--   0        0        0     1654 2023-05-26 00:09:33.375391 humanloop-0.4.4/humanloop/apis/tag_to_api.py
+-rw-r--r--   0        0        0      572 2023-05-26 00:09:33.375554 humanloop-0.4.4/humanloop/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1006 2023-05-26 00:09:33.375697 humanloop-0.4.4/humanloop/apis/tags/chats_api.py
+-rw-r--r--   0        0        0     1020 2023-05-26 00:09:33.375842 humanloop-0.4.4/humanloop/apis/tags/completions_api.py
+-rw-r--r--   0        0        0     1091 2023-05-26 00:09:33.375984 humanloop-0.4.4/humanloop/apis/tags/experiments_api.py
+-rw-r--r--   0        0        0      721 2023-05-26 00:09:33.376127 humanloop-0.4.4/humanloop/apis/tags/feedback_api.py
+-rw-r--r--   0        0        0      707 2023-05-26 00:09:33.376281 humanloop-0.4.4/humanloop/apis/tags/logs_api.py
+-rw-r--r--   0        0        0      803 2023-05-26 00:09:33.376418 humanloop-0.4.4/humanloop/apis/tags/model_configurations_api.py
+-rw-r--r--   0        0        0     1486 2023-05-26 00:09:33.376558 humanloop-0.4.4/humanloop/apis/tags/projects_api.py
+-rw-r--r--   0        0        0      834 2023-05-26 00:09:33.376707 humanloop-0.4.4/humanloop/apis/tags/sessions_api.py
+-rw-r--r--   0        0        0      717 2023-05-26 00:09:33.376890 humanloop-0.4.4/humanloop/apis/tags/traces_api.py
+-rw-r--r--   0        0        0    28032 2023-05-26 00:09:33.377102 humanloop-0.4.4/humanloop/client.py
+-rw-r--r--   0        0        0    28032 2023-05-26 00:09:33.377363 humanloop-0.4.4/humanloop/client.pyi
+-rw-r--r--   0        0        0     6780 2023-05-26 00:09:33.461499 humanloop-0.4.4/humanloop/client_custom.py
+-rw-r--r--   0        0        0    18674 2023-05-26 00:09:33.377771 humanloop-0.4.4/humanloop/configuration.py
+-rw-r--r--   0        0        0     7678 2023-05-26 00:09:33.377923 humanloop-0.4.4/humanloop/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-05-26 00:09:33.378073 humanloop-0.4.4/humanloop/exceptions_base.py
+-rw-r--r--   0        0        0      343 2023-05-26 00:09:33.378294 humanloop-0.4.4/humanloop/model/__init__.py
+-rw-r--r--   0        0        0     9140 2023-05-26 00:09:33.378430 humanloop-0.4.4/humanloop/model/agent_config_request.py
+-rw-r--r--   0        0        0     8975 2023-05-26 00:09:33.378583 humanloop-0.4.4/humanloop/model/agent_config_request.pyi
+-rw-r--r--   0        0        0    11140 2023-05-26 00:09:33.378781 humanloop-0.4.4/humanloop/model/agent_config_response.py
+-rw-r--r--   0        0        0    11140 2023-05-26 00:09:33.378963 humanloop-0.4.4/humanloop/model/agent_config_response.pyi
+-rw-r--r--   0        0        0     6379 2023-05-26 00:09:33.379130 humanloop-0.4.4/humanloop/model/base_metric_response.py
+-rw-r--r--   0        0        0     6379 2023-05-26 00:09:33.379267 humanloop-0.4.4/humanloop/model/base_metric_response.pyi
+-rw-r--r--   0        0        0     5150 2023-05-26 00:09:33.379404 humanloop-0.4.4/humanloop/model/categorical_feedback_label.py
+-rw-r--r--   0        0        0     5150 2023-05-26 00:09:33.379528 humanloop-0.4.4/humanloop/model/categorical_feedback_label.pyi
+-rw-r--r--   0        0        0     8957 2023-05-26 00:09:33.379697 humanloop-0.4.4/humanloop/model/chat_data_response.py
+-rw-r--r--   0        0        0     8957 2023-05-26 00:09:33.379968 humanloop-0.4.4/humanloop/model/chat_data_response.pyi
+-rw-r--r--   0        0        0     9998 2023-05-26 00:09:33.380203 humanloop-0.4.4/humanloop/model/chat_deployed_request.py
+-rw-r--r--   0        0        0     9998 2023-05-26 00:09:33.380397 humanloop-0.4.4/humanloop/model/chat_deployed_request.pyi
+-rw-r--r--   0        0        0    10659 2023-05-26 00:09:33.380532 humanloop-0.4.4/humanloop/model/chat_experiment_request.py
+-rw-r--r--   0        0        0    10659 2023-05-26 00:09:33.380642 humanloop-0.4.4/humanloop/model/chat_experiment_request.pyi
+-rw-r--r--   0        0        0     3702 2023-05-26 00:09:33.380742 humanloop-0.4.4/humanloop/model/chat_message.py
+-rw-r--r--   0        0        0     3702 2023-05-26 00:09:33.380870 humanloop-0.4.4/humanloop/model/chat_message.pyi
+-rw-r--r--   0        0        0    10693 2023-05-26 00:09:33.381686 humanloop-0.4.4/humanloop/model/chat_model_config_request.py
+-rw-r--r--   0        0        0    10693 2023-05-26 00:09:33.381926 humanloop-0.4.4/humanloop/model/chat_model_config_request.pyi
+-rw-r--r--   0        0        0    12556 2023-05-26 00:09:33.382103 humanloop-0.4.4/humanloop/model/chat_request.py
+-rw-r--r--   0        0        0    12556 2023-05-26 00:09:33.382263 humanloop-0.4.4/humanloop/model/chat_request.pyi
+-rw-r--r--   0        0        0    11076 2023-05-26 00:09:33.382438 humanloop-0.4.4/humanloop/model/chat_response.py
+-rw-r--r--   0        0        0    11076 2023-05-26 00:09:33.382606 humanloop-0.4.4/humanloop/model/chat_response.pyi
+-rw-r--r--   0        0        0     1446 2023-05-26 00:09:33.382751 humanloop-0.4.4/humanloop/model/chat_role.py
+-rw-r--r--   0        0        0     1285 2023-05-26 00:09:33.382870 humanloop-0.4.4/humanloop/model/chat_role.pyi
+-rw-r--r--   0        0        0     9674 2023-05-26 00:09:33.382985 humanloop-0.4.4/humanloop/model/completion_deployed_request.py
+-rw-r--r--   0        0        0     9674 2023-05-26 00:09:33.383129 humanloop-0.4.4/humanloop/model/completion_deployed_request.pyi
+-rw-r--r--   0        0        0    10340 2023-05-26 00:09:33.383270 humanloop-0.4.4/humanloop/model/completion_experiment_request.py
+-rw-r--r--   0        0        0    10340 2023-05-26 00:09:33.383396 humanloop-0.4.4/humanloop/model/completion_experiment_request.pyi
+-rw-r--r--   0        0        0    10376 2023-05-26 00:09:33.383699 humanloop-0.4.4/humanloop/model/completion_model_config_request.py
+-rw-r--r--   0        0        0    10376 2023-05-26 00:09:33.383857 humanloop-0.4.4/humanloop/model/completion_model_config_request.pyi
+-rw-r--r--   0        0        0    12258 2023-05-26 00:09:33.384017 humanloop-0.4.4/humanloop/model/completion_request.py
+-rw-r--r--   0        0        0    12258 2023-05-26 00:09:33.384162 humanloop-0.4.4/humanloop/model/completion_request.pyi
+-rw-r--r--   0        0        0    11017 2023-05-26 00:09:33.384298 humanloop-0.4.4/humanloop/model/completion_response.py
+-rw-r--r--   0        0        0    11017 2023-05-26 00:09:33.384424 humanloop-0.4.4/humanloop/model/completion_response.pyi
+-rw-r--r--   0        0        0     2672 2023-05-26 00:09:33.384526 humanloop-0.4.4/humanloop/model/config_response.py
+-rw-r--r--   0        0        0     2672 2023-05-26 00:09:33.384626 humanloop-0.4.4/humanloop/model/config_response.pyi
+-rw-r--r--   0        0        0     1546 2023-05-26 00:09:33.384720 humanloop-0.4.4/humanloop/model/config_type.py
+-rw-r--r--   0        0        0     1361 2023-05-26 00:09:33.384829 humanloop-0.4.4/humanloop/model/config_type.pyi
+-rw-r--r--   0        0        0     6196 2023-05-26 00:09:33.384928 humanloop-0.4.4/humanloop/model/create_experiment_request.py
+-rw-r--r--   0        0        0     6196 2023-05-26 00:09:33.385040 humanloop-0.4.4/humanloop/model/create_experiment_request.pyi
+-rw-r--r--   0        0        0     3199 2023-05-26 00:09:33.385125 humanloop-0.4.4/humanloop/model/create_log_response.py
+-rw-r--r--   0        0        0     3199 2023-05-26 00:09:33.385216 humanloop-0.4.4/humanloop/model/create_log_response.pyi
+-rw-r--r--   0        0        0     4266 2023-05-26 00:09:33.385300 humanloop-0.4.4/humanloop/model/create_project_request.py
+-rw-r--r--   0        0        0     4266 2023-05-26 00:09:33.385382 humanloop-0.4.4/humanloop/model/create_project_request.pyi
+-rw-r--r--   0        0        0     2635 2023-05-26 00:09:33.385464 humanloop-0.4.4/humanloop/model/create_session_response.py
+-rw-r--r--   0        0        0     2635 2023-05-26 00:09:33.385546 humanloop-0.4.4/humanloop/model/create_session_response.pyi
+-rw-r--r--   0        0        0     3232 2023-05-26 00:09:33.385659 humanloop-0.4.4/humanloop/model/create_trace_request.py
+-rw-r--r--   0        0        0     3232 2023-05-26 00:09:33.385751 humanloop-0.4.4/humanloop/model/create_trace_request.pyi
+-rw-r--r--   0        0        0     3329 2023-05-26 00:09:33.385854 humanloop-0.4.4/humanloop/model/create_trace_response.py
+-rw-r--r--   0        0        0     3329 2023-05-26 00:09:33.385954 humanloop-0.4.4/humanloop/model/create_trace_response.pyi
+-rw-r--r--   0        0        0     7455 2023-05-26 00:09:33.386097 humanloop-0.4.4/humanloop/model/data_response.py
+-rw-r--r--   0        0        0     7455 2023-05-26 00:09:33.386236 humanloop-0.4.4/humanloop/model/data_response.pyi
+-rw-r--r--   0        0        0     8998 2023-05-26 00:09:33.386373 humanloop-0.4.4/humanloop/model/experiment_config_response.py
+-rw-r--r--   0        0        0     8998 2023-05-26 00:09:33.386615 humanloop-0.4.4/humanloop/model/experiment_config_response.pyi
+-rw-r--r--   0        0        0    12827 2023-05-26 00:09:33.386902 humanloop-0.4.4/humanloop/model/experiment_response.py
+-rw-r--r--   0        0        0    12827 2023-05-26 00:09:33.387160 humanloop-0.4.4/humanloop/model/experiment_response.pyi
+-rw-r--r--   0        0        0     1376 2023-05-26 00:09:33.387417 humanloop-0.4.4/humanloop/model/experiment_status.py
+-rw-r--r--   0        0        0     1229 2023-05-26 00:09:33.387620 humanloop-0.4.4/humanloop/model/experiment_status.pyi
+-rw-r--r--   0        0        0     1685 2023-05-26 00:09:33.387813 humanloop-0.4.4/humanloop/model/experiments_list_response.py
+-rw-r--r--   0        0        0     1685 2023-05-26 00:09:33.388027 humanloop-0.4.4/humanloop/model/experiments_list_response.pyi
+-rw-r--r--   0        0        0     6681 2023-05-26 00:09:33.388222 humanloop-0.4.4/humanloop/model/feedback.py
+-rw-r--r--   0        0        0     6681 2023-05-26 00:09:33.388429 humanloop-0.4.4/humanloop/model/feedback.pyi
+-rw-r--r--   0        0        0     1463 2023-05-26 00:09:33.388630 humanloop-0.4.4/humanloop/model/feedback_class.py
+-rw-r--r--   0        0        0     1296 2023-05-26 00:09:33.388826 humanloop-0.4.4/humanloop/model/feedback_class.pyi
+-rw-r--r--   0        0        0     3334 2023-05-26 00:09:33.389017 humanloop-0.4.4/humanloop/model/feedback_label_request.py
+-rw-r--r--   0        0        0     3334 2023-05-26 00:09:33.389230 humanloop-0.4.4/humanloop/model/feedback_label_request.pyi
+-rw-r--r--   0        0        0     7189 2023-05-26 00:09:33.389411 humanloop-0.4.4/humanloop/model/feedback_request.py
+-rw-r--r--   0        0        0     7189 2023-05-26 00:09:33.389571 humanloop-0.4.4/humanloop/model/feedback_request.pyi
+-rw-r--r--   0        0        0     7141 2023-05-26 00:09:33.389747 humanloop-0.4.4/humanloop/model/feedback_response.py
+-rw-r--r--   0        0        0     7141 2023-05-26 00:09:33.390041 humanloop-0.4.4/humanloop/model/feedback_response.pyi
+-rw-r--r--   0        0        0     3200 2023-05-26 00:09:33.390309 humanloop-0.4.4/humanloop/model/feedback_submit_request.py
+-rw-r--r--   0        0        0     3200 2023-05-26 00:09:33.390470 humanloop-0.4.4/humanloop/model/feedback_submit_request.pyi
+-rw-r--r--   0        0        0     3210 2023-05-26 00:09:33.390620 humanloop-0.4.4/humanloop/model/feedback_submit_response.py
+-rw-r--r--   0        0        0     3210 2023-05-26 00:09:33.390801 humanloop-0.4.4/humanloop/model/feedback_submit_response.pyi
+-rw-r--r--   0        0        0     1690 2023-05-26 00:09:33.390957 humanloop-0.4.4/humanloop/model/feedback_type.py
+-rw-r--r--   0        0        0     1459 2023-05-26 00:09:33.391121 humanloop-0.4.4/humanloop/model/feedback_type.pyi
+-rw-r--r--   0        0        0     6161 2023-05-26 00:09:33.391277 humanloop-0.4.4/humanloop/model/feedback_type_model.py
+-rw-r--r--   0        0        0     6161 2023-05-26 00:09:33.391439 humanloop-0.4.4/humanloop/model/feedback_type_model.pyi
+-rw-r--r--   0        0        0     6289 2023-05-26 00:09:33.391592 humanloop-0.4.4/humanloop/model/feedback_type_request.py
+-rw-r--r--   0        0        0     6289 2023-05-26 00:09:33.391728 humanloop-0.4.4/humanloop/model/feedback_type_request.pyi
+-rw-r--r--   0        0        0     1659 2023-05-26 00:09:33.391809 humanloop-0.4.4/humanloop/model/feedback_types.py
+-rw-r--r--   0        0        0     1659 2023-05-26 00:09:33.391891 humanloop-0.4.4/humanloop/model/feedback_types.pyi
+-rw-r--r--   0        0        0     4407 2023-05-26 00:09:33.391974 humanloop-0.4.4/humanloop/model/generic_config_request.py
+-rw-r--r--   0        0        0     4238 2023-05-26 00:09:33.392059 humanloop-0.4.4/humanloop/model/generic_config_request.pyi
+-rw-r--r--   0        0        0     6562 2023-05-26 00:09:33.392142 humanloop-0.4.4/humanloop/model/generic_config_response.py
+-rw-r--r--   0        0        0     6562 2023-05-26 00:09:33.392226 humanloop-0.4.4/humanloop/model/generic_config_response.pyi
+-rw-r--r--   0        0        0     9619 2023-05-26 00:09:33.392316 humanloop-0.4.4/humanloop/model/get_model_config_response.py
+-rw-r--r--   0        0        0     9619 2023-05-26 00:09:33.392442 humanloop-0.4.4/humanloop/model/get_model_config_response.pyi
+-rw-r--r--   0        0        0     3611 2023-05-26 00:09:33.392585 humanloop-0.4.4/humanloop/model/http_validation_error.py
+-rw-r--r--   0        0        0     3611 2023-05-26 00:09:33.392724 humanloop-0.4.4/humanloop/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     1667 2023-05-26 00:09:33.392867 humanloop-0.4.4/humanloop/model/label_sentiment.py
+-rw-r--r--   0        0        0     1468 2023-05-26 00:09:33.393012 humanloop-0.4.4/humanloop/model/label_sentiment.pyi
+-rw-r--r--   0        0        0     3156 2023-05-26 00:09:33.393165 humanloop-0.4.4/humanloop/model/log_datapoint_request.py
+-rw-r--r--   0        0        0     3156 2023-05-26 00:09:33.393315 humanloop-0.4.4/humanloop/model/log_datapoint_request.pyi
+-rw-r--r--   0        0        0    17219 2023-05-26 00:09:33.393566 humanloop-0.4.4/humanloop/model/log_model_config_request.py
+-rw-r--r--   0        0        0    17219 2023-05-26 00:09:33.393871 humanloop-0.4.4/humanloop/model/log_model_config_request.pyi
+-rw-r--r--   0        0        0    15844 2023-05-26 00:09:33.394106 humanloop-0.4.4/humanloop/model/log_request.py
+-rw-r--r--   0        0        0    15844 2023-05-26 00:09:33.394496 humanloop-0.4.4/humanloop/model/log_request.pyi
+-rw-r--r--   0        0        0    20160 2023-05-26 00:09:33.394844 humanloop-0.4.4/humanloop/model/log_response.py
+-rw-r--r--   0        0        0    20160 2023-05-26 00:09:33.395113 humanloop-0.4.4/humanloop/model/log_response.pyi
+-rw-r--r--   0        0        0     3205 2023-05-26 00:09:33.395336 humanloop-0.4.4/humanloop/model/logs_log_response.py
+-rw-r--r--   0        0        0     3205 2023-05-26 00:09:33.395496 humanloop-0.4.4/humanloop/model/logs_log_response.pyi
+-rw-r--r--   0        0        0    16246 2023-05-26 00:09:33.395666 humanloop-0.4.4/humanloop/model/model_config_chat_request.py
+-rw-r--r--   0        0        0    16246 2023-05-26 00:09:33.395878 humanloop-0.4.4/humanloop/model/model_config_chat_request.pyi
+-rw-r--r--   0        0        0    15386 2023-05-26 00:09:33.396090 humanloop-0.4.4/humanloop/model/model_config_completion_request.py
+-rw-r--r--   0        0        0    15386 2023-05-26 00:09:33.396290 humanloop-0.4.4/humanloop/model/model_config_completion_request.pyi
+-rw-r--r--   0        0        0    17859 2023-05-26 00:09:33.396535 humanloop-0.4.4/humanloop/model/model_config_response.py
+-rw-r--r--   0        0        0    17859 2023-05-26 00:09:33.396754 humanloop-0.4.4/humanloop/model/model_config_response.pyi
+-rw-r--r--   0        0        0    20554 2023-05-26 00:09:33.396963 humanloop-0.4.4/humanloop/model/model_config_response2.py
+-rw-r--r--   0        0        0    20554 2023-05-26 00:09:33.397166 humanloop-0.4.4/humanloop/model/model_config_response2.pyi
+-rw-r--r--   0        0        0     1460 2023-05-26 00:09:33.397348 humanloop-0.4.4/humanloop/model/model_endpoints.py
+-rw-r--r--   0        0        0     1305 2023-05-26 00:09:33.397493 humanloop-0.4.4/humanloop/model/model_endpoints.pyi
+-rw-r--r--   0        0        0     1695 2023-05-26 00:09:33.397641 humanloop-0.4.4/humanloop/model/model_providers.py
+-rw-r--r--   0        0        0     1468 2023-05-26 00:09:33.397779 humanloop-0.4.4/humanloop/model/model_providers.pyi
+-rw-r--r--   0        0        0     5144 2023-05-26 00:09:33.397946 humanloop-0.4.4/humanloop/model/paginated_data_log_response.py
+-rw-r--r--   0        0        0     5144 2023-05-26 00:09:33.398153 humanloop-0.4.4/humanloop/model/paginated_data_log_response.pyi
+-rw-r--r--   0        0        0     5180 2023-05-26 00:09:33.398327 humanloop-0.4.4/humanloop/model/paginated_data_project_response.py
+-rw-r--r--   0        0        0     5180 2023-05-26 00:09:33.398475 humanloop-0.4.4/humanloop/model/paginated_data_project_response.pyi
+-rw-r--r--   0        0        0     5180 2023-05-26 00:09:33.398617 humanloop-0.4.4/humanloop/model/paginated_data_session_response.py
+-rw-r--r--   0        0        0     5180 2023-05-26 00:09:33.398802 humanloop-0.4.4/humanloop/model/paginated_data_session_response.pyi
+-rw-r--r--   0        0        0     3143 2023-05-26 00:09:33.398968 humanloop-0.4.4/humanloop/model/positive_label.py
+-rw-r--r--   0        0        0     3143 2023-05-26 00:09:33.399127 humanloop-0.4.4/humanloop/model/positive_label.pyi
+-rw-r--r--   0        0        0     8900 2023-05-26 00:09:33.399307 humanloop-0.4.4/humanloop/model/project_config_response.py
+-rw-r--r--   0        0        0     8900 2023-05-26 00:09:33.399516 humanloop-0.4.4/humanloop/model/project_config_response.pyi
+-rw-r--r--   0        0        0    18363 2023-05-26 00:09:33.399715 humanloop-0.4.4/humanloop/model/project_model_config_request.py
+-rw-r--r--   0        0        0    18363 2023-05-26 00:09:33.399923 humanloop-0.4.4/humanloop/model/project_model_config_request.pyi
+-rw-r--r--   0        0        0    23968 2023-05-26 00:09:33.400111 humanloop-0.4.4/humanloop/model/project_model_config_response.py
+-rw-r--r--   0        0        0    23968 2023-05-26 00:09:33.400242 humanloop-0.4.4/humanloop/model/project_model_config_response.pyi
+-rw-r--r--   0        0        0    13895 2023-05-26 00:09:33.400364 humanloop-0.4.4/humanloop/model/project_response.py
+-rw-r--r--   0        0        0    13895 2023-05-26 00:09:33.400542 humanloop-0.4.4/humanloop/model/project_response.pyi
+-rw-r--r--   0        0        0     1471 2023-05-26 00:09:33.400725 humanloop-0.4.4/humanloop/model/project_sort_by.py
+-rw-r--r--   0        0        0     1300 2023-05-26 00:09:33.400871 humanloop-0.4.4/humanloop/model/project_sort_by.pyi
+-rw-r--r--   0        0        0     3795 2023-05-26 00:09:33.401033 humanloop-0.4.4/humanloop/model/project_user_response.py
+-rw-r--r--   0        0        0     3795 2023-05-26 00:09:33.401194 humanloop-0.4.4/humanloop/model/project_user_response.pyi
+-rw-r--r--   0        0        0     1713 2023-05-26 00:09:33.401332 humanloop-0.4.4/humanloop/model/projects_get_configs_response.py
+-rw-r--r--   0        0        0     1713 2023-05-26 00:09:33.401471 humanloop-0.4.4/humanloop/model/projects_get_configs_response.pyi
+-rw-r--r--   0        0        0     1715 2023-05-26 00:09:33.401609 humanloop-0.4.4/humanloop/model/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0     1715 2023-05-26 00:09:33.401746 humanloop-0.4.4/humanloop/model/projects_update_feedback_types_request.pyi
+-rw-r--r--   0        0        0     4150 2023-05-26 00:09:33.401882 humanloop-0.4.4/humanloop/model/provider_api_keys.py
+-rw-r--r--   0        0        0     4150 2023-05-26 00:09:33.402020 humanloop-0.4.4/humanloop/model/provider_api_keys.pyi
+-rw-r--r--   0        0        0     3113 2023-05-26 00:09:33.402163 humanloop-0.4.4/humanloop/model/session_project_response.py
+-rw-r--r--   0        0        0     3113 2023-05-26 00:09:33.402305 humanloop-0.4.4/humanloop/model/session_project_response.pyi
+-rw-r--r--   0        0        0     6620 2023-05-26 00:09:33.402434 humanloop-0.4.4/humanloop/model/session_response.py
+-rw-r--r--   0        0        0     6620 2023-05-26 00:09:33.402574 humanloop-0.4.4/humanloop/model/session_response.pyi
+-rw-r--r--   0        0        0     1309 2023-05-26 00:09:33.402724 humanloop-0.4.4/humanloop/model/sort_order.py
+-rw-r--r--   0        0        0     1192 2023-05-26 00:09:33.402863 humanloop-0.4.4/humanloop/model/sort_order.pyi
+-rw-r--r--   0        0        0     4889 2023-05-26 00:09:33.403027 humanloop-0.4.4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4889 2023-05-26 00:09:33.403174 humanloop-0.4.4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0     4893 2023-05-26 00:09:33.403321 humanloop-0.4.4/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4893 2023-05-26 00:09:33.403485 humanloop-0.4.4/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0     4951 2023-05-26 00:09:33.403637 humanloop-0.4.4/humanloop/model/tool_config_request.py
+-rw-r--r--   0        0        0     4788 2023-05-26 00:09:33.403769 humanloop-0.4.4/humanloop/model/tool_config_request.pyi
+-rw-r--r--   0        0        0     7064 2023-05-26 00:09:33.403904 humanloop-0.4.4/humanloop/model/tool_config_response.py
+-rw-r--r--   0        0        0     7064 2023-05-26 00:09:33.404112 humanloop-0.4.4/humanloop/model/tool_config_response.pyi
+-rw-r--r--   0        0        0     4232 2023-05-26 00:09:33.404287 humanloop-0.4.4/humanloop/model/tool_result_response.py
+-rw-r--r--   0        0        0     4232 2023-05-26 00:09:33.404431 humanloop-0.4.4/humanloop/model/tool_result_response.pyi
+-rw-r--r--   0        0        0    13080 2023-05-26 00:09:33.404593 humanloop-0.4.4/humanloop/model/trace_log_request.py
+-rw-r--r--   0        0        0    13080 2023-05-26 00:09:33.404822 humanloop-0.4.4/humanloop/model/trace_log_request.pyi
+-rw-r--r--   0        0        0    19510 2023-05-26 00:09:33.405079 humanloop-0.4.4/humanloop/model/trace_model_config_request.py
+-rw-r--r--   0        0        0    19345 2023-05-26 00:09:33.405320 humanloop-0.4.4/humanloop/model/trace_model_config_request.pyi
+-rw-r--r--   0        0        0     7302 2023-05-26 00:09:33.405538 humanloop-0.4.4/humanloop/model/update_experiment_request.py
+-rw-r--r--   0        0        0     7302 2023-05-26 00:09:33.405700 humanloop-0.4.4/humanloop/model/update_experiment_request.pyi
+-rw-r--r--   0        0        0     5047 2023-05-26 00:09:33.405854 humanloop-0.4.4/humanloop/model/update_project_request.py
+-rw-r--r--   0        0        0     5047 2023-05-26 00:09:33.406011 humanloop-0.4.4/humanloop/model/update_project_request.pyi
+-rw-r--r--   0        0        0     4118 2023-05-26 00:09:33.406164 humanloop-0.4.4/humanloop/model/usage.py
+-rw-r--r--   0        0        0     4118 2023-05-26 00:09:33.406326 humanloop-0.4.4/humanloop/model/usage.pyi
+-rw-r--r--   0        0        0     6805 2023-05-26 00:09:33.406468 humanloop-0.4.4/humanloop/model/validation_error.py
+-rw-r--r--   0        0        0     6805 2023-05-26 00:09:33.406614 humanloop-0.4.4/humanloop/model/validation_error.pyi
+-rw-r--r--   0        0        0     6379 2023-05-26 00:09:33.406760 humanloop-0.4.4/humanloop/models/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-26 00:09:33.406910 humanloop-0.4.4/humanloop/paths/__init__.py
+-rw-r--r--   0        0        0      285 2023-05-26 00:09:33.407046 humanloop-0.4.4/humanloop/paths/chat/__init__.py
+-rw-r--r--   0        0        0    17428 2023-05-26 00:09:33.407245 humanloop-0.4.4/humanloop/paths/chat/post.py
+-rw-r--r--   0        0        0    17285 2023-05-26 00:09:33.407480 humanloop-0.4.4/humanloop/paths/chat/post.pyi
+-rw-r--r--   0        0        0      302 2023-05-26 00:09:33.407684 humanloop-0.4.4/humanloop/paths/chat_deployed/__init__.py
+-rw-r--r--   0        0        0    16991 2023-05-26 00:09:33.408384 humanloop-0.4.4/humanloop/paths/chat_deployed/post.py
+-rw-r--r--   0        0        0    16848 2023-05-26 00:09:33.408725 humanloop-0.4.4/humanloop/paths/chat_deployed/post.pyi
+-rw-r--r--   0        0        0      306 2023-05-26 00:09:33.408939 humanloop-0.4.4/humanloop/paths/chat_experiment/__init__.py
+-rw-r--r--   0        0        0    17434 2023-05-26 00:09:33.409140 humanloop-0.4.4/humanloop/paths/chat_experiment/post.py
+-rw-r--r--   0        0        0    17291 2023-05-26 00:09:33.409361 humanloop-0.4.4/humanloop/paths/chat_experiment/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-26 00:09:33.409537 humanloop-0.4.4/humanloop/paths/chat_model_config/__init__.py
+-rw-r--r--   0        0        0    17609 2023-05-26 00:09:33.409718 humanloop-0.4.4/humanloop/paths/chat_model_config/post.py
+-rw-r--r--   0        0        0    17466 2023-05-26 00:09:33.409984 humanloop-0.4.4/humanloop/paths/chat_model_config/post.pyi
+-rw-r--r--   0        0        0      297 2023-05-26 00:09:33.410169 humanloop-0.4.4/humanloop/paths/completion/__init__.py
+-rw-r--r--   0        0        0    17744 2023-05-26 00:09:33.410338 humanloop-0.4.4/humanloop/paths/completion/post.py
+-rw-r--r--   0        0        0    17601 2023-05-26 00:09:33.410486 humanloop-0.4.4/humanloop/paths/completion/post.pyi
+-rw-r--r--   0        0        0      314 2023-05-26 00:09:33.410662 humanloop-0.4.4/humanloop/paths/completion_deployed/__init__.py
+-rw-r--r--   0        0        0    17247 2023-05-26 00:09:33.410830 humanloop-0.4.4/humanloop/paths/completion_deployed/post.py
+-rw-r--r--   0        0        0    17104 2023-05-26 00:09:33.411069 humanloop-0.4.4/humanloop/paths/completion_deployed/post.pyi
+-rw-r--r--   0        0        0      318 2023-05-26 00:09:33.411316 humanloop-0.4.4/humanloop/paths/completion_experiment/__init__.py
+-rw-r--r--   0        0        0    17690 2023-05-26 00:09:33.411495 humanloop-0.4.4/humanloop/paths/completion_experiment/post.py
+-rw-r--r--   0        0        0    17547 2023-05-26 00:09:33.411728 humanloop-0.4.4/humanloop/paths/completion_experiment/post.pyi
+-rw-r--r--   0        0        0      321 2023-05-26 00:09:33.411961 humanloop-0.4.4/humanloop/paths/completion_model_config/__init__.py
+-rw-r--r--   0        0        0    17865 2023-05-26 00:09:33.412136 humanloop-0.4.4/humanloop/paths/completion_model_config/post.py
+-rw-r--r--   0        0        0    17722 2023-05-26 00:09:33.412367 humanloop-0.4.4/humanloop/paths/completion_model_config/post.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 00:09:33.412566 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/__init__.py
+-rw-r--r--   0        0        0    11995 2023-05-26 00:09:33.412728 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/delete.py
+-rw-r--r--   0        0        0    11852 2023-05-26 00:09:33.412933 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/delete.pyi
+-rw-r--r--   0        0        0    17043 2023-05-26 00:09:33.413163 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/patch.py
+-rw-r--r--   0        0        0    16900 2023-05-26 00:09:33.413376 humanloop-0.4.4/humanloop/paths/experiments_experiment_id/patch.pyi
+-rw-r--r--   0        0        0      352 2023-05-26 00:09:33.413607 humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/__init__.py
+-rw-r--r--   0        0        0    12496 2023-05-26 00:09:33.413778 humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/get.py
+-rw-r--r--   0        0        0    12353 2023-05-26 00:09:33.414188 humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-26 00:09:33.414383 humanloop-0.4.4/humanloop/paths/feedback/__init__.py
+-rw-r--r--   0        0        0    15089 2023-05-26 00:09:33.414553 humanloop-0.4.4/humanloop/paths/feedback/post.py
+-rw-r--r--   0        0        0    14946 2023-05-26 00:09:33.414768 humanloop-0.4.4/humanloop/paths/feedback/post.pyi
+-rw-r--r--   0        0        0      285 2023-05-26 00:09:33.414989 humanloop-0.4.4/humanloop/paths/logs/__init__.py
+-rw-r--r--   0        0        0    20891 2023-05-26 00:09:33.415195 humanloop-0.4.4/humanloop/paths/logs/post.py
+-rw-r--r--   0        0        0    20748 2023-05-26 00:09:33.415420 humanloop-0.4.4/humanloop/paths/logs/post.pyi
+-rw-r--r--   0        0        0      302 2023-05-26 00:09:33.415614 humanloop-0.4.4/humanloop/paths/model_configs/__init__.py
+-rw-r--r--   0        0        0    20266 2023-05-26 00:09:33.415801 humanloop-0.4.4/humanloop/paths/model_configs/post.py
+-rw-r--r--   0        0        0    20123 2023-05-26 00:09:33.416037 humanloop-0.4.4/humanloop/paths/model_configs/post.pyi
+-rw-r--r--   0        0        0      308 2023-05-26 00:09:33.416239 humanloop-0.4.4/humanloop/paths/model_configs_id/__init__.py
+-rw-r--r--   0        0        0    12023 2023-05-26 00:09:33.416409 humanloop-0.4.4/humanloop/paths/model_configs_id/get.py
+-rw-r--r--   0        0        0    11880 2023-05-26 00:09:33.416832 humanloop-0.4.4/humanloop/paths/model_configs_id/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-26 00:09:33.417031 humanloop-0.4.4/humanloop/paths/projects/__init__.py
+-rw-r--r--   0        0        0    20518 2023-05-26 00:09:33.417222 humanloop-0.4.4/humanloop/paths/projects/get.py
+-rw-r--r--   0        0        0    20375 2023-05-26 00:09:33.417418 humanloop-0.4.4/humanloop/paths/projects/get.pyi
+-rw-r--r--   0        0        0    13007 2023-05-26 00:09:33.417605 humanloop-0.4.4/humanloop/paths/projects/post.py
+-rw-r--r--   0        0        0    12864 2023-05-26 00:09:33.417827 humanloop-0.4.4/humanloop/paths/projects/post.pyi
+-rw-r--r--   0        0        0      299 2023-05-26 00:09:33.418042 humanloop-0.4.4/humanloop/paths/projects_id/__init__.py
+-rw-r--r--   0        0        0    11979 2023-05-26 00:09:33.418232 humanloop-0.4.4/humanloop/paths/projects_id/get.py
+-rw-r--r--   0        0        0    11836 2023-05-26 00:09:33.418471 humanloop-0.4.4/humanloop/paths/projects_id/get.pyi
+-rw-r--r--   0        0        0    16066 2023-05-26 00:09:33.418722 humanloop-0.4.4/humanloop/paths/projects_id/patch.py
+-rw-r--r--   0        0        0    15923 2023-05-26 00:09:33.418969 humanloop-0.4.4/humanloop/paths/projects_id/patch.pyi
+-rw-r--r--   0        0        0      326 2023-05-26 00:09:33.419195 humanloop-0.4.4/humanloop/paths/projects_id_active_config/__init__.py
+-rw-r--r--   0        0        0    12298 2023-05-26 00:09:33.419382 humanloop-0.4.4/humanloop/paths/projects_id_active_config/delete.py
+-rw-r--r--   0        0        0    12155 2023-05-26 00:09:33.419618 humanloop-0.4.4/humanloop/paths/projects_id_active_config/delete.pyi
+-rw-r--r--   0        0        0    12148 2023-05-26 00:09:33.419838 humanloop-0.4.4/humanloop/paths/projects_id_active_config/get.py
+-rw-r--r--   0        0        0    12005 2023-05-26 00:09:33.420056 humanloop-0.4.4/humanloop/paths/projects_id_active_config/get.pyi
+-rw-r--r--   0        0        0      334 2023-05-26 00:09:33.420251 humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/__init__.py
+-rw-r--r--   0        0        0    12306 2023-05-26 00:09:33.420447 humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/delete.py
+-rw-r--r--   0        0        0    12163 2023-05-26 00:09:33.420684 humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/delete.pyi
+-rw-r--r--   0        0        0      315 2023-05-26 00:09:33.420881 humanloop-0.4.4/humanloop/paths/projects_id_configs/__init__.py
+-rw-r--r--   0        0        0    12182 2023-05-26 00:09:33.421060 humanloop-0.4.4/humanloop/paths/projects_id_configs/get.py
+-rw-r--r--   0        0        0    12039 2023-05-26 00:09:33.421323 humanloop-0.4.4/humanloop/paths/projects_id_configs/get.pyi
+-rw-r--r--   0        0        0      313 2023-05-26 00:09:33.421557 humanloop-0.4.4/humanloop/paths/projects_id_export/__init__.py
+-rw-r--r--   0        0        0    15728 2023-05-26 00:09:33.421736 humanloop-0.4.4/humanloop/paths/projects_id_export/post.py
+-rw-r--r--   0        0        0    15585 2023-05-26 00:09:33.421996 humanloop-0.4.4/humanloop/paths/projects_id_export/post.pyi
+-rw-r--r--   0        0        0      328 2023-05-26 00:09:33.422193 humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/__init__.py
+-rw-r--r--   0        0        0    14798 2023-05-26 00:09:33.422375 humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/patch.py
+-rw-r--r--   0        0        0    14655 2023-05-26 00:09:33.422581 humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/patch.pyi
+-rw-r--r--   0        0        0      339 2023-05-26 00:09:33.422766 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/__init__.py
+-rw-r--r--   0        0        0    12256 2023-05-26 00:09:33.422935 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/get.py
+-rw-r--r--   0        0        0    12113 2023-05-26 00:09:33.423152 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/get.pyi
+-rw-r--r--   0        0        0    16250 2023-05-26 00:09:33.423350 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/post.py
+-rw-r--r--   0        0        0    16107 2023-05-26 00:09:33.423545 humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/post.pyi
+-rw-r--r--   0        0        0      293 2023-05-26 00:09:33.423731 humanloop-0.4.4/humanloop/paths/sessions/__init__.py
+-rw-r--r--   0        0        0    14112 2023-05-26 00:09:33.423900 humanloop-0.4.4/humanloop/paths/sessions/get.py
+-rw-r--r--   0        0        0    13969 2023-05-26 00:09:33.424115 humanloop-0.4.4/humanloop/paths/sessions/get.pyi
+-rw-r--r--   0        0        0     9192 2023-05-26 00:09:33.424327 humanloop-0.4.4/humanloop/paths/sessions/post.py
+-rw-r--r--   0        0        0     9079 2023-05-26 00:09:33.424529 humanloop-0.4.4/humanloop/paths/sessions/post.pyi
+-rw-r--r--   0        0        0      299 2023-05-26 00:09:33.424687 humanloop-0.4.4/humanloop/paths/sessions_id/__init__.py
+-rw-r--r--   0        0        0    11979 2023-05-26 00:09:33.424816 humanloop-0.4.4/humanloop/paths/sessions_id/get.py
+-rw-r--r--   0        0        0    11836 2023-05-26 00:09:33.424933 humanloop-0.4.4/humanloop/paths/sessions_id/get.pyi
+-rw-r--r--   0        0        0      289 2023-05-26 00:09:33.425044 humanloop-0.4.4/humanloop/paths/traces/__init__.py
+-rw-r--r--   0        0        0    12450 2023-05-26 00:09:33.425152 humanloop-0.4.4/humanloop/paths/traces/post.py
+-rw-r--r--   0        0        0    12307 2023-05-26 00:09:33.425308 humanloop-0.4.4/humanloop/paths/traces/post.pyi
+-rw-r--r--   0        0        0     1011 2023-05-26 00:09:33.425521 humanloop-0.4.4/humanloop/request_after_hook.py
+-rw-r--r--   0        0        0     1783 2023-05-26 00:09:33.461649 humanloop-0.4.4/humanloop/request_before_hook.py
+-rw-r--r--   0        0        0    11329 2023-05-26 00:09:33.425845 humanloop-0.4.4/humanloop/rest.py
+-rw-r--r--   0        0        0    95913 2023-05-26 00:09:33.426216 humanloop-0.4.4/humanloop/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-26 00:09:33.426384 humanloop-0.4.4/humanloop/type/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-26 00:09:33.426580 humanloop-0.4.4/humanloop/type/agent_config_request.py
+-rw-r--r--   0        0        0     1608 2023-05-26 00:09:33.426720 humanloop-0.4.4/humanloop/type/agent_config_response.py
+-rw-r--r--   0        0        0     1408 2023-05-26 00:09:33.426864 humanloop-0.4.4/humanloop/type/base_metric_response.py
+-rw-r--r--   0        0        0     1062 2023-05-26 00:09:33.427008 humanloop-0.4.4/humanloop/type/categorical_feedback_label.py
+-rw-r--r--   0        0        0     2183 2023-05-26 00:09:33.427149 humanloop-0.4.4/humanloop/type/chat_data_response.py
+-rw-r--r--   0        0        0     1990 2023-05-26 00:09:33.427304 humanloop-0.4.4/humanloop/type/chat_deployed_request.py
+-rw-r--r--   0        0        0     2235 2023-05-26 00:09:33.427453 humanloop-0.4.4/humanloop/type/chat_experiment_request.py
+-rw-r--r--   0        0        0      919 2023-05-26 00:09:33.427608 humanloop-0.4.4/humanloop/type/chat_message.py
+-rw-r--r--   0        0        0     2104 2023-05-26 00:09:33.427759 humanloop-0.4.4/humanloop/type/chat_model_config_request.py
+-rw-r--r--   0        0        0     2130 2023-05-26 00:09:33.427911 humanloop-0.4.4/humanloop/type/chat_request.py
+-rw-r--r--   0        0        0     1818 2023-05-26 00:09:33.428071 humanloop-0.4.4/humanloop/type/chat_response.py
+-rw-r--r--   0        0        0      711 2023-05-26 00:09:33.428224 humanloop-0.4.4/humanloop/type/chat_role.py
+-rw-r--r--   0        0        0     2095 2023-05-26 00:09:33.428413 humanloop-0.4.4/humanloop/type/completion_deployed_request.py
+-rw-r--r--   0        0        0     2343 2023-05-26 00:09:33.428576 humanloop-0.4.4/humanloop/type/completion_experiment_request.py
+-rw-r--r--   0        0        0     2209 2023-05-26 00:09:33.428729 humanloop-0.4.4/humanloop/type/completion_model_config_request.py
+-rw-r--r--   0        0        0     2239 2023-05-26 00:09:33.428905 humanloop-0.4.4/humanloop/type/completion_request.py
+-rw-r--r--   0        0        0     1864 2023-05-26 00:09:33.429066 humanloop-0.4.4/humanloop/type/completion_response.py
+-rw-r--r--   0        0        0     1054 2023-05-26 00:09:33.429226 humanloop-0.4.4/humanloop/type/config_response.py
+-rw-r--r--   0        0        0      719 2023-05-26 00:09:33.429407 humanloop-0.4.4/humanloop/type/config_type.py
+-rw-r--r--   0        0        0     1362 2023-05-26 00:09:33.429552 humanloop-0.4.4/humanloop/type/create_experiment_request.py
+-rw-r--r--   0        0        0     1024 2023-05-26 00:09:33.429724 humanloop-0.4.4/humanloop/type/create_log_response.py
+-rw-r--r--   0        0        0     1066 2023-05-26 00:09:33.429874 humanloop-0.4.4/humanloop/type/create_project_request.py
+-rw-r--r--   0        0        0      942 2023-05-26 00:09:33.430013 humanloop-0.4.4/humanloop/type/create_session_response.py
+-rw-r--r--   0        0        0     1045 2023-05-26 00:09:33.430181 humanloop-0.4.4/humanloop/type/create_trace_request.py
+-rw-r--r--   0        0        0      998 2023-05-26 00:09:33.430340 humanloop-0.4.4/humanloop/type/create_trace_response.py
+-rw-r--r--   0        0        0     2013 2023-05-26 00:09:33.430502 humanloop-0.4.4/humanloop/type/data_response.py
+-rw-r--r--   0        0        0     1677 2023-05-26 00:09:33.430838 humanloop-0.4.4/humanloop/type/experiment_config_response.py
+-rw-r--r--   0        0        0     1788 2023-05-26 00:09:33.431062 humanloop-0.4.4/humanloop/type/experiment_response.py
+-rw-r--r--   0        0        0      718 2023-05-26 00:09:33.431306 humanloop-0.4.4/humanloop/type/experiment_status.py
+-rw-r--r--   0        0        0      785 2023-05-26 00:09:33.431545 humanloop-0.4.4/humanloop/type/experiments_list_response.py
+-rw-r--r--   0        0        0     1449 2023-05-26 00:09:33.431838 humanloop-0.4.4/humanloop/type/feedback.py
+-rw-r--r--   0        0        0      719 2023-05-26 00:09:33.432126 humanloop-0.4.4/humanloop/type/feedback_class.py
+-rw-r--r--   0        0        0      970 2023-05-26 00:09:33.432425 humanloop-0.4.4/humanloop/type/feedback_label_request.py
+-rw-r--r--   0        0        0     1546 2023-05-26 00:09:33.432656 humanloop-0.4.4/humanloop/type/feedback_request.py
+-rw-r--r--   0        0        0     1578 2023-05-26 00:09:33.432901 humanloop-0.4.4/humanloop/type/feedback_response.py
+-rw-r--r--   0        0        0      804 2023-05-26 00:09:33.433105 humanloop-0.4.4/humanloop/type/feedback_submit_request.py
+-rw-r--r--   0        0        0      809 2023-05-26 00:09:33.433304 humanloop-0.4.4/humanloop/type/feedback_submit_response.py
+-rw-r--r--   0        0        0      738 2023-05-26 00:09:33.433734 humanloop-0.4.4/humanloop/type/feedback_type.py
+-rw-r--r--   0        0        0     1307 2023-05-26 00:09:33.434005 humanloop-0.4.4/humanloop/type/feedback_type_model.py
+-rw-r--r--   0        0        0     1541 2023-05-26 00:09:33.434262 humanloop-0.4.4/humanloop/type/feedback_type_request.py
+-rw-r--r--   0        0        0      773 2023-05-26 00:09:33.434743 humanloop-0.4.4/humanloop/type/feedback_types.py
+-rw-r--r--   0        0        0     1064 2023-05-26 00:09:33.435026 humanloop-0.4.4/humanloop/type/generic_config_request.py
+-rw-r--r--   0        0        0     1262 2023-05-26 00:09:33.435250 humanloop-0.4.4/humanloop/type/generic_config_response.py
+-rw-r--r--   0        0        0     1900 2023-05-26 00:09:33.435468 humanloop-0.4.4/humanloop/type/get_model_config_response.py
+-rw-r--r--   0        0        0      972 2023-05-26 00:09:33.435661 humanloop-0.4.4/humanloop/type/http_validation_error.py
+-rw-r--r--   0        0        0      730 2023-05-26 00:09:33.435872 humanloop-0.4.4/humanloop/type/label_sentiment.py
+-rw-r--r--   0        0        0      782 2023-05-26 00:09:33.436098 humanloop-0.4.4/humanloop/type/log_datapoint_request.py
+-rw-r--r--   0        0        0     3033 2023-05-26 00:09:33.436346 humanloop-0.4.4/humanloop/type/log_model_config_request.py
+-rw-r--r--   0        0        0     2652 2023-05-26 00:09:33.436549 humanloop-0.4.4/humanloop/type/log_request.py
+-rw-r--r--   0        0        0     2961 2023-05-26 00:09:33.436748 humanloop-0.4.4/humanloop/type/log_response.py
+-rw-r--r--   0        0        0      807 2023-05-26 00:09:33.436938 humanloop-0.4.4/humanloop/type/logs_log_response.py
+-rw-r--r--   0        0        0     2820 2023-05-26 00:09:33.437190 humanloop-0.4.4/humanloop/type/model_config_chat_request.py
+-rw-r--r--   0        0        0     2713 2023-05-26 00:09:33.437424 humanloop-0.4.4/humanloop/type/model_config_completion_request.py
+-rw-r--r--   0        0        0     3160 2023-05-26 00:09:33.437692 humanloop-0.4.4/humanloop/type/model_config_response.py
+-rw-r--r--   0        0        0     3281 2023-05-26 00:09:33.438021 humanloop-0.4.4/humanloop/type/model_config_response2.py
+-rw-r--r--   0        0        0      714 2023-05-26 00:09:33.438400 humanloop-0.4.4/humanloop/type/model_endpoints.py
+-rw-r--r--   0        0        0      738 2023-05-26 00:09:33.438780 humanloop-0.4.4/humanloop/type/model_providers.py
+-rw-r--r--   0        0        0     1032 2023-05-26 00:09:33.439012 humanloop-0.4.4/humanloop/type/paginated_data_log_response.py
+-rw-r--r--   0        0        0     1064 2023-05-26 00:09:33.439156 humanloop-0.4.4/humanloop/type/paginated_data_project_response.py
+-rw-r--r--   0        0        0     1064 2023-05-26 00:09:33.439314 humanloop-0.4.4/humanloop/type/paginated_data_session_response.py
+-rw-r--r--   0        0        0      871 2023-05-26 00:09:33.439484 humanloop-0.4.4/humanloop/type/positive_label.py
+-rw-r--r--   0        0        0     1820 2023-05-26 00:09:33.439701 humanloop-0.4.4/humanloop/type/project_config_response.py
+-rw-r--r--   0        0        0     3410 2023-05-26 00:09:33.439904 humanloop-0.4.4/humanloop/type/project_model_config_request.py
+-rw-r--r--   0        0        0     4053 2023-05-26 00:09:33.440080 humanloop-0.4.4/humanloop/type/project_model_config_response.py
+-rw-r--r--   0        0        0     2032 2023-05-26 00:09:33.440251 humanloop-0.4.4/humanloop/type/project_response.py
+-rw-r--r--   0        0        0      721 2023-05-26 00:09:33.440413 humanloop-0.4.4/humanloop/type/project_sort_by.py
+-rw-r--r--   0        0        0     1022 2023-05-26 00:09:33.440572 humanloop-0.4.4/humanloop/type/project_user_response.py
+-rw-r--r--   0        0        0      798 2023-05-26 00:09:33.440762 humanloop-0.4.4/humanloop/type/projects_get_configs_response.py
+-rw-r--r--   0        0        0      800 2023-05-26 00:09:33.440947 humanloop-0.4.4/humanloop/type/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0      917 2023-05-26 00:09:33.441099 humanloop-0.4.4/humanloop/type/provider_api_keys.py
+-rw-r--r--   0        0        0      985 2023-05-26 00:09:33.441384 humanloop-0.4.4/humanloop/type/session_project_response.py
+-rw-r--r--   0        0        0     1442 2023-05-26 00:09:33.442041 humanloop-0.4.4/humanloop/type/session_response.py
+-rw-r--r--   0        0        0      696 2023-05-26 00:09:33.442226 humanloop-0.4.4/humanloop/type/sort_order.py
+-rw-r--r--   0        0        0     1241 2023-05-26 00:09:33.442401 humanloop-0.4.4/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     1251 2023-05-26 00:09:33.442587 humanloop-0.4.4/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     1066 2023-05-26 00:09:33.442780 humanloop-0.4.4/humanloop/type/tool_config_request.py
+-rw-r--r--   0        0        0     1295 2023-05-26 00:09:33.442940 humanloop-0.4.4/humanloop/type/tool_config_response.py
+-rw-r--r--   0        0        0      930 2023-05-26 00:09:33.443088 humanloop-0.4.4/humanloop/type/tool_result_response.py
+-rw-r--r--   0        0        0     2427 2023-05-26 00:09:33.443226 humanloop-0.4.4/humanloop/type/trace_log_request.py
+-rw-r--r--   0        0        0     3095 2023-05-26 00:09:33.443373 humanloop-0.4.4/humanloop/type/trace_model_config_request.py
+-rw-r--r--   0        0        0     1361 2023-05-26 00:09:33.443521 humanloop-0.4.4/humanloop/type/update_experiment_request.py
+-rw-r--r--   0        0        0     1434 2023-05-26 00:09:33.443664 humanloop-0.4.4/humanloop/type/update_project_request.py
+-rw-r--r--   0        0        0     1042 2023-05-26 00:09:33.443809 humanloop-0.4.4/humanloop/type/usage.py
+-rw-r--r--   0        0        0      951 2023-05-26 00:09:33.443976 humanloop-0.4.4/humanloop/type/validation_error.py
+-rw-r--r--   0        0        0      868 2023-05-26 00:09:33.444124 humanloop-0.4.4/humanloop/type_util.py
+-rw-r--r--   0        0        0     3165 2023-05-26 00:09:33.444298 humanloop-0.4.4/humanloop/validation_metadata.py
+-rw-r--r--   0        0        0      714 2023-05-26 00:09:33.444959 humanloop-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     9366 1970-01-01 00:00:00.000000 humanloop-0.4.4/PKG-INFO
```

### Comparing `humanloop-0.4.3/LICENSE` & `humanloop-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/README.md` & `humanloop-0.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# humanloop@0.4.3
+# humanloop@0.4.4
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.3
+pip install humanloop==0.4.4
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
```

### Comparing `humanloop-0.4.3/humanloop/__init__.py` & `humanloop-0.4.4/humanloop/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 # import ApiClient
 from humanloop.api_client import ApiClient
 
 # import Configuration
 from humanloop.configuration import Configuration
```

### Comparing `humanloop-0.4.3/humanloop/api_client.py` & `humanloop-0.4.4/humanloop/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2759,15 +2759,15 @@
 0000ac60: 6164 6572 5f6e 616d 655d 203d 2068 6561  ader_name] = hea
 0000ac70: 6465 725f 7661 6c75 650a 2020 2020 2020  der_value.      
 0000ac80: 2020 7365 6c66 2e63 6f6f 6b69 6520 3d20    self.cookie = 
 0000ac90: 636f 6f6b 6965 0a20 2020 2020 2020 2023  cookie.        #
 0000aca0: 2053 6574 2064 6566 6175 6c74 2055 7365   Set default Use
 0000acb0: 722d 4167 656e 742e 0a20 2020 2020 2020  r-Agent..       
 0000acc0: 2073 656c 662e 7573 6572 5f61 6765 6e74   self.user_agent
-0000acd0: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e33   = 'Konfig/0.4.3
+0000acd0: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e34   = 'Konfig/0.4.4
 0000ace0: 2f70 7974 686f 6e27 0a0a 2020 2020 6465  /python'..    de
 0000acf0: 6620 5f5f 656e 7465 725f 5f28 7365 6c66  f __enter__(self
 0000ad00: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
 0000ad10: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
 0000ad20: 5f5f 6578 6974 5f5f 2873 656c 662c 2065  __exit__(self, e
 0000ad30: 7863 5f74 7970 652c 2065 7863 5f76 616c  xc_type, exc_val
 0000ad40: 7565 2c20 7472 6163 6562 6163 6b29 3a0a  ue, traceback):.
```

### Comparing `humanloop-0.4.3/humanloop/api_response.py` & `humanloop-0.4.4/humanloop/api_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/path_to_api.py` & `humanloop-0.4.4/humanloop/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tag_to_api.py` & `humanloop-0.4.4/humanloop/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/__init__.py` & `humanloop-0.4.4/humanloop/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/chats_api.py` & `humanloop-0.4.4/humanloop/apis/tags/chats_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/completions_api.py` & `humanloop-0.4.4/humanloop/apis/tags/completions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/experiments_api.py` & `humanloop-0.4.4/humanloop/apis/tags/experiments_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/feedback_api.py` & `humanloop-0.4.4/humanloop/apis/tags/feedback_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/logs_api.py` & `humanloop-0.4.4/humanloop/apis/tags/logs_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/model_configurations_api.py` & `humanloop-0.4.4/humanloop/apis/tags/model_configurations_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/projects_api.py` & `humanloop-0.4.4/humanloop/apis/tags/projects_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/sessions_api.py` & `humanloop-0.4.4/humanloop/apis/tags/sessions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/apis/tags/traces_api.py` & `humanloop-0.4.4/humanloop/apis/tags/traces_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/client.py` & `humanloop-0.4.4/humanloop/client.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/client.pyi` & `humanloop-0.4.4/humanloop/client.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/client_custom.py` & `humanloop-0.4.4/humanloop/client_custom.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,25 +35,17 @@
         async for line in generator:
             parsed = _parse_sse_chunk(line)
             if parsed is None:
                 continue
             try:
                 as_json = json.loads(parsed)
 
-                choice = as_json["provider_responses"][0]["choices"][0]
-                if "delta" in choice:
-                    # for /chat
-                    delta = as_json["provider_responses"][0]["choices"][0]["delta"]
-                    if "content" in delta:
-                        yield delta["content"]
-                elif "text" in choice:
-                    # for /completion
-                    yield as_json["provider_responses"][0]["choices"][0]["text"]
-                else:
-                    raise Exception("Unknown response type")
+                output = as_json["data"][0]["output"]
+                id = as_json["data"][0]["id"]
+                yield {"output": output, "id": id}
             except Exception as e:
                 # move on silently
                 pass
 
     @copy_signature(ChatsApi.aresponse)
     async def chat_stream(self, *args, **kwargs):
         kwargs["stream"] = True
```

### Comparing `humanloop-0.4.3/humanloop/configuration.py` & `humanloop-0.4.4/humanloop/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 4.0.0\n"\
-               "SDK Package Version: 0.4.3".\
+               "SDK Package Version: 0.4.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `humanloop-0.4.3/humanloop/exceptions.py` & `humanloop-0.4.4/humanloop/exceptions.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/exceptions_base.py` & `humanloop-0.4.4/humanloop/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/agent_config_request.py` & `humanloop-0.4.4/humanloop/model/agent_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/agent_config_request.pyi` & `humanloop-0.4.4/humanloop/model/agent_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/agent_config_response.py` & `humanloop-0.4.4/humanloop/model/agent_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/agent_config_response.pyi` & `humanloop-0.4.4/humanloop/model/agent_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/base_metric_response.py` & `humanloop-0.4.4/humanloop/model/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/base_metric_response.pyi` & `humanloop-0.4.4/humanloop/model/base_metric_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/categorical_feedback_label.py` & `humanloop-0.4.4/humanloop/model/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/categorical_feedback_label.pyi` & `humanloop-0.4.4/humanloop/model/categorical_feedback_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_data_response.py` & `humanloop-0.4.4/humanloop/model/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_data_response.pyi` & `humanloop-0.4.4/humanloop/model/chat_data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_deployed_request.py` & `humanloop-0.4.4/humanloop/model/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_deployed_request.pyi` & `humanloop-0.4.4/humanloop/model/chat_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_experiment_request.py` & `humanloop-0.4.4/humanloop/model/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_experiment_request.pyi` & `humanloop-0.4.4/humanloop/model/chat_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_message.py` & `humanloop-0.4.4/humanloop/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_message.pyi` & `humanloop-0.4.4/humanloop/model/chat_message.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_model_config_request.py` & `humanloop-0.4.4/humanloop/model/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_model_config_request.pyi` & `humanloop-0.4.4/humanloop/model/chat_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_request.py` & `humanloop-0.4.4/humanloop/model/chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_request.pyi` & `humanloop-0.4.4/humanloop/model/chat_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_response.py` & `humanloop-0.4.4/humanloop/model/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_response.pyi` & `humanloop-0.4.4/humanloop/model/chat_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_role.py` & `humanloop-0.4.4/humanloop/model/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/chat_role.pyi` & `humanloop-0.4.4/humanloop/model/chat_role.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_deployed_request.py` & `humanloop-0.4.4/humanloop/model/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_deployed_request.pyi` & `humanloop-0.4.4/humanloop/model/completion_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_experiment_request.py` & `humanloop-0.4.4/humanloop/model/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_experiment_request.pyi` & `humanloop-0.4.4/humanloop/model/completion_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_model_config_request.py` & `humanloop-0.4.4/humanloop/model/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_model_config_request.pyi` & `humanloop-0.4.4/humanloop/model/completion_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_request.py` & `humanloop-0.4.4/humanloop/model/completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_request.pyi` & `humanloop-0.4.4/humanloop/model/completion_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_response.py` & `humanloop-0.4.4/humanloop/model/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/completion_response.pyi` & `humanloop-0.4.4/humanloop/model/completion_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/config_response.py` & `humanloop-0.4.4/humanloop/model/config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/config_response.pyi` & `humanloop-0.4.4/humanloop/model/config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/config_type.py` & `humanloop-0.4.4/humanloop/model/config_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/config_type.pyi` & `humanloop-0.4.4/humanloop/model/config_type.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_experiment_request.py` & `humanloop-0.4.4/humanloop/model/create_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_experiment_request.pyi` & `humanloop-0.4.4/humanloop/model/create_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_log_response.py` & `humanloop-0.4.4/humanloop/model/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_log_response.pyi` & `humanloop-0.4.4/humanloop/model/create_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_project_request.py` & `humanloop-0.4.4/humanloop/model/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_project_request.pyi` & `humanloop-0.4.4/humanloop/model/create_project_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_session_response.py` & `humanloop-0.4.4/humanloop/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_session_response.pyi` & `humanloop-0.4.4/humanloop/model/create_session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_trace_request.py` & `humanloop-0.4.4/humanloop/model/create_trace_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_trace_request.pyi` & `humanloop-0.4.4/humanloop/model/create_trace_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_trace_response.py` & `humanloop-0.4.4/humanloop/model/create_trace_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/create_trace_response.pyi` & `humanloop-0.4.4/humanloop/model/create_trace_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/data_response.py` & `humanloop-0.4.4/humanloop/model/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/data_response.pyi` & `humanloop-0.4.4/humanloop/model/data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/experiment_config_response.py` & `humanloop-0.4.4/humanloop/model/experiment_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/experiment_config_response.pyi` & `humanloop-0.4.4/humanloop/model/experiment_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/experiment_response.py` & `humanloop-0.4.4/humanloop/model/experiment_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/experiment_response.pyi` & `humanloop-0.4.4/humanloop/model/experiment_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/experiment_status.py` & `humanloop-0.4.4/humanloop/model/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/experiment_status.pyi` & `humanloop-0.4.4/humanloop/model/experiment_status.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/experiments_list_response.py` & `humanloop-0.4.4/humanloop/model/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/experiments_list_response.pyi` & `humanloop-0.4.4/humanloop/model/experiments_list_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback.py` & `humanloop-0.4.4/humanloop/model/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback.pyi` & `humanloop-0.4.4/humanloop/model/feedback.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_class.py` & `humanloop-0.4.4/humanloop/model/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_class.pyi` & `humanloop-0.4.4/humanloop/model/feedback_class.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_label_request.py` & `humanloop-0.4.4/humanloop/model/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_label_request.pyi` & `humanloop-0.4.4/humanloop/model/feedback_label_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_request.py` & `humanloop-0.4.4/humanloop/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_request.pyi` & `humanloop-0.4.4/humanloop/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_response.py` & `humanloop-0.4.4/humanloop/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_response.pyi` & `humanloop-0.4.4/humanloop/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_submit_request.py` & `humanloop-0.4.4/humanloop/model/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_submit_request.pyi` & `humanloop-0.4.4/humanloop/model/feedback_submit_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_submit_response.py` & `humanloop-0.4.4/humanloop/model/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_submit_response.pyi` & `humanloop-0.4.4/humanloop/model/feedback_submit_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_type.py` & `humanloop-0.4.4/humanloop/model/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_type.pyi` & `humanloop-0.4.4/humanloop/model/feedback_type.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_type_model.py` & `humanloop-0.4.4/humanloop/model/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_type_model.pyi` & `humanloop-0.4.4/humanloop/model/feedback_type_model.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_type_request.py` & `humanloop-0.4.4/humanloop/model/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_type_request.pyi` & `humanloop-0.4.4/humanloop/model/feedback_type_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_types.py` & `humanloop-0.4.4/humanloop/model/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/feedback_types.pyi` & `humanloop-0.4.4/humanloop/model/feedback_types.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/generic_config_request.py` & `humanloop-0.4.4/humanloop/model/generic_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/generic_config_request.pyi` & `humanloop-0.4.4/humanloop/model/generic_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/generic_config_response.py` & `humanloop-0.4.4/humanloop/model/generic_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/generic_config_response.pyi` & `humanloop-0.4.4/humanloop/model/generic_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/get_model_config_response.py` & `humanloop-0.4.4/humanloop/model/get_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/get_model_config_response.pyi` & `humanloop-0.4.4/humanloop/model/get_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/http_validation_error.py` & `humanloop-0.4.4/humanloop/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/http_validation_error.pyi` & `humanloop-0.4.4/humanloop/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/label_sentiment.py` & `humanloop-0.4.4/humanloop/model/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/label_sentiment.pyi` & `humanloop-0.4.4/humanloop/model/label_sentiment.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/log_datapoint_request.py` & `humanloop-0.4.4/humanloop/model/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/log_datapoint_request.pyi` & `humanloop-0.4.4/humanloop/model/log_datapoint_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/log_model_config_request.py` & `humanloop-0.4.4/humanloop/model/log_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/log_model_config_request.pyi` & `humanloop-0.4.4/humanloop/model/log_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/log_request.py` & `humanloop-0.4.4/humanloop/model/log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/log_request.pyi` & `humanloop-0.4.4/humanloop/model/log_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/log_response.py` & `humanloop-0.4.4/humanloop/model/log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/log_response.pyi` & `humanloop-0.4.4/humanloop/model/log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/logs_log_response.py` & `humanloop-0.4.4/humanloop/model/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/logs_log_response.pyi` & `humanloop-0.4.4/humanloop/model/logs_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_config_chat_request.py` & `humanloop-0.4.4/humanloop/model/model_config_chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_config_chat_request.pyi` & `humanloop-0.4.4/humanloop/model/model_config_chat_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_config_completion_request.py` & `humanloop-0.4.4/humanloop/model/model_config_completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_config_completion_request.pyi` & `humanloop-0.4.4/humanloop/model/model_config_completion_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_config_response.py` & `humanloop-0.4.4/humanloop/model/model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_config_response.pyi` & `humanloop-0.4.4/humanloop/model/model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_config_response2.py` & `humanloop-0.4.4/humanloop/model/model_config_response2.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_config_response2.pyi` & `humanloop-0.4.4/humanloop/model/model_config_response2.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_endpoints.py` & `humanloop-0.4.4/humanloop/model/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_endpoints.pyi` & `humanloop-0.4.4/humanloop/model/model_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_providers.py` & `humanloop-0.4.4/humanloop/model/model_providers.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/model_providers.pyi` & `humanloop-0.4.4/humanloop/model/model_providers.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/paginated_data_log_response.py` & `humanloop-0.4.4/humanloop/model/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/paginated_data_log_response.pyi` & `humanloop-0.4.4/humanloop/model/paginated_data_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/paginated_data_project_response.py` & `humanloop-0.4.4/humanloop/model/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/paginated_data_project_response.pyi` & `humanloop-0.4.4/humanloop/model/paginated_data_project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/paginated_data_session_response.py` & `humanloop-0.4.4/humanloop/model/paginated_data_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/paginated_data_session_response.pyi` & `humanloop-0.4.4/humanloop/model/paginated_data_session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/positive_label.py` & `humanloop-0.4.4/humanloop/model/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/positive_label.pyi` & `humanloop-0.4.4/humanloop/model/positive_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_config_response.py` & `humanloop-0.4.4/humanloop/model/project_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_config_response.pyi` & `humanloop-0.4.4/humanloop/model/project_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_model_config_request.py` & `humanloop-0.4.4/humanloop/model/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_model_config_request.pyi` & `humanloop-0.4.4/humanloop/model/project_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_model_config_response.py` & `humanloop-0.4.4/humanloop/model/project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_model_config_response.pyi` & `humanloop-0.4.4/humanloop/model/project_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_response.py` & `humanloop-0.4.4/humanloop/model/project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_response.pyi` & `humanloop-0.4.4/humanloop/model/project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_sort_by.py` & `humanloop-0.4.4/humanloop/model/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_sort_by.pyi` & `humanloop-0.4.4/humanloop/model/project_sort_by.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_user_response.py` & `humanloop-0.4.4/humanloop/model/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/project_user_response.pyi` & `humanloop-0.4.4/humanloop/model/project_user_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/projects_get_configs_response.py` & `humanloop-0.4.4/humanloop/model/projects_get_configs_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/projects_get_configs_response.pyi` & `humanloop-0.4.4/humanloop/model/projects_get_configs_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/projects_update_feedback_types_request.py` & `humanloop-0.4.4/humanloop/model/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/projects_update_feedback_types_request.pyi` & `humanloop-0.4.4/humanloop/model/projects_update_feedback_types_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/provider_api_keys.py` & `humanloop-0.4.4/humanloop/model/provider_api_keys.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/provider_api_keys.pyi` & `humanloop-0.4.4/humanloop/model/provider_api_keys.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/session_project_response.py` & `humanloop-0.4.4/humanloop/model/session_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/session_project_response.pyi` & `humanloop-0.4.4/humanloop/model/session_project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/session_response.py` & `humanloop-0.4.4/humanloop/model/session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/session_response.pyi` & `humanloop-0.4.4/humanloop/model/session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/sort_order.py` & `humanloop-0.4.4/humanloop/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/sort_order.pyi` & `humanloop-0.4.4/humanloop/model/sort_order.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.4/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.4/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/tool_config_request.py` & `humanloop-0.4.4/humanloop/model/tool_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/tool_config_request.pyi` & `humanloop-0.4.4/humanloop/model/tool_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/tool_config_response.py` & `humanloop-0.4.4/humanloop/model/tool_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/tool_config_response.pyi` & `humanloop-0.4.4/humanloop/model/tool_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/tool_result_response.py` & `humanloop-0.4.4/humanloop/model/tool_result_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/tool_result_response.pyi` & `humanloop-0.4.4/humanloop/model/tool_result_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/trace_log_request.py` & `humanloop-0.4.4/humanloop/model/trace_log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/trace_log_request.pyi` & `humanloop-0.4.4/humanloop/model/trace_log_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/trace_model_config_request.py` & `humanloop-0.4.4/humanloop/model/trace_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/trace_model_config_request.pyi` & `humanloop-0.4.4/humanloop/model/trace_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/update_experiment_request.py` & `humanloop-0.4.4/humanloop/model/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/update_experiment_request.pyi` & `humanloop-0.4.4/humanloop/model/update_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/update_project_request.py` & `humanloop-0.4.4/humanloop/model/update_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/update_project_request.pyi` & `humanloop-0.4.4/humanloop/model/update_project_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/usage.py` & `humanloop-0.4.4/humanloop/model/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/usage.pyi` & `humanloop-0.4.4/humanloop/model/usage.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/validation_error.py` & `humanloop-0.4.4/humanloop/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/model/validation_error.pyi` & `humanloop-0.4.4/humanloop/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/models/__init__.py` & `humanloop-0.4.4/humanloop/models/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/__init__.py` & `humanloop-0.4.4/humanloop/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/chat/post.py` & `humanloop-0.4.4/humanloop/paths/chat/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/chat/post.pyi` & `humanloop-0.4.4/humanloop/paths/chat/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/chat_deployed/post.py` & `humanloop-0.4.4/humanloop/paths/chat_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/chat_deployed/post.pyi` & `humanloop-0.4.4/humanloop/paths/chat_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/chat_experiment/post.py` & `humanloop-0.4.4/humanloop/paths/chat_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/chat_experiment/post.pyi` & `humanloop-0.4.4/humanloop/paths/chat_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/chat_model_config/post.py` & `humanloop-0.4.4/humanloop/paths/chat_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/chat_model_config/post.pyi` & `humanloop-0.4.4/humanloop/paths/chat_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/completion/post.py` & `humanloop-0.4.4/humanloop/paths/completion/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/completion/post.pyi` & `humanloop-0.4.4/humanloop/paths/completion/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/completion_deployed/post.py` & `humanloop-0.4.4/humanloop/paths/completion_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/completion_deployed/post.pyi` & `humanloop-0.4.4/humanloop/paths/completion_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/completion_experiment/post.py` & `humanloop-0.4.4/humanloop/paths/completion_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/completion_experiment/post.pyi` & `humanloop-0.4.4/humanloop/paths/completion_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/completion_model_config/post.py` & `humanloop-0.4.4/humanloop/paths/completion_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/completion_model_config/post.pyi` & `humanloop-0.4.4/humanloop/paths/completion_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/experiments_experiment_id/delete.py` & `humanloop-0.4.4/humanloop/paths/experiments_experiment_id/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/experiments_experiment_id/delete.pyi` & `humanloop-0.4.4/humanloop/paths/experiments_experiment_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/experiments_experiment_id/patch.py` & `humanloop-0.4.4/humanloop/paths/experiments_experiment_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/experiments_experiment_id/patch.pyi` & `humanloop-0.4.4/humanloop/paths/experiments_experiment_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/get.py` & `humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/get.pyi` & `humanloop-0.4.4/humanloop/paths/experiments_experiment_id_model_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/feedback/post.py` & `humanloop-0.4.4/humanloop/paths/feedback/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/feedback/post.pyi` & `humanloop-0.4.4/humanloop/paths/feedback/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/logs/post.py` & `humanloop-0.4.4/humanloop/paths/logs/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/logs/post.pyi` & `humanloop-0.4.4/humanloop/paths/logs/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/model_configs/post.py` & `humanloop-0.4.4/humanloop/paths/model_configs/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/model_configs/post.pyi` & `humanloop-0.4.4/humanloop/paths/model_configs/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/model_configs_id/get.py` & `humanloop-0.4.4/humanloop/paths/model_configs_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/model_configs_id/get.pyi` & `humanloop-0.4.4/humanloop/paths/model_configs_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects/get.py` & `humanloop-0.4.4/humanloop/paths/projects/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects/get.pyi` & `humanloop-0.4.4/humanloop/paths/projects/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects/post.py` & `humanloop-0.4.4/humanloop/paths/projects/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects/post.pyi` & `humanloop-0.4.4/humanloop/paths/projects/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id/get.py` & `humanloop-0.4.4/humanloop/paths/projects_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id/get.pyi` & `humanloop-0.4.4/humanloop/paths/projects_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id/patch.py` & `humanloop-0.4.4/humanloop/paths/projects_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id/patch.pyi` & `humanloop-0.4.4/humanloop/paths/projects_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_active_config/delete.py` & `humanloop-0.4.4/humanloop/paths/projects_id_active_config/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_active_config/delete.pyi` & `humanloop-0.4.4/humanloop/paths/projects_id_active_config/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_active_config/get.py` & `humanloop-0.4.4/humanloop/paths/projects_id_active_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_active_config/get.pyi` & `humanloop-0.4.4/humanloop/paths/projects_id_active_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/delete.py` & `humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/delete.pyi` & `humanloop-0.4.4/humanloop/paths/projects_id_active_experiment/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_configs/get.py` & `humanloop-0.4.4/humanloop/paths/projects_id_configs/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_configs/get.pyi` & `humanloop-0.4.4/humanloop/paths/projects_id_configs/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_export/post.py` & `humanloop-0.4.4/humanloop/paths/projects_id_export/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_export/post.pyi` & `humanloop-0.4.4/humanloop/paths/projects_id_export/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/patch.py` & `humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/patch.pyi` & `humanloop-0.4.4/humanloop/paths/projects_id_feedback_types/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/get.py` & `humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/get.pyi` & `humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/post.py` & `humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/post.pyi` & `humanloop-0.4.4/humanloop/paths/projects_project_id_experiments/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/sessions/get.py` & `humanloop-0.4.4/humanloop/paths/sessions/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/sessions/get.pyi` & `humanloop-0.4.4/humanloop/paths/sessions/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/sessions/post.py` & `humanloop-0.4.4/humanloop/paths/sessions/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/sessions/post.pyi` & `humanloop-0.4.4/humanloop/paths/sessions/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/sessions_id/get.py` & `humanloop-0.4.4/humanloop/paths/sessions_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/sessions_id/get.pyi` & `humanloop-0.4.4/humanloop/paths/sessions_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/traces/post.py` & `humanloop-0.4.4/humanloop/paths/traces/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/paths/traces/post.pyi` & `humanloop-0.4.4/humanloop/paths/traces/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/request_after_hook.py` & `humanloop-0.4.4/humanloop/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/request_before_hook.py` & `humanloop-0.4.4/humanloop/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/rest.py` & `humanloop-0.4.4/humanloop/rest.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/schemas.py` & `humanloop-0.4.4/humanloop/schemas.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/agent_config_request.py` & `humanloop-0.4.4/humanloop/type/agent_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/agent_config_response.py` & `humanloop-0.4.4/humanloop/type/agent_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/base_metric_response.py` & `humanloop-0.4.4/humanloop/type/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/categorical_feedback_label.py` & `humanloop-0.4.4/humanloop/type/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/chat_data_response.py` & `humanloop-0.4.4/humanloop/type/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/chat_deployed_request.py` & `humanloop-0.4.4/humanloop/type/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/chat_experiment_request.py` & `humanloop-0.4.4/humanloop/type/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/chat_message.py` & `humanloop-0.4.4/humanloop/type/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/chat_model_config_request.py` & `humanloop-0.4.4/humanloop/type/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/chat_request.py` & `humanloop-0.4.4/humanloop/type/chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/chat_response.py` & `humanloop-0.4.4/humanloop/type/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/chat_role.py` & `humanloop-0.4.4/humanloop/type/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/completion_deployed_request.py` & `humanloop-0.4.4/humanloop/type/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/completion_experiment_request.py` & `humanloop-0.4.4/humanloop/type/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/completion_model_config_request.py` & `humanloop-0.4.4/humanloop/type/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/completion_request.py` & `humanloop-0.4.4/humanloop/type/completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/completion_response.py` & `humanloop-0.4.4/humanloop/type/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/config_response.py` & `humanloop-0.4.4/humanloop/type/config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/config_type.py` & `humanloop-0.4.4/humanloop/type/config_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/create_experiment_request.py` & `humanloop-0.4.4/humanloop/type/create_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/create_log_response.py` & `humanloop-0.4.4/humanloop/type/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/create_project_request.py` & `humanloop-0.4.4/humanloop/type/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/create_session_response.py` & `humanloop-0.4.4/humanloop/type/create_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/create_trace_request.py` & `humanloop-0.4.4/humanloop/type/create_trace_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/create_trace_response.py` & `humanloop-0.4.4/humanloop/type/create_trace_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/data_response.py` & `humanloop-0.4.4/humanloop/type/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/experiment_config_response.py` & `humanloop-0.4.4/humanloop/type/experiment_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/experiment_response.py` & `humanloop-0.4.4/humanloop/type/experiment_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/experiment_status.py` & `humanloop-0.4.4/humanloop/type/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/experiments_list_response.py` & `humanloop-0.4.4/humanloop/type/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback.py` & `humanloop-0.4.4/humanloop/type/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_class.py` & `humanloop-0.4.4/humanloop/type/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_label_request.py` & `humanloop-0.4.4/humanloop/type/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_request.py` & `humanloop-0.4.4/humanloop/type/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_response.py` & `humanloop-0.4.4/humanloop/type/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_submit_request.py` & `humanloop-0.4.4/humanloop/type/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_submit_response.py` & `humanloop-0.4.4/humanloop/type/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_type.py` & `humanloop-0.4.4/humanloop/type/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_type_model.py` & `humanloop-0.4.4/humanloop/type/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_type_request.py` & `humanloop-0.4.4/humanloop/type/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/feedback_types.py` & `humanloop-0.4.4/humanloop/type/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/generic_config_request.py` & `humanloop-0.4.4/humanloop/type/generic_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/generic_config_response.py` & `humanloop-0.4.4/humanloop/type/generic_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/get_model_config_response.py` & `humanloop-0.4.4/humanloop/type/get_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/http_validation_error.py` & `humanloop-0.4.4/humanloop/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/label_sentiment.py` & `humanloop-0.4.4/humanloop/type/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/log_datapoint_request.py` & `humanloop-0.4.4/humanloop/type/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/log_model_config_request.py` & `humanloop-0.4.4/humanloop/type/log_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/log_request.py` & `humanloop-0.4.4/humanloop/type/log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/log_response.py` & `humanloop-0.4.4/humanloop/type/log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/logs_log_response.py` & `humanloop-0.4.4/humanloop/type/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/model_config_chat_request.py` & `humanloop-0.4.4/humanloop/type/model_config_chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/model_config_completion_request.py` & `humanloop-0.4.4/humanloop/type/model_config_completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/model_config_response.py` & `humanloop-0.4.4/humanloop/type/model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/model_config_response2.py` & `humanloop-0.4.4/humanloop/type/model_config_response2.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/model_endpoints.py` & `humanloop-0.4.4/humanloop/type/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/model_providers.py` & `humanloop-0.4.4/humanloop/type/model_providers.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/paginated_data_log_response.py` & `humanloop-0.4.4/humanloop/type/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/paginated_data_project_response.py` & `humanloop-0.4.4/humanloop/type/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/paginated_data_session_response.py` & `humanloop-0.4.4/humanloop/type/paginated_data_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/positive_label.py` & `humanloop-0.4.4/humanloop/type/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/project_config_response.py` & `humanloop-0.4.4/humanloop/type/project_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/project_model_config_request.py` & `humanloop-0.4.4/humanloop/type/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/project_model_config_response.py` & `humanloop-0.4.4/humanloop/type/project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/project_response.py` & `humanloop-0.4.4/humanloop/type/project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/project_sort_by.py` & `humanloop-0.4.4/humanloop/type/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/project_user_response.py` & `humanloop-0.4.4/humanloop/type/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/projects_get_configs_response.py` & `humanloop-0.4.4/humanloop/type/projects_get_configs_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/projects_update_feedback_types_request.py` & `humanloop-0.4.4/humanloop/type/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/provider_api_keys.py` & `humanloop-0.4.4/humanloop/type/provider_api_keys.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/session_project_response.py` & `humanloop-0.4.4/humanloop/type/session_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/session_response.py` & `humanloop-0.4.4/humanloop/type/session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/sort_order.py` & `humanloop-0.4.4/humanloop/type/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.4/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.4/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/tool_config_request.py` & `humanloop-0.4.4/humanloop/type/tool_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/tool_config_response.py` & `humanloop-0.4.4/humanloop/type/tool_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/tool_result_response.py` & `humanloop-0.4.4/humanloop/type/tool_result_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/trace_log_request.py` & `humanloop-0.4.4/humanloop/type/trace_log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/trace_model_config_request.py` & `humanloop-0.4.4/humanloop/type/trace_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/update_experiment_request.py` & `humanloop-0.4.4/humanloop/type/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/update_project_request.py` & `humanloop-0.4.4/humanloop/type/update_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/usage.py` & `humanloop-0.4.4/humanloop/type/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type/validation_error.py` & `humanloop-0.4.4/humanloop/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/type_util.py` & `humanloop-0.4.4/humanloop/type_util.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/humanloop/validation_metadata.py` & `humanloop-0.4.4/humanloop/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.3/pyproject.toml` & `humanloop-0.4.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "humanloop"
-version = "0.4.3"
+version = "0.4.4"
 description = "Client for Humanloop API"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "humanloop"}]
 
 [tool.poetry.dependencies]
```

### Comparing `humanloop-0.4.3/PKG-INFO` & `humanloop-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanloop
-Version: 0.4.3
+Version: 0.4.4
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
 
-# humanloop@0.4.3
+# humanloop@0.4.4
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.3
+pip install humanloop==0.4.4
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
```


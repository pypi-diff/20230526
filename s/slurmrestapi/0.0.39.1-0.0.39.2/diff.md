# Comparing `tmp/slurmrestapi-0.0.39.1.tar.gz` & `tmp/slurmrestapi-0.0.39.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmrestapi-0.0.39.1.tar", last modified: Fri May 26 01:41:21 2023, max compression
+gzip compressed data, was "slurmrestapi-0.0.39.2.tar", last modified: Fri May 26 02:13:04 2023, max compression
```

## Comparing `slurmrestapi-0.0.39.1.tar` & `slurmrestapi-0.0.39.2.tar`

### file list

```diff
@@ -1,570 +1,570 @@
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/
--rw-r--r--   0 keyemyria   (501) staff       (20)      298 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/PKG-INFO
--rw-r--r--   0 keyemyria   (501) staff       (20)    28416 2023-05-26 01:38:12.000000 slurmrestapi-0.0.39.1/README.md
--rw-r--r--   0 keyemyria   (501) staff       (20)       69 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/setup.cfg
--rw-r--r--   0 keyemyria   (501) staff       (20)     1136 2023-05-26 01:40:39.000000 slurmrestapi-0.0.39.1/setup.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/
--rw-r--r--   0 keyemyria   (501) staff       (20)      731 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    58488 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/api_client.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/
--rw-r--r--   0 keyemyria   (501) staff       (20)      214 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     7168 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/path_to_api.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/
--rw-r--r--   0 keyemyria   (501) staff       (20)      239 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)       97 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/openapi.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      106 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/openapi_json.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      102 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/openapi_v3.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      106 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/openapi_yaml.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_job_job_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_job_submit.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_jobs.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      123 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_node_node_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      153 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_partition_partition_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      127 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_partitions.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      161 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_reservation_reservation_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      131 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurm_v0_0_39_reservations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_account_account_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_accounts.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      230 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_association.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_associations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_cluster_cluster_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_clusters.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_job_job_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_jobs.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      200 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      231 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_qos_qos_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      203 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      237 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_user_user_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      206 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      229 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_wckey_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_wckeys.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      440 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/tag_to_api.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/tags/
--rw-r--r--   0 keyemyria   (501) staff       (20)      329 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/tags/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      719 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/tags/openapi_api.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5807 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/apis/tags/slurm_api.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17342 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/configuration.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4510 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/exceptions.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/
--rw-r--r--   0 keyemyria   (501) staff       (20)      346 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4422 2023-05-26 01:36:51.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_account_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4458 2023-05-26 01:36:51.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_associations_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4446 2023-05-26 01:36:51.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_clusters_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8204 2023-05-26 01:36:51.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_config_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4535 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4062 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1397 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4346 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13002 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4336 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_qos_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5298 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_response_associations_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     7172 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_set_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4355 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_tres_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2505 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_tres_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2486 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_update_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2517 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_update_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4365 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_user_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3492 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_warning.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1417 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_warnings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3732 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_wckey_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3738 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/status.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6821 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1385 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_account_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6300 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_accounting.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1412 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_accounting_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5876 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_acct_gather_energy.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_acct_gather_energy_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    24335 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      588 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1367 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3993 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_short.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1413 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_short_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_short_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9791 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_usage.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_usage_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13467 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_cluster_rec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1413 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_cluster_rec_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3961 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_controller_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1451 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_controller_ping_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2910 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_coord.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1367 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_coord_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11112 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_cron_entry.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      593 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_cron_entry_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1279 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_csv_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4361 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4058 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1379 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4627 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_ext_sensors_data.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_ext_sensors_data_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3484 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_float64_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1281 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_hostlist.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1293 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_hostlist_string.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    48231 2023-05-26 01:36:56.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5214 2023-05-26 01:36:56.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_array_response_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-26 01:36:56.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_array_response_msg_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)   104040 2023-05-26 01:36:57.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg_argv.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg_env.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1414 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      599 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg_spank_env.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2052 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_exclusive.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6447 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_exit_code.py
--rw-r--r--   0 keyemyria   (501) staff       (20)   103636 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1299 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_info_gres_detail.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1384 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_info_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1349 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      593 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_mem_per_cpu.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_mem_per_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5027 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_res.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1609 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_res_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      590 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_res_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3788 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_submission.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5450 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_submission_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4436 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_update_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4332 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_jobs_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6796 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_license.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1379 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4356 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_licenses_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12998 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    49226 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1352 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4307 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_nodes_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    36220 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_partition_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1442 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_partition_info_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4460 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_partitions_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4391 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_pings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     7422 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_power_mgmt_data.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      597 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_power_mgmt_data_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    26380 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1349 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_qos_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1293 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_qos_preempt_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1318 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_qos_string_id_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2877 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservation_core_spec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    24061 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservation_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1460 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservation_info_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1495 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservation_info_core_spec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4498 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservations_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     7457 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_rollup_stats.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_rollup_stats_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3643 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_slurm_step_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    32111 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6044 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_msg_rpcs_by_type.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5932 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_msg_rpcs_by_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4397 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_rec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_rec_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5623 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_rpc.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1395 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_rpc_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5638 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1404 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_user_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    32486 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1358 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      590 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1370 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_tres_req_max.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1370 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_tres_req_min.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1374 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_tres_usage_max.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1374 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_tres_usage_min.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1287 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_string_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3863 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1358 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_tres_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      588 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_tres_str.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3459 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_uint16_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3459 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_uint32_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3459 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_uint64_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17972 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_update_node_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12437 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1358 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_user_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3488 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_warning.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1399 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_warnings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6390 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1367 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_wckey_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4257 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_wckey_tag.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/models/
--rw-r--r--   0 keyemyria   (501) staff       (20)     9276 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/models/__init__.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/
--rw-r--r--   0 keyemyria   (501) staff       (20)     2215 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/__init__.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi/
--rw-r--r--   0 keyemyria   (501) staff       (20)      297 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6911 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_json/
--rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_json/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6970 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_json/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_v3/
--rw-r--r--   0 keyemyria   (501) staff       (20)      303 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_v3/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6946 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_v3/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_yaml/
--rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_yaml/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6970 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_yaml/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9190 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_diag/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15026 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10760 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17861 2023-05-26 01:37:08.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_submit/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_submit/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15525 2023-05-26 01:37:08.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_submit/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11454 2023-05-26 01:37:07.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_jobs/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_licenses/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_licenses/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8971 2023-05-26 01:37:08.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_licenses/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11218 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11264 2023-05-26 01:37:07.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17815 2023-05-26 01:37:08.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_nodes/
--rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_nodes/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11470 2023-05-26 01:37:07.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_nodes/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      359 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13566 2023-05-26 01:37:07.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_partitions/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_partitions/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11550 2023-05-26 01:37:07.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_partitions/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_ping/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_ping/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9188 2023-05-26 01:37:08.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_ping/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      367 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13612 2023-05-26 01:37:07.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_reservations/
--rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_reservations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11582 2023-05-26 01:37:07.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_reservations/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11297 2023-05-26 01:37:09.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13833 2023-05-26 01:37:10.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11827 2023-05-26 01:37:10.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15503 2023-05-26 01:37:13.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_association/
--rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_association/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12415 2023-05-26 01:37:09.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_association/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12325 2023-05-26 01:37:10.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_association/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12427 2023-05-26 01:37:09.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12336 2023-05-26 01:37:10.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15599 2023-05-26 01:37:13.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11297 2023-05-26 01:37:09.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11347 2023-05-26 01:37:11.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9341 2023-05-26 01:37:11.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15461 2023-05-26 01:37:08.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_config/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_config/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9329 2023-05-26 01:37:11.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_config/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15847 2023-05-26 01:37:12.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_config/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9228 2023-05-26 01:37:10.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_diag/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11237 2023-05-26 01:37:11.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    18842 2023-05-26 01:37:11.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_jobs/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/
--rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11752 2023-05-26 01:37:11.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15413 2023-05-26 01:37:13.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11221 2023-05-26 01:37:09.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13817 2023-05-26 01:37:12.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8811 2023-05-26 01:37:12.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15435 2023-05-26 01:37:13.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      343 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11240 2023-05-26 01:37:10.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13764 2023-05-26 01:37:12.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_users/
--rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_users/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11779 2023-05-26 01:37:12.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_users/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15454 2023-05-26 01:37:13.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_users/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/
--rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11227 2023-05-26 01:37:10.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11265 2023-05-26 01:37:12.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9305 2023-05-26 01:37:12.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15823 2023-05-26 01:37:09.000000 slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/post.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10661 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/rest.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    97642 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/slurmrestapi/schemas.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi.egg-info/
--rw-r--r--   0 keyemyria   (501) staff       (20)      298 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi.egg-info/PKG-INFO
--rw-r--r--   0 keyemyria   (501) staff       (20)    23247 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi.egg-info/SOURCES.txt
--rw-r--r--   0 keyemyria   (501) staff       (20)        1 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi.egg-info/dependency_links.txt
--rw-r--r--   0 keyemyria   (501) staff       (20)      118 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi.egg-info/requires.txt
--rw-r--r--   0 keyemyria   (501) staff       (20)       18 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/slurmrestapi.egg-info/top_level.txt
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_models/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:15.000000 slurmrestapi-0.0.39.1/test/test_models/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 01:36:51.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_account_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-26 01:36:51.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_associations_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-26 01:36:51.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_clusters_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_config_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      540 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      544 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      548 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      540 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_qos_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      630 2023-05-26 01:36:52.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_response_associations_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_set_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_tres_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_tres_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_update_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_update_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_user_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      552 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_warning.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      556 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_warnings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_wckey_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      519 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_status.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      544 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_account_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      556 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_accounting.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_accounting_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      582 2023-05-26 01:36:53.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_acct_gather_energy.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_acct_gather_energy_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_short.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_short_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_short_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_usage.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 01:36:54.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_usage_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_cluster_rec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_cluster_rec_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_controller_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_controller_ping_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_coord.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_coord_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_cron_entry.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_cron_entry_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_csv_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      540 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_ext_sensors_data.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      587 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_ext_sensors_data_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_float64_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      548 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_hostlist.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-26 01:36:55.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_hostlist_string.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      528 2023-05-26 01:36:56.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-26 01:36:56.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_array_response_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-26 01:36:56.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_array_response_msg_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-26 01:36:57.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg_argv.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg_env.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg_spank_env.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_exclusive.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 01:36:58.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_exit_code.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      587 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_info_gres_detail.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_info_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_mem_per_cpu.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-26 01:36:59.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_mem_per_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      541 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_res.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_res_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_res_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_submission.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      602 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_submission_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      586 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_update_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_jobs_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      544 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_license.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      548 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_licenses_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 01:37:00.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_nodes_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_partition_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      590 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_partition_info_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_partitions_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 01:37:01.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_pings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_power_mgmt_data.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_power_mgmt_data_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      528 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_qos_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_qos_preempt_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_qos_string_id_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservation_core_spec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      577 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservation_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservation_info_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      611 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservation_info_core_spec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      597 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservations_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 01:37:02.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_rollup_stats.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_rollup_stats_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_slurm_step_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_msg_rpcs_by_type.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_msg_rpcs_by_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_rec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_rec_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_rpc.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_rpc_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 01:37:03.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_user_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_step.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_tres_req_max.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_tres_req_min.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_tres_usage_max.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_tres_usage_min.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_string_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_tres_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_tres_str.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 01:37:04.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_uint16_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_uint32_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_uint64_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_update_node_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_user_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      544 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_warning.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      548 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_warnings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_wckey_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 01:37:05.000000 slurmrestapi-0.0.39.1/test/test_models/test_v0039_wckey_tag.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/
--rw-r--r--   0 keyemyria   (501) staff       (20)     1995 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/__init__.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      826 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_json/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_json/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_json/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_v3/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_v3/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      833 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_v3/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_yaml/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_yaml/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-26 01:37:06.000000 slurmrestapi-0.0.39.1/test/test_paths/test_openapi_yaml/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_diag/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      845 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      833 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_submit/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_submit/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_submit/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      818 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_jobs/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_licenses/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_licenses/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_licenses/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_node_node_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_node_node_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      857 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_nodes/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_nodes/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      822 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_nodes/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_partition_partition_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_partition_partition_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      876 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_partition_partition_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_partitions/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_partitions/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_partitions/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_ping/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_ping/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      811 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_ping/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      890 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_reservations/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_reservations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      850 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_reservations/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_accounts/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_accounts/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_accounts/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_accounts/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_association/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_association/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_association/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      849 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_association/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_associations/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_associations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_clusters/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_clusters/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_clusters/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_clusters/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_config/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_config/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_config/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      851 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_config/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      831 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_diag/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      834 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_job_job_id/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      820 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_jobs/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      840 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_tres/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_tres/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      821 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_tres/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_tres/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      854 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_users/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_users/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_users/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      829 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_users/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:41:21.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      827 2023-05-26 01:37:14.000000 slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      298 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/PKG-INFO
+-rw-r--r--   0 keyemyria   (501) staff       (20)    28416 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/README.md
+-rw-r--r--   0 keyemyria   (501) staff       (20)       69 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/setup.cfg
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1136 2023-05-26 02:12:32.000000 slurmrestapi-0.0.39.2/setup.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      731 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    58488 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/api_client.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      214 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     7168 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/path_to_api.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      239 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)       97 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/openapi.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      106 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/openapi_json.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      102 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/openapi_v3.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      106 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/openapi_yaml.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_job_job_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_job_submit.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_jobs.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      123 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_node_node_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      153 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_partition_partition_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      127 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_partitions.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      161 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_reservation_reservation_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      131 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurm_v0_0_39_reservations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_account_account_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_accounts.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      230 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_association.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_associations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_cluster_cluster_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_clusters.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_job_job_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_jobs.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      200 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      231 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_qos_qos_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      203 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      237 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_user_user_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      206 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      229 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_wckey_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/paths/slurmdb_v0_0_39_wckeys.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      440 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/tag_to_api.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/tags/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      329 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/tags/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      719 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/tags/openapi_api.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5807 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/apis/tags/slurm_api.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17342 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/configuration.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4510 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/exceptions.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      346 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4422 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_account_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4458 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_associations_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4446 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_clusters_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8204 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_config_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4535 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4062 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1397 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4346 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13002 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4336 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_qos_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5298 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_response_associations_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     7172 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_set_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4355 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_tres_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2505 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_tres_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2486 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_update_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2517 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_update_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4365 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_user_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3492 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_warning.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1417 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_warnings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3732 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_wckey_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3738 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/status.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6821 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1385 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_account_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6300 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_accounting.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1412 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_accounting_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5876 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_acct_gather_energy.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_acct_gather_energy_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    24335 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      588 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1367 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3993 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_short.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1413 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_short_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_short_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9791 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_usage.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_usage_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13467 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_cluster_rec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1413 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_cluster_rec_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3961 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_controller_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1451 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_controller_ping_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2910 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_coord.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1367 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_coord_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11112 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_cron_entry.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      593 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_cron_entry_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1279 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_csv_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4361 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4058 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1379 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4627 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_ext_sensors_data.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_ext_sensors_data_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3484 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_float64_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1281 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_hostlist.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1293 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_hostlist_string.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    48231 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5214 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_array_response_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_array_response_msg_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)   104040 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg_argv.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg_env.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1414 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      599 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg_spank_env.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2052 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_exclusive.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6447 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_exit_code.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)   103636 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1299 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_info_gres_detail.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1384 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_info_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1349 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      593 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_mem_per_cpu.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_mem_per_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5027 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_res.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1609 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_res_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      590 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_res_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3788 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_submission.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5450 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_submission_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4436 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_update_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4332 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_jobs_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6796 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_license.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1379 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4356 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_licenses_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12998 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    49226 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1352 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4307 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_nodes_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    36220 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_partition_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1442 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_partition_info_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4460 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_partitions_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4391 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_pings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     7422 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_power_mgmt_data.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      597 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_power_mgmt_data_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    26380 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1349 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_qos_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1293 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_qos_preempt_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1318 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_qos_string_id_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2877 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservation_core_spec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    24061 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservation_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1460 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservation_info_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1495 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservation_info_core_spec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4498 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservations_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     7457 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_rollup_stats.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_rollup_stats_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3643 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_slurm_step_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    32111 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6044 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_msg_rpcs_by_type.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5932 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_msg_rpcs_by_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4397 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_rec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_rec_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5623 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_rpc.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1395 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_rpc_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5638 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1404 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_user_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    32486 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1358 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      590 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1370 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_tres_req_max.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1370 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_tres_req_min.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1374 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_tres_usage_max.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1374 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_tres_usage_min.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1287 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_string_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3863 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1358 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_tres_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      588 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_tres_str.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3459 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_uint16_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3459 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_uint32_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3459 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_uint64_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17972 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_update_node_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12437 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1358 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_user_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3488 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_warning.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1399 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_warnings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6390 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1367 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_wckey_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4257 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_wckey_tag.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/models/
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9276 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/models/__init__.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2215 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/__init__.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      297 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6911 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_json/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_json/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6970 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_json/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_v3/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      303 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_v3/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6946 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_v3/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_yaml/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_yaml/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6970 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_yaml/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9190 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_diag/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15026 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_job_id/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10760 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_job_id/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17861 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_job_id/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_submit/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_submit/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15525 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_submit/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11454 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_jobs/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_licenses/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_licenses/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8971 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_licenses/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_node_node_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_node_node_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11218 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_node_node_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11264 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_node_node_name/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17815 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_node_node_name/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_nodes/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_nodes/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11470 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_nodes/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      359 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13566 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_partitions/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_partitions/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11550 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_partitions/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_ping/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_ping/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9188 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_ping/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      367 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13612 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_reservations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_reservations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11582 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_reservations/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11297 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13833 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_accounts/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_accounts/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11827 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_accounts/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15503 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_accounts/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_association/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_association/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12415 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_association/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12325 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_association/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_associations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_associations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12427 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_associations/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12336 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_associations/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15599 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_associations/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11297 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11347 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_clusters/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_clusters/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9341 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_clusters/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15461 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_clusters/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_config/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_config/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9329 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_config/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15847 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_config/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9228 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_diag/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11237 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    18842 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_jobs/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11752 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15413 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11221 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13817 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_tres/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_tres/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8811 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_tres/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15435 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_tres/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      343 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11240 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13764 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_users/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_users/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11779 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_users/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15454 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_users/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11227 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11265 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9305 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15823 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/post.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10661 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/rest.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    97642 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/slurmrestapi/schemas.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi.egg-info/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      298 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi.egg-info/PKG-INFO
+-rw-r--r--   0 keyemyria   (501) staff       (20)    23247 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyemyria   (501) staff       (20)        1 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyemyria   (501) staff       (20)      118 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi.egg-info/requires.txt
+-rw-r--r--   0 keyemyria   (501) staff       (20)       18 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/slurmrestapi.egg-info/top_level.txt
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_models/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_models/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_account_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_associations_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_clusters_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_config_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      540 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      544 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      548 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      540 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_qos_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      630 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_response_associations_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_set_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_tres_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_tres_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_update_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_update_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_user_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      552 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_warning.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      556 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_warnings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_wckey_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      519 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_status.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      544 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_account_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      556 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_accounting.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_accounting_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      582 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_acct_gather_energy.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_acct_gather_energy_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_short.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_short_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_short_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_usage.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_usage_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      557 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_cluster_rec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_cluster_rec_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_controller_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_controller_ping_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_coord.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_coord_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_cron_entry.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_cron_entry_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_csv_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      540 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_ext_sensors_data.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      587 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_ext_sensors_data_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_float64_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      548 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_hostlist.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_hostlist_string.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      528 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_array_response_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_array_response_msg_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg_argv.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg_env.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg_spank_env.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_exclusive.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_exit_code.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      587 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_info_gres_detail.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_info_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_mem_per_cpu.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_mem_per_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      541 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_res.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_res_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_res_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_submission.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      602 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_submission_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      586 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_update_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_jobs_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      544 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_license.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      548 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      565 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_licenses_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_nodes_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      569 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_partition_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      590 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_partition_info_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_partitions_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_pings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_power_mgmt_data.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_power_mgmt_data_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      528 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_qos_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_qos_preempt_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_qos_string_id_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservation_core_spec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      577 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservation_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservation_info_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      611 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservation_info_core_spec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      597 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservations_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_rollup_stats.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_rollup_stats_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_slurm_step_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_msg_rpcs_by_type.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_msg_rpcs_by_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_rec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_rec_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_rpc.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_rpc_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_user_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_step.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_tres_req_max.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_tres_req_min.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_tres_usage_max.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_tres_usage_min.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      561 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_string_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_tres_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      545 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_tres_str.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_uint16_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_uint32_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_uint64_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_update_node_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      532 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_user_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      544 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_warning.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      548 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_warnings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      536 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      553 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_wckey_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      549 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_models/test_v0039_wckey_tag.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1995 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/__init__.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      826 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_json/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_json/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_json/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_v3/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_v3/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      833 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_v3/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_yaml/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_yaml/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-26 02:09:47.000000 slurmrestapi-0.0.39.2/test/test_paths/test_openapi_yaml/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_diag/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      845 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_job_id/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_job_id/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      833 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_job_id/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_submit/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_submit/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_submit/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      818 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_jobs/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_licenses/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_licenses/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_licenses/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_node_node_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_node_node_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_node_node_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_node_node_name/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      857 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_node_node_name/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_nodes/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_nodes/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      822 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_nodes/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_partition_partition_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_partition_partition_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      876 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_partition_partition_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_partitions/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_partitions/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_partitions/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_ping/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_ping/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      811 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_ping/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      890 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_reservations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_reservations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      850 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_reservations/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_account_account_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_account_account_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_accounts/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_accounts/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_accounts/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_accounts/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_association/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_association/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_association/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      849 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_association/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_associations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_associations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_associations/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_associations/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_associations/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_clusters/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_clusters/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_clusters/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_clusters/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_config/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_config/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_config/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      851 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_config/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      831 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_diag/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      834 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_job_job_id/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      820 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_jobs/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      840 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_tres/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_tres/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      821 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_tres/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_tres/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_user_user_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_user_user_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      854 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_users/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_users/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_users/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      829 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_users/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:13:04.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckeys/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckeys/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      827 2023-05-26 02:12:12.000000 slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_post.py
```

### Comparing `slurmrestapi-0.0.39.1/README.md` & `slurmrestapi-0.0.39.2/README.md`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/setup.py` & `slurmrestapi-0.0.39.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
     Contact: sales@schedmd.com
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "slurmrestapi"
-VERSION = "0.0.39.1"
+VERSION = "0.0.39.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 REQUIRES = [
     "certifi >= 14.5.14",
     "frozendict ~= 2.3.4",
-    "python-dateutil ~= 2.7.0",
+    "python-dateutil ~= 2.8.0",
     "setuptools >= 21.0.0",
     "typing_extensions ~= 4.3.0",
     "urllib3 ~= 1.26.7",
 ]
 
 setup(
     name=NAME,
```

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/__init__.py` & `slurmrestapi-0.0.39.2/slurmrestapi/__init__.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/api_client.py` & `slurmrestapi-0.0.39.2/slurmrestapi/api_client.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/apis/path_to_api.py` & `slurmrestapi-0.0.39.2/slurmrestapi/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/apis/tags/openapi_api.py` & `slurmrestapi-0.0.39.2/slurmrestapi/apis/tags/openapi_api.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/apis/tags/slurm_api.py` & `slurmrestapi-0.0.39.2/slurmrestapi/apis/tags/slurm_api.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/configuration.py` & `slurmrestapi-0.0.39.2/slurmrestapi/configuration.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/exceptions.py` & `slurmrestapi-0.0.39.2/slurmrestapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_account_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_account_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_associations_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_associations_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_clusters_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_clusters_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_config_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_config_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_diag.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_error.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_errors.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_job_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_meta.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_qos_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_qos_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_response_associations_delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_response_associations_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_set_config.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_set_config.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_tres_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_tres_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_tres_update.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_tres_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_update_qos.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_update_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_update_users.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_update_users.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_user_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_user_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_warning.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_warning.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_warnings.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_warnings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/dbv0039_wckey_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/dbv0039_wckey_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/status.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/status.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_account.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_account_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_account_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_accounting.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_accounting.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_accounting_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_accounting_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_acct_gather_energy.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_acct_gather_energy.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_acct_gather_energy_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_acct_gather_energy_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_id.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_id.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_short.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_short.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_short_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_short_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_short_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_short_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_usage.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_usage.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_assoc_usage_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_assoc_usage_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_cluster_rec.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_cluster_rec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_cluster_rec_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_cluster_rec_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_controller_ping.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_controller_ping.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_controller_ping_array.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_controller_ping_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_coord.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_coord.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_coord_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_coord_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_cron_entry.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_cron_entry.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_cron_entry_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_cron_entry_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_csv_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_csv_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_diag.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_error.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_errors.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_ext_sensors_data.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_ext_sensors_data.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_ext_sensors_data_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_ext_sensors_data_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_float64_no_val.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_float64_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_hostlist.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_hostlist.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_hostlist_string.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_hostlist_string.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_array_response_msg.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_array_response_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_array_response_msg_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_array_response_msg_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg_argv.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg_argv.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg_env.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg_env.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_desc_msg_spank_env.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_desc_msg_spank_env.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_exclusive.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_exclusive.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_exit_code.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_info_gres_detail.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_info_gres_detail.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_info_msg.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_info_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_mem_per_cpu.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_mem_per_cpu.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_mem_per_node.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_mem_per_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_res.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_res.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_res_nodes.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_res_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_res_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_res_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_submission.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_submission.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_submission_response.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_job_update_response.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_job_update_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_jobs_response.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_jobs_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_license.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_license.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_licenses.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_licenses.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_licenses_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_licenses_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_meta.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_node.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_nodes.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_nodes_response.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_nodes_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_partition_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_partition_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_partition_info_array.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_partition_info_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_partitions_response.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_partitions_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_pings.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_pings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_power_mgmt_data.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_power_mgmt_data.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_power_mgmt_data_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_power_mgmt_data_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_qos.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_qos_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_qos_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_qos_preempt_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_qos_preempt_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_qos_string_id_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_qos_string_id_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservation_core_spec.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservation_core_spec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservation_info.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservation_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservation_info_array.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservation_info_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservation_info_core_spec.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservation_info_core_spec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_reservations_response.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_reservations_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_rollup_stats.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_rollup_stats.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_rollup_stats_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_rollup_stats_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_slurm_step_id.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_slurm_step_id.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_msg.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_msg_rpcs_by_type.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_msg_rpcs_by_type.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_msg_rpcs_by_user.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_msg_rpcs_by_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_rec.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_rec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_rec_ptr.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_rec_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_rpc.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_rpc.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_rpc_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_rpc_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_user.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_stats_user_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_stats_user_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_nodes.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_tres_req_max.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_tres_req_max.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_tres_req_min.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_tres_req_min.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_tres_usage_max.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_tres_usage_max.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_step_tres_usage_min.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_step_tres_usage_min.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_string_array.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_string_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_tres.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_tres.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_tres_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_tres_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_tres_str.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_tres_str.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_uint16_no_val.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_uint16_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_uint32_no_val.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_uint32_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_uint64_no_val.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_uint64_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_update_node_msg.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_update_node_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_user.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_user_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_user_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_warning.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_warning.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_warnings.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_warnings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_wckey.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_wckey.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_wckey_list.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_wckey_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/model/v0039_wckey_tag.py` & `slurmrestapi-0.0.39.2/slurmrestapi/model/v0039_wckey_tag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/models/__init__.py` & `slurmrestapi-0.0.39.2/slurmrestapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/__init__.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_json/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_json/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_v3/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_v3/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/openapi_yaml/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/openapi_yaml/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_diag/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_diag/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_job_id/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_job_id/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_job_id/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_job_submit/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_job_submit/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_jobs/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_jobs/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_licenses/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_licenses/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_node_node_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_node_node_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_node_node_name/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_nodes/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_nodes/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_partitions/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_partitions/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_ping/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_ping/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurm_v0_0_39_reservations/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurm_v0_0_39_reservations/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_accounts/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_accounts/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_association/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_association/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_association/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_association/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_associations/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_associations/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_associations/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_clusters/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_clusters/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_config/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_config/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_config/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_config/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_diag/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_diag/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_jobs/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_jobs/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_tres/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_tres/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_users/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_users/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_users/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_users/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/delete.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/get.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/post.py` & `slurmrestapi-0.0.39.2/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/rest.py` & `slurmrestapi-0.0.39.2/slurmrestapi/rest.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi/schemas.py` & `slurmrestapi-0.0.39.2/slurmrestapi/schemas.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/slurmrestapi.egg-info/SOURCES.txt` & `slurmrestapi-0.0.39.2/slurmrestapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_account_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_account_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_associations_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_associations_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_clusters_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_clusters_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_config_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_config_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_diag.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_error.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_errors.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_job_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_meta.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_qos_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_qos_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_response_associations_delete.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_response_associations_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_set_config.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_set_config.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_tres_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_tres_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_tres_update.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_tres_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_update_qos.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_update_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_update_users.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_update_users.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_user_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_user_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_warning.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_warning.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_warnings.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_warnings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_dbv0039_wckey_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_dbv0039_wckey_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_status.py` & `slurmrestapi-0.0.39.2/test/test_models/test_status.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_account.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_account_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_account_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_accounting.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_accounting.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_accounting_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_accounting_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_acct_gather_energy.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_acct_gather_energy.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_acct_gather_energy_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_acct_gather_energy_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_id.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_id.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_short.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_short.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_short_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_short_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_short_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_short_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_usage.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_usage.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_assoc_usage_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_assoc_usage_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_cluster_rec.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_cluster_rec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_cluster_rec_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_cluster_rec_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_controller_ping.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_controller_ping.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_controller_ping_array.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_controller_ping_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_coord.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_coord.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_coord_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_coord_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_cron_entry.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_cron_entry.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_cron_entry_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_cron_entry_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_csv_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_csv_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_diag.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_error.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_errors.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_ext_sensors_data.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_ext_sensors_data.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_ext_sensors_data_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_ext_sensors_data_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_float64_no_val.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_float64_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_hostlist.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_hostlist.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_hostlist_string.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_hostlist_string.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_array_response_msg.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_array_response_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_array_response_msg_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_array_response_msg_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg_argv.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg_argv.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg_env.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg_env.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_desc_msg_spank_env.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_desc_msg_spank_env.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_exclusive.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_exclusive.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_exit_code.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_info_gres_detail.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_info_gres_detail.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_info_msg.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_info_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_mem_per_cpu.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_mem_per_cpu.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_mem_per_node.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_mem_per_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_res.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_res.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_res_nodes.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_res_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_res_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_res_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_submission.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_submission.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_submission_response.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_job_update_response.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_job_update_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_jobs_response.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_jobs_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_license.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_license.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_licenses.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_licenses.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_licenses_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_licenses_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_meta.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_node.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_nodes.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_nodes_response.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_nodes_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_partition_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_partition_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_partition_info_array.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_partition_info_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_partitions_response.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_partitions_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_pings.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_pings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_power_mgmt_data.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_power_mgmt_data.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_power_mgmt_data_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_power_mgmt_data_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_qos.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_qos_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_qos_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_qos_preempt_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_qos_preempt_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_qos_string_id_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_qos_string_id_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservation_core_spec.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservation_core_spec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservation_info.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservation_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservation_info_array.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservation_info_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservation_info_core_spec.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservation_info_core_spec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_reservations_response.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_reservations_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_rollup_stats.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_rollup_stats.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_rollup_stats_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_rollup_stats_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_slurm_step_id.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_slurm_step_id.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_msg.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_msg_rpcs_by_type.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_msg_rpcs_by_type.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_msg_rpcs_by_user.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_msg_rpcs_by_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_rec.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_rec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_rec_ptr.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_rec_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_rpc.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_rpc.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_rpc_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_rpc_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_user.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_stats_user_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_stats_user_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_step.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_step.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_nodes.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_tres_req_max.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_tres_req_max.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_tres_req_min.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_tres_req_min.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_tres_usage_max.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_tres_usage_max.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_step_tres_usage_min.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_step_tres_usage_min.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_string_array.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_string_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_tres.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_tres.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_tres_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_tres_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_tres_str.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_tres_str.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_uint16_no_val.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_uint16_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_uint32_no_val.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_uint32_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_uint64_no_val.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_uint64_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_update_node_msg.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_update_node_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_user.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_user_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_user_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_warning.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_warning.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_warnings.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_warnings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_wckey.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_wckey.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_wckey_list.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_wckey_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_models/test_v0039_wckey_tag.py` & `slurmrestapi-0.0.39.2/test/test_models/test_v0039_wckey_tag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/__init__.py` & `slurmrestapi-0.0.39.2/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_openapi/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_openapi/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_openapi_json/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_openapi_json/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_openapi_v3/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_openapi_v3/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_openapi_yaml/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_openapi_yaml/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_diag/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_diag/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_job_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_job_id/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_job_id/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_job_submit/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_job_submit/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_jobs/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_licenses/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_licenses/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_node_node_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_node_node_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_node_node_name/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_nodes/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_nodes/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_partition_partition_name/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_partition_partition_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_partitions/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_partitions/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_ping/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_ping/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurm_v0_0_39_reservations/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurm_v0_0_39_reservations/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_accounts/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_accounts/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_accounts/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_accounts/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_association/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_association/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_association/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_association/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_associations/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_associations/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_associations/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_clusters/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_clusters/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_clusters/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_clusters/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_config/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_config/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_config/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_config/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_diag/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_diag/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_job_job_id/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_job_job_id/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_jobs/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_tres/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_tres/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_tres/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_tres/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_users/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_users/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_users/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_users/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_delete.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_get.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-0.0.39.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_post.py` & `slurmrestapi-0.0.39.2/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_post.py`

 * *Files identical despite different names*


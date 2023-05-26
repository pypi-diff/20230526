# Comparing `tmp/sonatype_nexus_sdk-0.1.0.tar.gz` & `tmp/sonatype_nexus_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonatype_nexus_sdk-0.1.0.tar", max compression
+gzip compressed data, was "sonatype_nexus_sdk-0.1.3.tar", max compression
```

## Comparing `sonatype_nexus_sdk-0.1.0.tar` & `sonatype_nexus_sdk-0.1.3.tar`

### file list

```diff
@@ -1,1286 +1,1286 @@
--rw-r--r--   0        0        0   113061 2023-05-26 16:01:04.885693 sonatype_nexus_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      641 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/__init__.py
--rw-r--r--   0        0        0    59495 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/api_client.py
--rw-r--r--   0        0        0      215 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/__init__.py
--rw-r--r--   0        0        0    46580 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/path_to_api.py
--rw-r--r--   0        0        0      236 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/__init__.py
--rw-r--r--   0        0        0      220 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/beta_replication_connection.py
--rw-r--r--   0        0        0      330 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/beta_replication_connection_name.py
--rw-r--r--   0        0        0      157 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/beta_replicationtarget_repository_enable.py
--rw-r--r--   0        0        0      205 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/beta_replicationtarget_repository_repository_name_enable.py
--rw-r--r--   0        0        0       97 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_assets.py
--rw-r--r--   0        0        0      181 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_assets_id.py
--rw-r--r--   0        0        0      146 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_azureblobstore_test_connection.py
--rw-r--r--   0        0        0      105 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores.py
--rw-r--r--   0        0        0      119 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_azure.py
--rw-r--r--   0        0        0      207 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_azure_name.py
--rw-r--r--   0        0        0      117 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_file.py
--rw-r--r--   0        0        0      204 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_file_name.py
--rw-r--r--   0        0        0      119 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_group.py
--rw-r--r--   0        0        0      192 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_group_convert_name_new_name_for_original.py
--rw-r--r--   0        0        0      207 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_group_name.py
--rw-r--r--   0        0        0      123 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_name.py
--rw-r--r--   0        0        0      138 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_name_quota_status.py
--rw-r--r--   0        0        0      113 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_s3.py
--rw-r--r--   0        0        0      198 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_blobstores_s3_name.py
--rw-r--r--   0        0        0      179 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_components.py
--rw-r--r--   0        0        0      193 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_components_id.py
--rw-r--r--   0        0        0      236 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_email.py
--rw-r--r--   0        0        0      111 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_email_verify.py
--rw-r--r--   0        0        0      136 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_formats_format_upload_specs.py
--rw-r--r--   0        0        0      123 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_formats_upload_specs.py
--rw-r--r--   0        0        0      152 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_iq.py
--rw-r--r--   0        0        0      107 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_iq_disable.py
--rw-r--r--   0        0        0      105 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_iq_enable.py
--rw-r--r--   0        0        0      126 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_iq_verify_connection.py
--rw-r--r--   0        0        0      116 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_lifecycle_bounce.py
--rw-r--r--   0        0        0      190 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_lifecycle_phase.py
--rw-r--r--   0        0        0      102 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_read_only.py
--rw-r--r--   0        0        0      131 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_read_only_force_release.py
--rw-r--r--   0        0        0      118 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_read_only_freeze.py
--rw-r--r--   0        0        0      120 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_read_only_release.py
--rw-r--r--   0        0        0      109 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories.py
--rw-r--r--   0        0        0      132 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_apt_hosted.py
--rw-r--r--   0        0        0      259 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_apt_hosted_repository_name.py
--rw-r--r--   0        0        0      130 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_apt_proxy.py
--rw-r--r--   0        0        0      256 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_apt_proxy_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_bower_group.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_bower_group_repository_name.py
--rw-r--r--   0        0        0      136 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_bower_hosted.py
--rw-r--r--   0        0        0      265 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_bower_hosted_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_bower_proxy.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_bower_proxy_repository_name.py
--rw-r--r--   0        0        0      142 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_cocoapods_proxy.py
--rw-r--r--   0        0        0      292 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_cocoapods_proxy_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_conan_proxy.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_conan_proxy_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_conda_proxy.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_conda_proxy_repository_name.py
--rw-r--r--   0        0        0      136 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_docker_group.py
--rw-r--r--   0        0        0      265 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_docker_group_repository_name.py
--rw-r--r--   0        0        0      138 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_docker_hosted.py
--rw-r--r--   0        0        0      268 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_docker_hosted_repository_name.py
--rw-r--r--   0        0        0      136 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_docker_proxy.py
--rw-r--r--   0        0        0      265 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_docker_proxy_repository_name.py
--rw-r--r--   0        0        0      138 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_gitlfs_hosted.py
--rw-r--r--   0        0        0      268 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_gitlfs_hosted_repository_name.py
--rw-r--r--   0        0        0      128 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_go_group.py
--rw-r--r--   0        0        0      253 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_go_group_repository_name.py
--rw-r--r--   0        0        0      128 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_go_proxy.py
--rw-r--r--   0        0        0      253 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_go_proxy_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_helm_hosted.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_helm_hosted_repository_name.py
--rw-r--r--   0        0        0      132 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_helm_proxy.py
--rw-r--r--   0        0        0      259 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_helm_proxy_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_maven_group.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_maven_group_repository_name.py
--rw-r--r--   0        0        0      136 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_maven_hosted.py
--rw-r--r--   0        0        0      265 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_maven_hosted_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_maven_proxy.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_maven_proxy_repository_name.py
--rw-r--r--   0        0        0      130 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_npm_group.py
--rw-r--r--   0        0        0      256 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_npm_group_repository_name.py
--rw-r--r--   0        0        0      132 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_npm_hosted.py
--rw-r--r--   0        0        0      259 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_npm_hosted_repository_name.py
--rw-r--r--   0        0        0      130 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_npm_proxy.py
--rw-r--r--   0        0        0      256 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_npm_proxy_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_nuget_group.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_nuget_group_repository_name.py
--rw-r--r--   0        0        0      136 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_nuget_hosted.py
--rw-r--r--   0        0        0      265 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_nuget_hosted_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_nuget_proxy.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_nuget_proxy_repository_name.py
--rw-r--r--   0        0        0      128 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_p2_proxy.py
--rw-r--r--   0        0        0      253 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_p2_proxy_repository_name.py
--rw-r--r--   0        0        0      132 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_pypi_group.py
--rw-r--r--   0        0        0      259 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_pypi_group_repository_name.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_pypi_hosted.py
--rw-r--r--   0        0        0      262 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_pypi_hosted_repository_name.py
--rw-r--r--   0        0        0      132 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_pypi_proxy.py
--rw-r--r--   0        0        0      259 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_pypi_proxy_repository_name.py
--rw-r--r--   0        0        0      126 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_r_group.py
--rw-r--r--   0        0        0      250 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_r_group_repository_name.py
--rw-r--r--   0        0        0      128 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_r_hosted.py
--rw-r--r--   0        0        0      253 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_r_hosted_repository_name.py
--rw-r--r--   0        0        0      126 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_r_proxy.py
--rw-r--r--   0        0        0      250 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_r_proxy_repository_name.py
--rw-r--r--   0        0        0      130 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_raw_group.py
--rw-r--r--   0        0        0      256 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_raw_group_repository_name.py
--rw-r--r--   0        0        0      132 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_raw_hosted.py
--rw-r--r--   0        0        0      259 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_raw_hosted_repository_name.py
--rw-r--r--   0        0        0      130 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_raw_proxy.py
--rw-r--r--   0        0        0      256 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_raw_proxy_repository_name.py
--rw-r--r--   0        0        0      237 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_repository_name.py
--rw-r--r--   0        0        0      286 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_repository_name_health_check.py
--rw-r--r--   0        0        0      183 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_repository_name_invalidate_cache.py
--rw-r--r--   0        0        0      177 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_repository_name_rebuild_index.py
--rw-r--r--   0        0        0      140 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_rubygems_group.py
--rw-r--r--   0        0        0      271 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_rubygems_group_repository_name.py
--rw-r--r--   0        0        0      142 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_rubygems_hosted.py
--rw-r--r--   0        0        0      292 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_rubygems_hosted_repository_name.py
--rw-r--r--   0        0        0      140 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_rubygems_proxy.py
--rw-r--r--   0        0        0      271 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_rubygems_proxy_repository_name.py
--rw-r--r--   0        0        0      130 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_yum_group.py
--rw-r--r--   0        0        0      256 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_yum_group_repository_name.py
--rw-r--r--   0        0        0      132 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_yum_hosted.py
--rw-r--r--   0        0        0      259 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_yum_hosted_repository_name.py
--rw-r--r--   0        0        0      130 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_yum_proxy.py
--rw-r--r--   0        0        0      256 2023-05-26 16:01:04.893693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repositories_yum_proxy_repository_name.py
--rw-r--r--   0        0        0      122 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_repository_settings.py
--rw-r--r--   0        0        0      187 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_routing_rules.py
--rw-r--r--   0        0        0      286 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_routing_rules_name.py
--rw-r--r--   0        0        0      167 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_script.py
--rw-r--r--   0        0        0      259 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_script_name.py
--rw-r--r--   0        0        0      116 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_script_name_run.py
--rw-r--r--   0        0        0       97 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_search.py
--rw-r--r--   0        0        0      110 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_search_assets.py
--rw-r--r--   0        0        0      127 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_search_assets_download.py
--rw-r--r--   0        0        0      199 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_anonymous.py
--rw-r--r--   0        0        0      216 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_atlassian_crowd.py
--rw-r--r--   0        0        0      156 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_atlassian_crowd_clear_cache.py
--rw-r--r--   0        0        0      177 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_atlassian_crowd_verify_connection.py
--rw-r--r--   0        0        0      225 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_content_selectors.py
--rw-r--r--   0        0        0      337 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_content_selectors_name.py
--rw-r--r--   0        0        0      108 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_jwt.py
--rw-r--r--   0        0        0      187 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_ldap.py
--rw-r--r--   0        0        0      137 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_ldap_change_order.py
--rw-r--r--   0        0        0      286 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_ldap_name.py
--rw-r--r--   0        0        0      122 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges.py
--rw-r--r--   0        0        0      148 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_application.py
--rw-r--r--   0        0        0      182 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_application_privilege_name.py
--rw-r--r--   0        0        0      254 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_privilege_name.py
--rw-r--r--   0        0        0      157 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_repository_admin.py
--rw-r--r--   0        0        0      191 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_repository_admin_privilege_name.py
--rw-r--r--   0        0        0      187 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_repository_content_selector.py
--rw-r--r--   0        0        0      212 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_repository_content_selector_privilege_name.py
--rw-r--r--   0        0        0      155 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_repository_view.py
--rw-r--r--   0        0        0      189 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_repository_view_privilege_name.py
--rw-r--r--   0        0        0      138 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_script.py
--rw-r--r--   0        0        0      163 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_script_privilege_name.py
--rw-r--r--   0        0        0      142 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_wildcard.py
--rw-r--r--   0        0        0      167 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_privileges_wildcard_privilege_name.py
--rw-r--r--   0        0        0      210 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_realms_active.py
--rw-r--r--   0        0        0      133 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_realms_available.py
--rw-r--r--   0        0        0      190 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_roles.py
--rw-r--r--   0        0        0      282 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_roles_id.py
--rw-r--r--   0        0        0      267 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_saml.py
--rw-r--r--   0        0        0      127 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_saml_metadata.py
--rw-r--r--   0        0        0      117 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_saml_pem.py
--rw-r--r--   0        0        0      108 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_ssl.py
--rw-r--r--   0        0        0      216 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_ssl_truststore.py
--rw-r--r--   0        0        0      143 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_ssl_truststore_id.py
--rw-r--r--   0        0        0      125 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_user_sources.py
--rw-r--r--   0        0        0      294 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_user_tokens.py
--rw-r--r--   0        0        0      190 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_users.py
--rw-r--r--   0        0        0      218 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_users_user_id.py
--rw-r--r--   0        0        0      156 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_users_user_id_change_password.py
--rw-r--r--   0        0        0      186 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_security_users_user_id_realm_user_token_reset.py
--rw-r--r--   0        0        0      115 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_staging_delete.py
--rw-r--r--   0        0        0      134 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_staging_move_destination.py
--rw-r--r--   0        0        0       97 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_status.py
--rw-r--r--   0        0        0      108 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_status_check.py
--rw-r--r--   0        0        0      114 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_status_writable.py
--rw-r--r--   0        0        0      123 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_support_supportzip.py
--rw-r--r--   0        0        0      131 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_support_supportzippath.py
--rw-r--r--   0        0        0      274 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_system_license.py
--rw-r--r--   0        0        0      161 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_tags.py
--rw-r--r--   0        0        0      224 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_tags_associate_tag_name.py
--rw-r--r--   0        0        0      251 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_tags_name.py
--rw-r--r--   0        0        0       95 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_tasks.py
--rw-r--r--   0        0        0      100 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_tasks_id.py
--rw-r--r--   0        0        0      110 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_tasks_id_run.py
--rw-r--r--   0        0        0      112 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/paths/v1_tasks_id_stop.py
--rw-r--r--   0        0        0     6299 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tag_to_api.py
--rw-r--r--   0        0        0     1682 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/__init__.py
--rw-r--r--   0        0        0      691 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/assets_api.py
--rw-r--r--   0        0        0      587 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/azure_blob_store_api.py
--rw-r--r--   0        0        0     2077 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/blob_store_api.py
--rw-r--r--   0        0        0      815 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/components_api.py
--rw-r--r--   0        0        0     1054 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/content_selectors_api.py
--rw-r--r--   0        0        0      849 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/email_api.py
--rw-r--r--   0        0        0      621 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/formats_api.py
--rw-r--r--   0        0        0      693 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/lifecycle_api.py
--rw-r--r--   0        0        0      889 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/manage_iq_server_configuration_api.py
--rw-r--r--   0        0        0      734 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/product_licensing_api.py
--rw-r--r--   0        0        0      769 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/read_only_api.py
--rw-r--r--   0        0        0     1110 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/replication_api.py
--rw-r--r--   0        0        0    15722 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/repository_management_api.py
--rw-r--r--   0        0        0      936 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/routing_rules_api.py
--rw-r--r--   0        0        0      852 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/script_api.py
--rw-r--r--   0        0        0      723 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/search_api.py
--rw-r--r--   0        0        0      902 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_atlassian_crowd_api.py
--rw-r--r--   0        0        0      895 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_certificates_api.py
--rw-r--r--   0        0        0      640 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_anonymous_access_api.py
--rw-r--r--   0        0        0      575 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_api.py
--rw-r--r--   0        0        0      563 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_jwt_api.py
--rw-r--r--   0        0        0     1028 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_ldap_api.py
--rw-r--r--   0        0        0     2262 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_privileges_api.py
--rw-r--r--   0        0        0      765 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_realms_api.py
--rw-r--r--   0        0        0      854 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_roles_api.py
--rw-r--r--   0        0        0      993 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_saml_api.py
--rw-r--r--   0        0        0      779 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_user_tokens_api.py
--rw-r--r--   0        0        0     1031 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_users_api.py
--rw-r--r--   0        0        0      620 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/staging_api.py
--rw-r--r--   0        0        0      717 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/status_api.py
--rw-r--r--   0        0        0      648 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/support_api.py
--rw-r--r--   0        0        0      965 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/tags_api.py
--rw-r--r--   0        0        0      734 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/tasks_api.py
--rw-r--r--   0        0        0    15433 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/configuration.py
--rw-r--r--   0        0        0     4515 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/exceptions.py
--rw-r--r--   0        0        0      343 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/__init__.py
--rw-r--r--   0        0        0     6054 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/abstract_api_repository.py
--rw-r--r--   0        0        0     5015 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/abstract_api_repository.pyi
--rw-r--r--   0        0        0     4164 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/anonymous_access_settings_xo.py
--rw-r--r--   0        0        0     3552 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/anonymous_access_settings_xo.pyi
--rw-r--r--   0        0        0    10633 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_certificate.py
--rw-r--r--   0        0        0     9255 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_certificate.pyi
--rw-r--r--   0        0        0     8568 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_create_user.py
--rw-r--r--   0        0        0     7129 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_create_user.pyi
--rw-r--r--   0        0        0    10633 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_email_configuration.py
--rw-r--r--   0        0        0     9191 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_email_configuration.pyi
--rw-r--r--   0        0        0     3516 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_email_validation.py
--rw-r--r--   0        0        0     2994 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_email_validation.pyi
--rw-r--r--   0        0        0     8387 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_license_details_xo.py
--rw-r--r--   0        0        0     7235 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_license_details_xo.pyi
--rw-r--r--   0        0        0     4957 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege.py
--rw-r--r--   0        0        0     4101 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege.pyi
--rw-r--r--   0        0        0     7909 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_application_request.py
--rw-r--r--   0        0        0     6540 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_application_request.pyi
--rw-r--r--   0        0        0     8564 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_admin_request.py
--rw-r--r--   0        0        0     7105 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_admin_request.pyi
--rw-r--r--   0        0        0     9296 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_content_selector_request.py
--rw-r--r--   0        0        0     7747 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_content_selector_request.pyi
--rw-r--r--   0        0        0     8562 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_view_request.py
--rw-r--r--   0        0        0     7103 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_view_request.pyi
--rw-r--r--   0        0        0     7951 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_script_request.py
--rw-r--r--   0        0        0     6582 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_script_request.pyi
--rw-r--r--   0        0        0     4402 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_wildcard_request.py
--rw-r--r--   0        0        0     3637 2023-05-26 16:01:04.897693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_wildcard_request.pyi
--rw-r--r--   0        0        0    10951 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_user.py
--rw-r--r--   0        0        0     9032 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_user.pyi
--rw-r--r--   0        0        0     3391 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_user_source.py
--rw-r--r--   0        0        0     2891 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_user_source.pyi
--rw-r--r--   0        0        0     7650 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_api_repository.py
--rw-r--r--   0        0        0     6647 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_api_repository.pyi
--rw-r--r--   0        0        0     2862 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_repositories_attributes.py
--rw-r--r--   0        0        0     2578 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_repositories_attributes.pyi
--rw-r--r--   0        0        0     7672 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_repository_api_request.py
--rw-r--r--   0        0        0     6658 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     9725 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_api_repository.py
--rw-r--r--   0        0        0     8498 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_api_repository.pyi
--rw-r--r--   0        0        0     3620 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_repositories_attributes.py
--rw-r--r--   0        0        0     3090 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_repositories_attributes.pyi
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_repository_api_request.py
--rw-r--r--   0        0        0     8457 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     3594 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_signing_repositories_attributes.py
--rw-r--r--   0        0        0     3072 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_signing_repositories_attributes.pyi
--rw-r--r--   0        0        0    11166 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/asset_xo.py
--rw-r--r--   0        0        0     9654 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/asset_xo.pyi
--rw-r--r--   0        0        0     4550 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_authentication.py
--rw-r--r--   0        0        0     3858 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_authentication.pyi
--rw-r--r--   0        0        0     4922 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_bucket_configuration.py
--rw-r--r--   0        0        0     4167 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_bucket_configuration.pyi
--rw-r--r--   0        0        0     4732 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_model.py
--rw-r--r--   0        0        0     4129 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_model.pyi
--rw-r--r--   0        0        0     5079 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_connection_xo.py
--rw-r--r--   0        0        0     4377 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_connection_xo.pyi
--rw-r--r--   0        0        0     4087 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/base_tag_xo.py
--rw-r--r--   0        0        0     3692 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/base_tag_xo.pyi
--rw-r--r--   0        0        0     4135 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/blob_store_api_soft_quota.py
--rw-r--r--   0        0        0     3450 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/blob_store_api_soft_quota.pyi
--rw-r--r--   0        0        0     4275 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/blob_store_quota_result_xo.py
--rw-r--r--   0        0        0     3663 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/blob_store_quota_result_xo.pyi
--rw-r--r--   0        0        0     2993 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_attributes.py
--rw-r--r--   0        0        0     2701 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_attributes.pyi
--rw-r--r--   0        0        0     5145 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_group_repository_api_request.py
--rw-r--r--   0        0        0     4329 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6044 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5168 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     9646 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_proxy_api_repository.py
--rw-r--r--   0        0        0     8428 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_proxy_api_repository.pyi
--rw-r--r--   0        0        0     9616 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_proxy_repository_api_request.py
--rw-r--r--   0        0        0     8387 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     3903 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/cleanup_policy_attributes.py
--rw-r--r--   0        0        0     3359 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/cleanup_policy_attributes.pyi
--rw-r--r--   0        0        0     8945 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/cocoapods_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7776 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/cocoapods_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     2975 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/component_attributes.py
--rw-r--r--   0        0        0     2673 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/component_attributes.pyi
--rw-r--r--   0        0        0     7191 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/component_xo.py
--rw-r--r--   0        0        0     6365 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/component_xo.pyi
--rw-r--r--   0        0        0     8937 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/conan_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7768 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/conan_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     8937 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/conda_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7768 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/conda_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     4449 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_create_request.py
--rw-r--r--   0        0        0     3684 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_create_request.pyi
--rw-r--r--   0        0        0     5195 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_response.py
--rw-r--r--   0        0        0     4418 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_response.pyi
--rw-r--r--   0        0        0     3644 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_update_request.py
--rw-r--r--   0        0        0     3122 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_update_request.pyi
--rw-r--r--   0        0        0    26439 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/create_ldap_server_xo.py
--rw-r--r--   0        0        0    22642 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/create_ldap_server_xo.pyi
--rw-r--r--   0        0        0     7213 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/crowd_api_xo.py
--rw-r--r--   0        0        0     6163 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/crowd_api_xo.pyi
--rw-r--r--   0        0        0     5665 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_attributes.py
--rw-r--r--   0        0        0     4854 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_attributes.pyi
--rw-r--r--   0        0        0     5849 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_group_api_repository.py
--rw-r--r--   0        0        0     4984 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_group_api_repository.pyi
--rw-r--r--   0        0        0     5871 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_group_repository_api_request.py
--rw-r--r--   0        0        0     4995 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6699 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_api_repository.py
--rw-r--r--   0        0        0     5774 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_api_repository.pyi
--rw-r--r--   0        0        0     6779 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5834 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     5964 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_storage_attributes.py
--rw-r--r--   0        0        0     5130 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_storage_attributes.pyi
--rw-r--r--   0        0        0    10420 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_api_repository.py
--rw-r--r--   0        0        0     9142 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_api_repository.pyi
--rw-r--r--   0        0        0     6830 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_attributes.py
--rw-r--r--   0        0        0     5759 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_attributes.pyi
--rw-r--r--   0        0        0    10390 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_repository_api_request.py
--rw-r--r--   0        0        0     9101 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     4237 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_create_request.py
--rw-r--r--   0        0        0     3654 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_create_request.pyi
--rw-r--r--   0        0        0     3652 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_model.py
--rw-r--r--   0        0        0     3159 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_model.pyi
--rw-r--r--   0        0        0     3668 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_update_request.py
--rw-r--r--   0        0        0     3175 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_update_request.pyi
--rw-r--r--   0        0        0     7138 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/generic_blob_store_api_response.py
--rw-r--r--   0        0        0     6158 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/generic_blob_store_api_response.pyi
--rw-r--r--   0        0        0     6046 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/git_lfs_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5170 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/git_lfs_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     5147 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/golang_group_repository_api_request.py
--rw-r--r--   0        0        0     4331 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/golang_group_repository_api_request.pyi
--rw-r--r--   0        0        0     8939 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/golang_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7770 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/golang_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     3887 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_attributes.py
--rw-r--r--   0        0        0     3343 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_attributes.pyi
--rw-r--r--   0        0        0     6475 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_create_request.py
--rw-r--r--   0        0        0     5437 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_create_request.pyi
--rw-r--r--   0        0        0     5890 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_model.py
--rw-r--r--   0        0        0     4942 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_model.pyi
--rw-r--r--   0        0        0     6465 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_response.py
--rw-r--r--   0        0        0     5427 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_response.pyi
--rw-r--r--   0        0        0     5906 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_update_request.py
--rw-r--r--   0        0        0     4958 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_update_request.pyi
--rw-r--r--   0        0        0     4746 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_deploy_attributes.py
--rw-r--r--   0        0        0     3964 2023-05-26 16:01:04.901693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_deploy_attributes.pyi
--rw-r--r--   0        0        0     6042 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/helm_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5166 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/helm_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     8935 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/helm_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7766 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/helm_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     5277 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/hosted_storage_attributes.py
--rw-r--r--   0        0        0     4533 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/hosted_storage_attributes.pyi
--rw-r--r--   0        0        0     5542 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_attributes.py
--rw-r--r--   0        0        0     4785 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_attributes.pyi
--rw-r--r--   0        0        0     5730 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_attributes_with_preemptive_auth.py
--rw-r--r--   0        0        0     4921 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_attributes_with_preemptive_auth.pyi
--rw-r--r--   0        0        0     6820 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_attributes.py
--rw-r--r--   0        0        0     5779 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_attributes.pyi
--rw-r--r--   0        0        0     5880 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_authentication_attributes.py
--rw-r--r--   0        0        0     5006 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_authentication_attributes.pyi
--rw-r--r--   0        0        0     6557 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_authentication_attributes_with_preemptive.py
--rw-r--r--   0        0        0     5593 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_authentication_attributes_with_preemptive.pyi
--rw-r--r--   0        0        0     3532 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/iq_connection_verification_xo.py
--rw-r--r--   0        0        0     3010 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/iq_connection_verification_xo.pyi
--rw-r--r--   0        0        0     8859 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/iq_connection_xo.py
--rw-r--r--   0        0        0     7568 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/iq_connection_xo.pyi
--rw-r--r--   0        0        0     5927 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_attributes.py
--rw-r--r--   0        0        0     5021 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_attributes.pyi
--rw-r--r--   0        0        0     5145 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_group_repository_api_request.py
--rw-r--r--   0        0        0     4329 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6677 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_hosted_api_repository.py
--rw-r--r--   0        0        0     5752 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_hosted_api_repository.pyi
--rw-r--r--   0        0        0     6699 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5763 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     9622 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_proxy_api_repository.py
--rw-r--r--   0        0        0     8404 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_proxy_api_repository.pyi
--rw-r--r--   0        0        0     9748 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_proxy_repository_api_request.py
--rw-r--r--   0        0        0     8510 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     3685 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/negative_cache_attributes.py
--rw-r--r--   0        0        0     3132 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/negative_cache_attributes.pyi
--rw-r--r--   0        0        0     3924 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_attributes.py
--rw-r--r--   0        0        0     3383 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_attributes.pyi
--rw-r--r--   0        0        0     5190 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_group_repository_api_request.py
--rw-r--r--   0        0        0     4374 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6040 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5164 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     9594 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_proxy_api_repository.py
--rw-r--r--   0        0        0     8390 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_proxy_api_repository.pyi
--rw-r--r--   0        0        0     9564 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_proxy_repository_api_request.py
--rw-r--r--   0        0        0     8349 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     4218 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_attributes.py
--rw-r--r--   0        0        0     3592 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_attributes.pyi
--rw-r--r--   0        0        0     5145 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_group_repository_api_request.py
--rw-r--r--   0        0        0     4329 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6044 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5168 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     9682 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_proxy_api_repository.py
--rw-r--r--   0        0        0     8464 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_proxy_api_repository.pyi
--rw-r--r--   0        0        0     9652 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_proxy_repository_api_request.py
--rw-r--r--   0        0        0     8423 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     8931 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/p2_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7762 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/p2_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     4780 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page.py
--rw-r--r--   0        0        0     3934 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page.pyi
--rw-r--r--   0        0        0     4392 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_asset_xo.py
--rw-r--r--   0        0        0     3995 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_asset_xo.pyi
--rw-r--r--   0        0        0     4474 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_component_xo.py
--rw-r--r--   0        0        0     4031 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_component_xo.pyi
--rw-r--r--   0        0        0     4374 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_tag_xo.py
--rw-r--r--   0        0        0     3977 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_tag_xo.pyi
--rw-r--r--   0        0        0     4383 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_task_xo.py
--rw-r--r--   0        0        0     3986 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_task_xo.pyi
--rw-r--r--   0        0        0     4492 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/proxy_attributes.py
--rw-r--r--   0        0        0     3837 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/proxy_attributes.pyi
--rw-r--r--   0        0        0     5143 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_group_repository_api_request.py
--rw-r--r--   0        0        0     4327 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6042 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5166 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     8935 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7766 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     5137 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_group_repository_api_request.py
--rw-r--r--   0        0        0     4321 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6036 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5160 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     8929 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7760 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     3358 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_attributes.py
--rw-r--r--   0        0        0     2984 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_attributes.pyi
--rw-r--r--   0        0        0     5772 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_group_repository_api_request.py
--rw-r--r--   0        0        0     4910 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6671 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5749 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     9564 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_proxy_repository_api_request.py
--rw-r--r--   0        0        0     8349 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0    26852 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/read_ldap_server_xo.py
--rw-r--r--   0        0        0    22998 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/read_ldap_server_xo.pyi
--rw-r--r--   0        0        0     4298 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/read_only_state.py
--rw-r--r--   0        0        0     3686 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/read_only_state.pyi
--rw-r--r--   0        0        0     3385 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/realm_api_xo.py
--rw-r--r--   0        0        0     2885 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/realm_api_xo.pyi
--rw-r--r--   0        0        0     3900 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_attributes.py
--rw-r--r--   0        0        0     3370 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_attributes.pyi
--rw-r--r--   0        0        0    11065 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_connection_xo.py
--rw-r--r--   0        0        0     9543 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_connection_xo.pyi
--rw-r--r--   0        0        0     4925 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_enable_xo.py
--rw-r--r--   0        0        0     4283 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_enable_xo.pyi
--rw-r--r--   0        0        0     6509 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/repository_xo.py
--rw-r--r--   0        0        0     5627 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/repository_xo.pyi
--rw-r--r--   0        0        0     7892 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/result.py
--rw-r--r--   0        0        0     6851 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/result.pyi
--rw-r--r--   0        0        0     7494 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/role_xo_request.py
--rw-r--r--   0        0        0     6123 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/role_xo_request.pyi
--rw-r--r--   0        0        0     8714 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/role_xo_response.py
--rw-r--r--   0        0        0     7163 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/role_xo_response.pyi
--rw-r--r--   0        0        0     6454 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/routing_rule_xo.py
--rw-r--r--   0        0        0     5260 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/routing_rule_xo.pyi
--rw-r--r--   0        0        0     5151 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_group_repository_api_request.py
--rw-r--r--   0        0        0     4335 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6050 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5174 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     8943 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_proxy_repository_api_request.py
--rw-r--r--   0        0        0     7774 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     5166 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_advanced_bucket_connection.py
--rw-r--r--   0        0        0     4427 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_advanced_bucket_connection.pyi
--rw-r--r--   0        0        0     4833 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket.py
--rw-r--r--   0        0        0     4089 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket.pyi
--rw-r--r--   0        0        0     5896 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket_configuration.py
--rw-r--r--   0        0        0     5200 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket_configuration.pyi
--rw-r--r--   0        0        0     4945 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket_security.py
--rw-r--r--   0        0        0     4243 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket_security.pyi
--rw-r--r--   0        0        0     4260 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_encryption.py
--rw-r--r--   0        0        0     3599 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_encryption.pyi
--rw-r--r--   0        0        0     5271 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_model.py
--rw-r--r--   0        0        0     4578 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_model.pyi
--rw-r--r--   0        0        0     9042 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/saml_configuration_xo.py
--rw-r--r--   0        0        0     7871 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/saml_configuration_xo.pyi
--rw-r--r--   0        0        0     3467 2023-05-26 16:01:04.905693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/script_result_xo.py
--rw-r--r--   0        0        0     2945 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/script_result_xo.pyi
--rw-r--r--   0        0        0     4273 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/script_xo.py
--rw-r--r--   0        0        0     3508 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/script_xo.pyi
--rw-r--r--   0        0        0     5186 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_group_deploy_repository.py
--rw-r--r--   0        0        0     4381 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_group_deploy_repository.pyi
--rw-r--r--   0        0        0     5125 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_group_repository.py
--rw-r--r--   0        0        0     4320 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_group_repository.pyi
--rw-r--r--   0        0        0     6024 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_hosted_repository.py
--rw-r--r--   0        0        0     5159 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_hosted_repository.pyi
--rw-r--r--   0        0        0     8969 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_proxy_repository.py
--rw-r--r--   0        0        0     7811 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_proxy_repository.pyi
--rw-r--r--   0        0        0     5552 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/stack_trace_element.py
--rw-r--r--   0        0        0     4760 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/stack_trace_element.pyi
--rw-r--r--   0        0        0     3975 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/storage_attributes.py
--rw-r--r--   0        0        0     3445 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/storage_attributes.pyi
--rw-r--r--   0        0        0     9980 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/support_zip_generator_request.py
--rw-r--r--   0        0        0     8602 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/support_zip_generator_request.pyi
--rw-r--r--   0        0        0     4642 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/support_zip_xo.py
--rw-r--r--   0        0        0     3940 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/support_zip_xo.pyi
--rw-r--r--   0        0        0     6508 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/tag_xo.py
--rw-r--r--   0        0        0     5462 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/tag_xo.pyi
--rw-r--r--   0        0        0     7159 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/task_xo.py
--rw-r--r--   0        0        0     6119 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/task_xo.pyi
--rw-r--r--   0        0        0     7206 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/throwable.py
--rw-r--r--   0        0        0     6591 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/throwable.pyi
--rw-r--r--   0        0        0    26960 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/update_ldap_server_xo.py
--rw-r--r--   0        0        0    23095 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/update_ldap_server_xo.pyi
--rw-r--r--   0        0        0     6835 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/upload_definition_xo.py
--rw-r--r--   0        0        0     6241 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/upload_definition_xo.pyi
--rw-r--r--   0        0        0     5324 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/upload_field_definition_xo.py
--rw-r--r--   0        0        0     4532 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/upload_field_definition_xo.pyi
--rw-r--r--   0        0        0     3622 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/user_tokens_api_model.py
--rw-r--r--   0        0        0     3100 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/user_tokens_api_model.pyi
--rw-r--r--   0        0        0     4373 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_attributes.py
--rw-r--r--   0        0        0     3664 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_attributes.pyi
--rw-r--r--   0        0        0     6022 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_group_repository_api_request.py
--rw-r--r--   0        0        0     5115 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_group_repository_api_request.pyi
--rw-r--r--   0        0        0     6605 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_hosted_api_repository.py
--rw-r--r--   0        0        0     5708 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_hosted_api_repository.pyi
--rw-r--r--   0        0        0     6627 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_hosted_repository_api_request.py
--rw-r--r--   0        0        0     5719 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_hosted_repository_api_request.pyi
--rw-r--r--   0        0        0     8741 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_proxy_repository_api_request.py
--rw-r--r--   0        0        0     8554 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_proxy_repository_api_request.pyi
--rw-r--r--   0        0        0     3072 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_signing_repositories_attributes.py
--rw-r--r--   0        0        0     3072 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_signing_repositories_attributes.pyi
--rw-r--r--   0        0        0    13448 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/models/__init__.py
--rw-r--r--   0        0        0    13274 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/__init__.py
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/__init__.py
--rw-r--r--   0        0        0     6485 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/get.py
--rw-r--r--   0        0        0     6371 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/get.pyi
--rw-r--r--   0        0        0    10757 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/post.py
--rw-r--r--   0        0        0    10613 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/post.pyi
--rw-r--r--   0        0        0      341 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/__init__.py
--rw-r--r--   0        0        0     9022 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/delete.py
--rw-r--r--   0        0        0     8847 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/delete.pyi
--rw-r--r--   0        0        0     8970 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/get.py
--rw-r--r--   0        0        0     8795 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/get.pyi
--rw-r--r--   0        0        0    13200 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/put.py
--rw-r--r--   0        0        0    13026 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/put.pyi
--rw-r--r--   0        0        0      357 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_enable/__init__.py
--rw-r--r--   0        0        0    11023 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_enable/put.py
--rw-r--r--   0        0        0    10849 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_enable/put.pyi
--rw-r--r--   0        0        0      389 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/__init__.py
--rw-r--r--   0        0        0     9106 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/delete.py
--rw-r--r--   0        0        0     8931 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/delete.pyi
--rw-r--r--   0        0        0      295 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets/__init__.py
--rw-r--r--   0        0        0    10679 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets/get.py
--rw-r--r--   0        0        0    10565 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets/get.pyi
--rw-r--r--   0        0        0      301 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/__init__.py
--rw-r--r--   0        0        0     8763 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/delete.py
--rw-r--r--   0        0        0     8618 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/delete.pyi
--rw-r--r--   0        0        0    10408 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/get.py
--rw-r--r--   0        0        0    10264 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/get.pyi
--rw-r--r--   0        0        0      342 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_azureblobstore_test_connection/__init__.py
--rw-r--r--   0        0        0    10907 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_azureblobstore_test_connection/post.py
--rw-r--r--   0        0        0    10763 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_azureblobstore_test_connection/post.pyi
--rw-r--r--   0        0        0      303 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores/__init__.py
--rw-r--r--   0        0        0     8340 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores/get.py
--rw-r--r--   0        0        0     8287 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores/get.pyi
--rw-r--r--   0        0        0      315 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure/__init__.py
--rw-r--r--   0        0        0    10603 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure/post.py
--rw-r--r--   0        0        0    10489 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure/post.pyi
--rw-r--r--   0        0        0      325 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/__init__.py
--rw-r--r--   0        0        0    10498 2023-05-26 16:01:04.909693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/get.py
--rw-r--r--   0        0        0    10354 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/get.pyi
--rw-r--r--   0        0        0    13068 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/put.py
--rw-r--r--   0        0        0    12924 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/put.pyi
--rw-r--r--   0        0        0      313 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file/__init__.py
--rw-r--r--   0        0        0    10395 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file/post.py
--rw-r--r--   0        0        0    10302 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file/post.pyi
--rw-r--r--   0        0        0      323 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/__init__.py
--rw-r--r--   0        0        0    10401 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/get.py
--rw-r--r--   0        0        0    10287 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/get.pyi
--rw-r--r--   0        0        0    12860 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/put.py
--rw-r--r--   0        0        0    12737 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/put.pyi
--rw-r--r--   0        0        0      315 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group/__init__.py
--rw-r--r--   0        0        0    10412 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group/post.py
--rw-r--r--   0        0        0    10319 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group/post.pyi
--rw-r--r--   0        0        0      385 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/__init__.py
--rw-r--r--   0        0        0    10709 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/post.py
--rw-r--r--   0        0        0    10595 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/post.pyi
--rw-r--r--   0        0        0      325 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/__init__.py
--rw-r--r--   0        0        0    10416 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/get.py
--rw-r--r--   0        0        0    10302 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/get.pyi
--rw-r--r--   0        0        0    12877 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/put.py
--rw-r--r--   0        0        0    12754 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/put.pyi
--rw-r--r--   0        0        0      313 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name/__init__.py
--rw-r--r--   0        0        0     8260 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name/delete.py
--rw-r--r--   0        0        0     8197 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name/delete.pyi
--rw-r--r--   0        0        0      338 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name_quota_status/__init__.py
--rw-r--r--   0        0        0     9596 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name_quota_status/get.py
--rw-r--r--   0        0        0     9542 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name_quota_status/get.pyi
--rw-r--r--   0        0        0      309 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3/__init__.py
--rw-r--r--   0        0        0    10578 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3/post.py
--rw-r--r--   0        0        0    10464 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3/post.pyi
--rw-r--r--   0        0        0      319 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/__init__.py
--rw-r--r--   0        0        0    10474 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/get.py
--rw-r--r--   0        0        0    10330 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/get.pyi
--rw-r--r--   0        0        0    13043 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/put.py
--rw-r--r--   0        0        0    12899 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/put.pyi
--rw-r--r--   0        0        0      303 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/__init__.py
--rw-r--r--   0        0        0    10739 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/get.py
--rw-r--r--   0        0        0    10625 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/get.pyi
--rw-r--r--   0        0        0    12630 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/post.py
--rw-r--r--   0        0        0    12546 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/post.pyi
--rw-r--r--   0        0        0      309 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/__init__.py
--rw-r--r--   0        0        0     8811 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/delete.py
--rw-r--r--   0        0        0     8666 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/delete.pyi
--rw-r--r--   0        0        0    10468 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/get.py
--rw-r--r--   0        0        0    10324 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/get.pyi
--rw-r--r--   0        0        0      293 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/__init__.py
--rw-r--r--   0        0        0     6121 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/delete.py
--rw-r--r--   0        0        0     6067 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/delete.pyi
--rw-r--r--   0        0        0     8036 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/get.py
--rw-r--r--   0        0        0     7952 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/get.pyi
--rw-r--r--   0        0        0    10009 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/put.py
--rw-r--r--   0        0        0     9895 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/put.pyi
--rw-r--r--   0        0        0      307 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email_verify/__init__.py
--rw-r--r--   0        0        0    11555 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email_verify/post.py
--rw-r--r--   0        0        0    11471 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email_verify/post.pyi
--rw-r--r--   0        0        0      336 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_format_upload_specs/__init__.py
--rw-r--r--   0        0        0     9522 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_format_upload_specs/get.py
--rw-r--r--   0        0        0     9468 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_format_upload_specs/get.pyi
--rw-r--r--   0        0        0      322 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_upload_specs/__init__.py
--rw-r--r--   0        0        0     8180 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_upload_specs/get.py
--rw-r--r--   0        0        0     8127 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_upload_specs/get.pyi
--rw-r--r--   0        0        0      287 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/__init__.py
--rw-r--r--   0        0        0     5991 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/get.py
--rw-r--r--   0        0        0     5937 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/get.pyi
--rw-r--r--   0        0        0    10025 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/put.py
--rw-r--r--   0        0        0     9971 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/put.pyi
--rw-r--r--   0        0        0      303 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_disable/__init__.py
--rw-r--r--   0        0        0     6198 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_disable/post.py
--rw-r--r--   0        0        0     6114 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_disable/post.pyi
--rw-r--r--   0        0        0      301 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_enable/__init__.py
--rw-r--r--   0        0        0     6186 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_enable/post.py
--rw-r--r--   0        0        0     6102 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_enable/post.pyi
--rw-r--r--   0        0        0      322 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_verify_connection/__init__.py
--rw-r--r--   0        0        0     5997 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_verify_connection/post.py
--rw-r--r--   0        0        0     5943 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_verify_connection/post.pyi
--rw-r--r--   0        0        0      315 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_bounce/__init__.py
--rw-r--r--   0        0        0    10009 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_bounce/put.py
--rw-r--r--   0        0        0     9946 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_bounce/put.pyi
--rw-r--r--   0        0        0      313 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/__init__.py
--rw-r--r--   0        0        0     7474 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/get.py
--rw-r--r--   0        0        0     7419 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/get.pyi
--rw-r--r--   0        0        0    10052 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/put.py
--rw-r--r--   0        0        0     9989 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/put.pyi
--rw-r--r--   0        0        0      300 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only/__init__.py
--rw-r--r--   0        0        0     7485 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only/get.py
--rw-r--r--   0        0        0     7431 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only/get.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_force_release/__init__.py
--rw-r--r--   0        0        0     6528 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_force_release/post.py
--rw-r--r--   0        0        0     6414 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_force_release/post.pyi
--rw-r--r--   0        0        0      314 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_freeze/__init__.py
--rw-r--r--   0        0        0     6442 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_freeze/post.py
--rw-r--r--   0        0        0     6328 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_freeze/post.pyi
--rw-r--r--   0        0        0      316 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_release/__init__.py
--rw-r--r--   0        0        0     6454 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_release/post.py
--rw-r--r--   0        0        0     6340 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_release/post.pyi
--rw-r--r--   0        0        0      307 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories/__init__.py
--rw-r--r--   0        0        0     8241 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories/get.py
--rw-r--r--   0        0        0     8188 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories/get.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted/__init__.py
--rw-r--r--   0        0        0    10924 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted/post.py
--rw-r--r--   0        0        0    10771 2023-05-26 16:01:04.913693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted/post.pyi
--rw-r--r--   0        0        0      361 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9675 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9621 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    13151 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12998 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy/__init__.py
--rw-r--r--   0        0        0    10920 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy/post.py
--rw-r--r--   0        0        0    10767 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy/post.pyi
--rw-r--r--   0        0        0      359 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9672 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9618 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    13147 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12994 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group/__init__.py
--rw-r--r--   0        0        0    10653 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group/post.py
--rw-r--r--   0        0        0    10530 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12880 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/put.py
--rw-r--r--   0        0        0    12757 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/put.pyi
--rw-r--r--   0        0        0      333 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted/__init__.py
--rw-r--r--   0        0        0    10657 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted/post.py
--rw-r--r--   0        0        0    10534 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted/post.pyi
--rw-r--r--   0        0        0      365 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12884 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12761 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy/__init__.py
--rw-r--r--   0        0        0    10653 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy/post.py
--rw-r--r--   0        0        0    10530 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9689 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9635 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12880 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12757 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      339 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy/__init__.py
--rw-r--r--   0        0        0    10957 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy/post.py
--rw-r--r--   0        0        0    10804 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy/post.pyi
--rw-r--r--   0        0        0      371 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12896 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12773 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy/__init__.py
--rw-r--r--   0        0        0    10941 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy/post.py
--rw-r--r--   0        0        0    10788 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    13168 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/put.py
--rw-r--r--   0        0        0    13015 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy/__init__.py
--rw-r--r--   0        0        0    10941 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy/post.py
--rw-r--r--   0        0        0    10788 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12880 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12757 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      333 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group/__init__.py
--rw-r--r--   0        0        0    10657 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group/post.py
--rw-r--r--   0        0        0    10534 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group/post.pyi
--rw-r--r--   0        0        0      365 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/get.pyi
--rw-r--r--   0        0        0    13172 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/put.py
--rw-r--r--   0        0        0    13019 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/put.pyi
--rw-r--r--   0        0        0      335 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted/__init__.py
--rw-r--r--   0        0        0    10661 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted/post.py
--rw-r--r--   0        0        0    10538 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted/post.pyi
--rw-r--r--   0        0        0      367 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    13176 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/put.py
--rw-r--r--   0        0        0    13023 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      333 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy/__init__.py
--rw-r--r--   0        0        0    10657 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy/post.py
--rw-r--r--   0        0        0    10534 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy/post.pyi
--rw-r--r--   0        0        0      365 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    13172 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/put.py
--rw-r--r--   0        0        0    13019 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      335 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted/__init__.py
--rw-r--r--   0        0        0    10663 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted/post.py
--rw-r--r--   0        0        0    10540 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted/post.pyi
--rw-r--r--   0        0        0      367 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12890 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12767 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      325 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group/__init__.py
--rw-r--r--   0        0        0    10943 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group/post.py
--rw-r--r--   0        0        0    10790 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group/post.pyi
--rw-r--r--   0        0        0      357 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/get.pyi
--rw-r--r--   0        0        0    13170 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/put.py
--rw-r--r--   0        0        0    13017 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/put.pyi
--rw-r--r--   0        0        0      325 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy/__init__.py
--rw-r--r--   0        0        0    10943 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy/post.py
--rw-r--r--   0        0        0    10790 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy/post.pyi
--rw-r--r--   0        0        0      357 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    13170 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/put.py
--rw-r--r--   0        0        0    13017 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted/__init__.py
--rw-r--r--   0        0        0    10941 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted/post.py
--rw-r--r--   0        0        0    10788 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12880 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12757 2023-05-26 16:01:04.917693 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy/__init__.py
--rw-r--r--   0        0        0    10937 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy/post.py
--rw-r--r--   0        0        0    10784 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy/post.pyi
--rw-r--r--   0        0        0      361 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12876 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12753 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group/__init__.py
--rw-r--r--   0        0        0    10627 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group/post.py
--rw-r--r--   0        0        0    10504 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9681 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/get.py
--rw-r--r--   0        0        0     9627 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12854 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/put.py
--rw-r--r--   0        0        0    12731 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/put.pyi
--rw-r--r--   0        0        0      333 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted/__init__.py
--rw-r--r--   0        0        0    10644 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted/post.py
--rw-r--r--   0        0        0    10521 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted/post.pyi
--rw-r--r--   0        0        0      365 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9681 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9627 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12871 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12748 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy/__init__.py
--rw-r--r--   0        0        0    10640 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy/post.py
--rw-r--r--   0        0        0    10517 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9678 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9624 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12867 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12744 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group/__init__.py
--rw-r--r--   0        0        0    10632 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group/post.py
--rw-r--r--   0        0        0    10509 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group/post.pyi
--rw-r--r--   0        0        0      359 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9709 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/get.py
--rw-r--r--   0        0        0     9646 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12859 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/put.py
--rw-r--r--   0        0        0    12736 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/put.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted/__init__.py
--rw-r--r--   0        0        0    10636 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted/post.py
--rw-r--r--   0        0        0    10513 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted/post.pyi
--rw-r--r--   0        0        0      361 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12863 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12740 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy/__init__.py
--rw-r--r--   0        0        0    10645 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy/post.py
--rw-r--r--   0        0        0    10522 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy/post.pyi
--rw-r--r--   0        0        0      359 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9683 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9629 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12872 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12749 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group/__init__.py
--rw-r--r--   0        0        0    10653 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group/post.py
--rw-r--r--   0        0        0    10530 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12880 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/put.py
--rw-r--r--   0        0        0    12757 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/put.pyi
--rw-r--r--   0        0        0      333 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted/__init__.py
--rw-r--r--   0        0        0    10657 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted/post.py
--rw-r--r--   0        0        0    10534 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted/post.pyi
--rw-r--r--   0        0        0      365 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12884 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12761 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy/__init__.py
--rw-r--r--   0        0        0    10653 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy/post.py
--rw-r--r--   0        0        0    10530 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9689 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9635 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12880 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12757 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      325 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy/__init__.py
--rw-r--r--   0        0        0    10920 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy/post.py
--rw-r--r--   0        0        0    10776 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy/post.pyi
--rw-r--r--   0        0        0      357 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12859 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12745 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group/__init__.py
--rw-r--r--   0        0        0    10649 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group/post.py
--rw-r--r--   0        0        0    10526 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group/post.pyi
--rw-r--r--   0        0        0      361 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12876 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/put.py
--rw-r--r--   0        0        0    12753 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/put.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted/__init__.py
--rw-r--r--   0        0        0    10653 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted/post.py
--rw-r--r--   0        0        0    10530 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted/post.pyi
--rw-r--r--   0        0        0      363 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12880 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12757 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy/__init__.py
--rw-r--r--   0        0        0    10649 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy/post.py
--rw-r--r--   0        0        0    10526 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy/post.pyi
--rw-r--r--   0        0        0      361 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12876 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12753 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      323 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group/__init__.py
--rw-r--r--   0        0        0    10916 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group/post.py
--rw-r--r--   0        0        0    10772 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group/post.pyi
--rw-r--r--   0        0        0      355 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12855 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/put.py
--rw-r--r--   0        0        0    12741 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/put.pyi
--rw-r--r--   0        0        0      325 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted/__init__.py
--rw-r--r--   0        0        0    10920 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted/post.py
--rw-r--r--   0        0        0    10776 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted/post.pyi
--rw-r--r--   0        0        0      357 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.921692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12859 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12745 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      323 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy/__init__.py
--rw-r--r--   0        0        0    10916 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy/post.py
--rw-r--r--   0        0        0    10772 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy/post.pyi
--rw-r--r--   0        0        0      355 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    13143 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12999 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group/__init__.py
--rw-r--r--   0        0        0    10632 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group/post.py
--rw-r--r--   0        0        0    10509 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group/post.pyi
--rw-r--r--   0        0        0      359 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9681 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/get.py
--rw-r--r--   0        0        0     9627 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12859 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/put.py
--rw-r--r--   0        0        0    12736 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/put.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted/__init__.py
--rw-r--r--   0        0        0    10636 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted/post.py
--rw-r--r--   0        0        0    10513 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted/post.pyi
--rw-r--r--   0        0        0      361 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9684 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9630 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12863 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12740 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy/__init__.py
--rw-r--r--   0        0        0    10632 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy/post.py
--rw-r--r--   0        0        0    10509 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy/post.pyi
--rw-r--r--   0        0        0      359 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9681 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9627 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12859 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12736 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      339 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/__init__.py
--rw-r--r--   0        0        0     8914 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/delete.py
--rw-r--r--   0        0        0     8769 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/delete.pyi
--rw-r--r--   0        0        0    10504 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/get.py
--rw-r--r--   0        0        0    10360 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/get.pyi
--rw-r--r--   0        0        0      364 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/__init__.py
--rw-r--r--   0        0        0     9092 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/delete.py
--rw-r--r--   0        0        0     8947 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/delete.pyi
--rw-r--r--   0        0        0     9356 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/post.py
--rw-r--r--   0        0        0     9181 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/post.pyi
--rw-r--r--   0        0        0      372 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/__init__.py
--rw-r--r--   0        0        0     9210 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/post.py
--rw-r--r--   0        0        0     9035 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/post.pyi
--rw-r--r--   0        0        0      366 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/__init__.py
--rw-r--r--   0        0        0     9213 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/post.py
--rw-r--r--   0        0        0     9038 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/post.pyi
--rw-r--r--   0        0        0      337 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group/__init__.py
--rw-r--r--   0        0        0    10666 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group/post.py
--rw-r--r--   0        0        0    10543 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group/post.pyi
--rw-r--r--   0        0        0      369 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12893 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/put.py
--rw-r--r--   0        0        0    12770 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/put.pyi
--rw-r--r--   0        0        0      339 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted/__init__.py
--rw-r--r--   0        0        0    10670 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted/post.py
--rw-r--r--   0        0        0    10547 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted/post.pyi
--rw-r--r--   0        0        0      371 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9695 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9641 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12897 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12774 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      337 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy/__init__.py
--rw-r--r--   0        0        0    10666 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy/post.py
--rw-r--r--   0        0        0    10543 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy/post.pyi
--rw-r--r--   0        0        0      369 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12893 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12770 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group/__init__.py
--rw-r--r--   0        0        0    10645 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group/post.py
--rw-r--r--   0        0        0    10522 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group/post.pyi
--rw-r--r--   0        0        0      359 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/get.pyi
--rw-r--r--   0        0        0    12872 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/put.py
--rw-r--r--   0        0        0    12749 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/put.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted/__init__.py
--rw-r--r--   0        0        0    10649 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted/post.py
--rw-r--r--   0        0        0    10526 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted/post.pyi
--rw-r--r--   0        0        0      361 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/__init__.py
--rw-r--r--   0        0        0     9686 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/get.py
--rw-r--r--   0        0        0     9632 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/get.pyi
--rw-r--r--   0        0        0    12876 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/put.py
--rw-r--r--   0        0        0    12753 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy/__init__.py
--rw-r--r--   0        0        0    10645 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy/post.py
--rw-r--r--   0        0        0    10522 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy/post.pyi
--rw-r--r--   0        0        0      359 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/__init__.py
--rw-r--r--   0        0        0     9692 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/get.py
--rw-r--r--   0        0        0     9638 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/get.pyi
--rw-r--r--   0        0        0    12872 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/put.py
--rw-r--r--   0        0        0    12749 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/put.pyi
--rw-r--r--   0        0        0      321 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repository_settings/__init__.py
--rw-r--r--   0        0        0     8870 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repository_settings/get.py
--rw-r--r--   0        0        0     8757 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repository_settings/get.pyi
--rw-r--r--   0        0        0      308 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/__init__.py
--rw-r--r--   0        0        0     8537 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/get.py
--rw-r--r--   0        0        0     8454 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/get.pyi
--rw-r--r--   0        0        0    10279 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/post.py
--rw-r--r--   0        0        0    10165 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/post.pyi
--rw-r--r--   0        0        0      318 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/__init__.py
--rw-r--r--   0        0        0     8572 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/delete.py
--rw-r--r--   0        0        0     8457 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/delete.pyi
--rw-r--r--   0        0        0    10172 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/get.py
--rw-r--r--   0        0        0    10058 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/get.pyi
--rw-r--r--   0        0        0    12722 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/put.py
--rw-r--r--   0        0        0    12578 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/put.pyi
--rw-r--r--   0        0        0      295 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/__init__.py
--rw-r--r--   0        0        0     8099 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/get.py
--rw-r--r--   0        0        0     8046 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/get.pyi
--rw-r--r--   0        0        0    10067 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/post.py
--rw-r--r--   0        0        0     9983 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/post.pyi
--rw-r--r--   0        0        0      305 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/__init__.py
--rw-r--r--   0        0        0     8154 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/delete.py
--rw-r--r--   0        0        0     8069 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/delete.pyi
--rw-r--r--   0        0        0     9750 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/get.py
--rw-r--r--   0        0        0     9666 2023-05-26 16:01:04.925692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/get.pyi
--rw-r--r--   0        0        0    12535 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/put.py
--rw-r--r--   0        0        0    12421 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/put.pyi
--rw-r--r--   0        0        0      313 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name_run/__init__.py
--rw-r--r--   0        0        0    16672 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name_run/post.py
--rw-r--r--   0        0        0    16558 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name_run/post.pyi
--rw-r--r--   0        0        0      295 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search/__init__.py
--rw-r--r--   0        0        0    22446 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search/get.py
--rw-r--r--   0        0        0    22080 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search/get.pyi
--rw-r--r--   0        0        0      309 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets/__init__.py
--rw-r--r--   0        0        0    22506 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets/get.py
--rw-r--r--   0        0        0    22140 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets/get.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets_download/__init__.py
--rw-r--r--   0        0        0    20854 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets_download/get.py
--rw-r--r--   0        0        0    20457 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets_download/get.pyi
--rw-r--r--   0        0        0      319 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/__init__.py
--rw-r--r--   0        0        0     7831 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/get.py
--rw-r--r--   0        0        0     7747 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/get.pyi
--rw-r--r--   0        0        0    11892 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/put.py
--rw-r--r--   0        0        0    11808 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/put.pyi
--rw-r--r--   0        0        0      330 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/__init__.py
--rw-r--r--   0        0        0     6568 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/get.py
--rw-r--r--   0        0        0     6454 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/get.pyi
--rw-r--r--   0        0        0    10218 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/put.py
--rw-r--r--   0        0        0    10104 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/put.pyi
--rw-r--r--   0        0        0      353 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/__init__.py
--rw-r--r--   0        0        0     6507 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/post.py
--rw-r--r--   0        0        0     6393 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/post.pyi
--rw-r--r--   0        0        0      365 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/__init__.py
--rw-r--r--   0        0        0    10539 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/post.py
--rw-r--r--   0        0        0    10395 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/post.pyi
--rw-r--r--   0        0        0      334 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/__init__.py
--rw-r--r--   0        0        0     8677 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/get.py
--rw-r--r--   0        0        0     8594 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/get.pyi
--rw-r--r--   0        0        0    10707 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/post.py
--rw-r--r--   0        0        0    10584 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/post.pyi
--rw-r--r--   0        0        0      344 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/__init__.py
--rw-r--r--   0        0        0     8613 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/delete.py
--rw-r--r--   0        0        0     8498 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/delete.pyi
--rw-r--r--   0        0        0     9973 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/get.py
--rw-r--r--   0        0        0     9889 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/get.pyi
--rw-r--r--   0        0        0    12858 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/put.py
--rw-r--r--   0        0        0    12735 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/put.pyi
--rw-r--r--   0        0        0      307 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_jwt/__init__.py
--rw-r--r--   0        0        0     6187 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_jwt/put.py
--rw-r--r--   0        0        0     6103 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_jwt/put.pyi
--rw-r--r--   0        0        0      309 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/__init__.py
--rw-r--r--   0        0        0     6545 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/get.py
--rw-r--r--   0        0        0     6431 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/get.pyi
--rw-r--r--   0        0        0    10582 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/post.py
--rw-r--r--   0        0        0    10468 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/post.pyi
--rw-r--r--   0        0        0      334 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_change_order/__init__.py
--rw-r--r--   0        0        0    11198 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_change_order/post.py
--rw-r--r--   0        0        0    11083 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_change_order/post.pyi
--rw-r--r--   0        0        0      319 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/__init__.py
--rw-r--r--   0        0        0     8839 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/delete.py
--rw-r--r--   0        0        0     8694 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/delete.pyi
--rw-r--r--   0        0        0     8785 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/get.py
--rw-r--r--   0        0        0     8640 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/get.pyi
--rw-r--r--   0        0        0    13025 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/put.py
--rw-r--r--   0        0        0    12881 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/put.pyi
--rw-r--r--   0        0        0      321 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges/__init__.py
--rw-r--r--   0        0        0     8509 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges/get.py
--rw-r--r--   0        0        0     8426 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges/get.pyi
--rw-r--r--   0        0        0      345 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application/__init__.py
--rw-r--r--   0        0        0    10247 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application/post.py
--rw-r--r--   0        0        0    10154 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application/post.pyi
--rw-r--r--   0        0        0      375 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application_privilege_name/__init__.py
--rw-r--r--   0        0        0    12755 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application_privilege_name/put.py
--rw-r--r--   0        0        0    12632 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application_privilege_name/put.pyi
--rw-r--r--   0        0        0      351 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/__init__.py
--rw-r--r--   0        0        0     8514 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/delete.py
--rw-r--r--   0        0        0     8399 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/delete.pyi
--rw-r--r--   0        0        0    10205 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/get.py
--rw-r--r--   0        0        0    10091 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/get.pyi
--rw-r--r--   0        0        0      354 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin/__init__.py
--rw-r--r--   0        0        0    10264 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin/post.py
--rw-r--r--   0        0        0    10171 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin/post.pyi
--rw-r--r--   0        0        0      384 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/__init__.py
--rw-r--r--   0        0        0    12772 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/put.py
--rw-r--r--   0        0        0    12649 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/put.pyi
--rw-r--r--   0        0        0      375 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector/__init__.py
--rw-r--r--   0        0        0    10306 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector/post.py
--rw-r--r--   0        0        0    10213 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector/post.pyi
--rw-r--r--   0        0        0      405 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/__init__.py
--rw-r--r--   0        0        0    12814 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/put.py
--rw-r--r--   0        0        0    12691 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/put.pyi
--rw-r--r--   0        0        0      352 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view/__init__.py
--rw-r--r--   0        0        0    10260 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view/post.py
--rw-r--r--   0        0        0    10167 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view/post.pyi
--rw-r--r--   0        0        0      382 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/__init__.py
--rw-r--r--   0        0        0    12768 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/put.py
--rw-r--r--   0        0        0    12645 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/put.pyi
--rw-r--r--   0        0        0      335 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script/__init__.py
--rw-r--r--   0        0        0    10217 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script/post.py
--rw-r--r--   0        0        0    10133 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script/post.pyi
--rw-r--r--   0        0        0      365 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script_privilege_name/__init__.py
--rw-r--r--   0        0        0    12725 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script_privilege_name/put.py
--rw-r--r--   0        0        0    12611 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script_privilege_name/put.pyi
--rw-r--r--   0        0        0      339 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard/__init__.py
--rw-r--r--   0        0        0    10212 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard/post.py
--rw-r--r--   0        0        0    10128 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard/post.pyi
--rw-r--r--   0        0        0      369 2023-05-26 16:01:04.929692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/__init__.py
--rw-r--r--   0        0        0    12720 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/put.py
--rw-r--r--   0        0        0    12606 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/__init__.py
--rw-r--r--   0        0        0     8163 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/get.py
--rw-r--r--   0        0        0     8109 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/get.pyi
--rw-r--r--   0        0        0    11017 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/put.py
--rw-r--r--   0        0        0    10954 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/put.pyi
--rw-r--r--   0        0        0      333 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_available/__init__.py
--rw-r--r--   0        0        0     8159 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_available/get.py
--rw-r--r--   0        0        0     8106 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_available/get.pyi
--rw-r--r--   0        0        0      311 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/__init__.py
--rw-r--r--   0        0        0    10892 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/get.py
--rw-r--r--   0        0        0    10778 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/get.pyi
--rw-r--r--   0        0        0    11580 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/post.py
--rw-r--r--   0        0        0    11496 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/post.pyi
--rw-r--r--   0        0        0      317 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/__init__.py
--rw-r--r--   0        0        0     8022 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/delete.py
--rw-r--r--   0        0        0     7937 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/delete.pyi
--rw-r--r--   0        0        0    12499 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/get.py
--rw-r--r--   0        0        0    12355 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/get.pyi
--rw-r--r--   0        0        0    11862 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/put.py
--rw-r--r--   0        0        0    11778 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/put.pyi
--rw-r--r--   0        0        0      309 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/__init__.py
--rw-r--r--   0        0        0     6670 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/delete.py
--rw-r--r--   0        0        0     6556 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/delete.pyi
--rw-r--r--   0        0        0     6904 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/get.py
--rw-r--r--   0        0        0     6760 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/get.pyi
--rw-r--r--   0        0        0    11465 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/put.py
--rw-r--r--   0        0        0    11291 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/put.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_metadata/__init__.py
--rw-r--r--   0        0        0     6815 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_metadata/get.py
--rw-r--r--   0        0        0     6671 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_metadata/get.pyi
--rw-r--r--   0        0        0      317 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_pem/__init__.py
--rw-r--r--   0        0        0     7087 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_pem/get.py
--rw-r--r--   0        0        0     6943 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_pem/get.pyi
--rw-r--r--   0        0        0      307 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl/__init__.py
--rw-r--r--   0        0        0    11057 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl/get.py
--rw-r--r--   0        0        0    10943 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl/get.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/__init__.py
--rw-r--r--   0        0        0     8702 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/get.py
--rw-r--r--   0        0        0     8619 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/get.pyi
--rw-r--r--   0        0        0    11994 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/post.py
--rw-r--r--   0        0        0    11880 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/post.pyi
--rw-r--r--   0        0        0      335 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore_id/__init__.py
--rw-r--r--   0        0        0     7894 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore_id/delete.py
--rw-r--r--   0        0        0     7839 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore_id/delete.pyi
--rw-r--r--   0        0        0      324 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_sources/__init__.py
--rw-r--r--   0        0        0     8554 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_sources/get.py
--rw-r--r--   0        0        0     8471 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_sources/get.pyi
--rw-r--r--   0        0        0      322 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/__init__.py
--rw-r--r--   0        0        0     6347 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/delete.py
--rw-r--r--   0        0        0     6285 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/delete.pyi
--rw-r--r--   0        0        0     7653 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/get.py
--rw-r--r--   0        0        0     7599 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/get.pyi
--rw-r--r--   0        0        0    11738 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/put.py
--rw-r--r--   0        0        0    11684 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/put.pyi
--rw-r--r--   0        0        0      311 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/__init__.py
--rw-r--r--   0        0        0    11219 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/get.py
--rw-r--r--   0        0        0    11105 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/get.pyi
--rw-r--r--   0        0        0    12249 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/post.py
--rw-r--r--   0        0        0    12135 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/post.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/__init__.py
--rw-r--r--   0        0        0     8397 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/delete.py
--rw-r--r--   0        0        0     8282 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/delete.pyi
--rw-r--r--   0        0        0    12535 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/put.py
--rw-r--r--   0        0        0    12421 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/put.pyi
--rw-r--r--   0        0        0      358 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_change_password/__init__.py
--rw-r--r--   0        0        0    12489 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_change_password/put.py
--rw-r--r--   0        0        0    12374 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_change_password/put.pyi
--rw-r--r--   0        0        0      371 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/__init__.py
--rw-r--r--   0        0        0     9005 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/delete.py
--rw-r--r--   0        0        0     8860 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/delete.pyi
--rw-r--r--   0        0        0      311 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_delete/__init__.py
--rw-r--r--   0        0        0    19869 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_delete/post.py
--rw-r--r--   0        0        0    19694 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_delete/post.pyi
--rw-r--r--   0        0        0      331 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_move_destination/__init__.py
--rw-r--r--   0        0        0    21847 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_move_destination/post.py
--rw-r--r--   0        0        0    21672 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_move_destination/post.pyi
--rw-r--r--   0        0        0      295 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status/get.py
--rw-r--r--   0        0        0     6185 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status/get.pyi
--rw-r--r--   0        0        0      307 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_check/__init__.py
--rw-r--r--   0        0        0     8565 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_check/get.py
--rw-r--r--   0        0        0     8512 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_check/get.pyi
--rw-r--r--   0        0        0      313 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_writable/__init__.py
--rw-r--r--   0        0        0     6268 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_writable/get.py
--rw-r--r--   0        0        0     6184 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_writable/get.pyi
--rw-r--r--   0        0        0      319 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzip/__init__.py
--rw-r--r--   0        0        0    10244 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzip/post.py
--rw-r--r--   0        0        0    10182 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzip/post.pyi
--rw-r--r--   0        0        0      327 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzippath/__init__.py
--rw-r--r--   0        0        0    11771 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzippath/post.py
--rw-r--r--   0        0        0    11717 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzippath/post.pyi
--rw-r--r--   0        0        0      311 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/__init__.py
--rw-r--r--   0        0        0     6265 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/delete.py
--rw-r--r--   0        0        0     6203 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/delete.pyi
--rw-r--r--   0        0        0     7679 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/get.py
--rw-r--r--   0        0        0     7625 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/get.pyi
--rw-r--r--   0        0        0    12254 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/post.py
--rw-r--r--   0        0        0    12200 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/post.pyi
--rw-r--r--   0        0        0      291 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/__init__.py
--rw-r--r--   0        0        0     9750 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/get.py
--rw-r--r--   0        0        0     9696 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/get.pyi
--rw-r--r--   0        0        0    10106 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/post.py
--rw-r--r--   0        0        0    10022 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/post.pyi
--rw-r--r--   0        0        0      329 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/__init__.py
--rw-r--r--   0        0        0    21076 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/delete.py
--rw-r--r--   0        0        0    20991 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/delete.pyi
--rw-r--r--   0        0        0    21292 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/post.py
--rw-r--r--   0        0        0    21207 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/post.pyi
--rw-r--r--   0        0        0      301 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/__init__.py
--rw-r--r--   0        0        0     8138 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/delete.py
--rw-r--r--   0        0        0     8053 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/delete.pyi
--rw-r--r--   0        0        0     9713 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/get.py
--rw-r--r--   0        0        0     9629 2023-05-26 16:01:04.933692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/get.pyi
--rw-r--r--   0        0        0    14319 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/put.py
--rw-r--r--   0        0        0    14205 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/put.pyi
--rw-r--r--   0        0        0      293 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks/__init__.py
--rw-r--r--   0        0        0     9672 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks/get.py
--rw-r--r--   0        0        0     9618 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks/get.pyi
--rw-r--r--   0        0        0      299 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id/__init__.py
--rw-r--r--   0        0        0     9823 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id/get.py
--rw-r--r--   0        0        0     9739 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id/get.pyi
--rw-r--r--   0        0        0      307 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_run/__init__.py
--rw-r--r--   0        0        0     8352 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_run/post.py
--rw-r--r--   0        0        0     8237 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_run/post.pyi
--rw-r--r--   0        0        0      309 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_stop/__init__.py
--rw-r--r--   0        0        0     8364 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_stop/post.py
--rw-r--r--   0        0        0     8249 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_stop/post.pyi
--rw-r--r--   0        0        0    10722 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/rest.py
--rw-r--r--   0        0        0    97679 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/nexus_sdk/schemas.py
--rw-r--r--   0        0        0      621 2023-05-26 16:01:04.937692 sonatype_nexus_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0   113836 1970-01-01 00:00:00.000000 sonatype_nexus_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0   101067 2023-05-26 16:14:06.909423 sonatype_nexus_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0      641 2023-05-26 16:14:06.917424 sonatype_nexus_sdk-0.1.3/nexus_sdk/__init__.py
+-rw-r--r--   0        0        0    59495 2023-05-26 16:14:06.917424 sonatype_nexus_sdk-0.1.3/nexus_sdk/api_client.py
+-rw-r--r--   0        0        0      215 2023-05-26 16:14:06.917424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/__init__.py
+-rw-r--r--   0        0        0    46580 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/path_to_api.py
+-rw-r--r--   0        0        0      236 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/beta_replication_connection.py
+-rw-r--r--   0        0        0      330 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/beta_replication_connection_name.py
+-rw-r--r--   0        0        0      157 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/beta_replicationtarget_repository_enable.py
+-rw-r--r--   0        0        0      205 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/beta_replicationtarget_repository_repository_name_enable.py
+-rw-r--r--   0        0        0       97 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_assets.py
+-rw-r--r--   0        0        0      181 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_assets_id.py
+-rw-r--r--   0        0        0      146 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_azureblobstore_test_connection.py
+-rw-r--r--   0        0        0      105 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores.py
+-rw-r--r--   0        0        0      119 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_azure.py
+-rw-r--r--   0        0        0      207 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_azure_name.py
+-rw-r--r--   0        0        0      117 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_file.py
+-rw-r--r--   0        0        0      204 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_file_name.py
+-rw-r--r--   0        0        0      119 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_group.py
+-rw-r--r--   0        0        0      192 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_group_convert_name_new_name_for_original.py
+-rw-r--r--   0        0        0      207 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_group_name.py
+-rw-r--r--   0        0        0      123 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_name.py
+-rw-r--r--   0        0        0      138 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_name_quota_status.py
+-rw-r--r--   0        0        0      113 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_s3.py
+-rw-r--r--   0        0        0      198 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_blobstores_s3_name.py
+-rw-r--r--   0        0        0      179 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_components.py
+-rw-r--r--   0        0        0      193 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_components_id.py
+-rw-r--r--   0        0        0      236 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_email.py
+-rw-r--r--   0        0        0      111 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_email_verify.py
+-rw-r--r--   0        0        0      136 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_formats_format_upload_specs.py
+-rw-r--r--   0        0        0      123 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_formats_upload_specs.py
+-rw-r--r--   0        0        0      152 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_iq.py
+-rw-r--r--   0        0        0      107 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_iq_disable.py
+-rw-r--r--   0        0        0      105 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_iq_enable.py
+-rw-r--r--   0        0        0      126 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_iq_verify_connection.py
+-rw-r--r--   0        0        0      116 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_lifecycle_bounce.py
+-rw-r--r--   0        0        0      190 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_lifecycle_phase.py
+-rw-r--r--   0        0        0      102 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_read_only.py
+-rw-r--r--   0        0        0      131 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_read_only_force_release.py
+-rw-r--r--   0        0        0      118 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_read_only_freeze.py
+-rw-r--r--   0        0        0      120 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_read_only_release.py
+-rw-r--r--   0        0        0      109 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories.py
+-rw-r--r--   0        0        0      132 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_apt_hosted.py
+-rw-r--r--   0        0        0      259 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_apt_hosted_repository_name.py
+-rw-r--r--   0        0        0      130 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_apt_proxy.py
+-rw-r--r--   0        0        0      256 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_apt_proxy_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_bower_group.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_bower_group_repository_name.py
+-rw-r--r--   0        0        0      136 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_bower_hosted.py
+-rw-r--r--   0        0        0      265 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_bower_hosted_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_bower_proxy.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_bower_proxy_repository_name.py
+-rw-r--r--   0        0        0      142 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_cocoapods_proxy.py
+-rw-r--r--   0        0        0      292 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_cocoapods_proxy_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_conan_proxy.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_conan_proxy_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_conda_proxy.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_conda_proxy_repository_name.py
+-rw-r--r--   0        0        0      136 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_docker_group.py
+-rw-r--r--   0        0        0      265 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_docker_group_repository_name.py
+-rw-r--r--   0        0        0      138 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_docker_hosted.py
+-rw-r--r--   0        0        0      268 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_docker_hosted_repository_name.py
+-rw-r--r--   0        0        0      136 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_docker_proxy.py
+-rw-r--r--   0        0        0      265 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_docker_proxy_repository_name.py
+-rw-r--r--   0        0        0      138 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_gitlfs_hosted.py
+-rw-r--r--   0        0        0      268 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_gitlfs_hosted_repository_name.py
+-rw-r--r--   0        0        0      128 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_go_group.py
+-rw-r--r--   0        0        0      253 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_go_group_repository_name.py
+-rw-r--r--   0        0        0      128 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_go_proxy.py
+-rw-r--r--   0        0        0      253 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_go_proxy_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_helm_hosted.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_helm_hosted_repository_name.py
+-rw-r--r--   0        0        0      132 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_helm_proxy.py
+-rw-r--r--   0        0        0      259 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_helm_proxy_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_maven_group.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_maven_group_repository_name.py
+-rw-r--r--   0        0        0      136 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_maven_hosted.py
+-rw-r--r--   0        0        0      265 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_maven_hosted_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_maven_proxy.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_maven_proxy_repository_name.py
+-rw-r--r--   0        0        0      130 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_npm_group.py
+-rw-r--r--   0        0        0      256 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_npm_group_repository_name.py
+-rw-r--r--   0        0        0      132 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_npm_hosted.py
+-rw-r--r--   0        0        0      259 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_npm_hosted_repository_name.py
+-rw-r--r--   0        0        0      130 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_npm_proxy.py
+-rw-r--r--   0        0        0      256 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_npm_proxy_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_nuget_group.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_nuget_group_repository_name.py
+-rw-r--r--   0        0        0      136 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_nuget_hosted.py
+-rw-r--r--   0        0        0      265 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_nuget_hosted_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_nuget_proxy.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_nuget_proxy_repository_name.py
+-rw-r--r--   0        0        0      128 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_p2_proxy.py
+-rw-r--r--   0        0        0      253 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_p2_proxy_repository_name.py
+-rw-r--r--   0        0        0      132 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_pypi_group.py
+-rw-r--r--   0        0        0      259 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_pypi_group_repository_name.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_pypi_hosted.py
+-rw-r--r--   0        0        0      262 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_pypi_hosted_repository_name.py
+-rw-r--r--   0        0        0      132 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_pypi_proxy.py
+-rw-r--r--   0        0        0      259 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_pypi_proxy_repository_name.py
+-rw-r--r--   0        0        0      126 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_r_group.py
+-rw-r--r--   0        0        0      250 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_r_group_repository_name.py
+-rw-r--r--   0        0        0      128 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_r_hosted.py
+-rw-r--r--   0        0        0      253 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_r_hosted_repository_name.py
+-rw-r--r--   0        0        0      126 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_r_proxy.py
+-rw-r--r--   0        0        0      250 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_r_proxy_repository_name.py
+-rw-r--r--   0        0        0      130 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_raw_group.py
+-rw-r--r--   0        0        0      256 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_raw_group_repository_name.py
+-rw-r--r--   0        0        0      132 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_raw_hosted.py
+-rw-r--r--   0        0        0      259 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_raw_hosted_repository_name.py
+-rw-r--r--   0        0        0      130 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_raw_proxy.py
+-rw-r--r--   0        0        0      256 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_raw_proxy_repository_name.py
+-rw-r--r--   0        0        0      237 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_repository_name.py
+-rw-r--r--   0        0        0      286 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_repository_name_health_check.py
+-rw-r--r--   0        0        0      183 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_repository_name_invalidate_cache.py
+-rw-r--r--   0        0        0      177 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_repository_name_rebuild_index.py
+-rw-r--r--   0        0        0      140 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_rubygems_group.py
+-rw-r--r--   0        0        0      271 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_rubygems_group_repository_name.py
+-rw-r--r--   0        0        0      142 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_rubygems_hosted.py
+-rw-r--r--   0        0        0      292 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_rubygems_hosted_repository_name.py
+-rw-r--r--   0        0        0      140 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_rubygems_proxy.py
+-rw-r--r--   0        0        0      271 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_rubygems_proxy_repository_name.py
+-rw-r--r--   0        0        0      130 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_yum_group.py
+-rw-r--r--   0        0        0      256 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_yum_group_repository_name.py
+-rw-r--r--   0        0        0      132 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_yum_hosted.py
+-rw-r--r--   0        0        0      259 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_yum_hosted_repository_name.py
+-rw-r--r--   0        0        0      130 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_yum_proxy.py
+-rw-r--r--   0        0        0      256 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repositories_yum_proxy_repository_name.py
+-rw-r--r--   0        0        0      122 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_repository_settings.py
+-rw-r--r--   0        0        0      187 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_routing_rules.py
+-rw-r--r--   0        0        0      286 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_routing_rules_name.py
+-rw-r--r--   0        0        0      167 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_script.py
+-rw-r--r--   0        0        0      259 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_script_name.py
+-rw-r--r--   0        0        0      116 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_script_name_run.py
+-rw-r--r--   0        0        0       97 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_search.py
+-rw-r--r--   0        0        0      110 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_search_assets.py
+-rw-r--r--   0        0        0      127 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_search_assets_download.py
+-rw-r--r--   0        0        0      199 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_anonymous.py
+-rw-r--r--   0        0        0      216 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_atlassian_crowd.py
+-rw-r--r--   0        0        0      156 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_atlassian_crowd_clear_cache.py
+-rw-r--r--   0        0        0      177 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_atlassian_crowd_verify_connection.py
+-rw-r--r--   0        0        0      225 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_content_selectors.py
+-rw-r--r--   0        0        0      337 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_content_selectors_name.py
+-rw-r--r--   0        0        0      108 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_jwt.py
+-rw-r--r--   0        0        0      187 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_ldap.py
+-rw-r--r--   0        0        0      137 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_ldap_change_order.py
+-rw-r--r--   0        0        0      286 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_ldap_name.py
+-rw-r--r--   0        0        0      122 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges.py
+-rw-r--r--   0        0        0      148 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_application.py
+-rw-r--r--   0        0        0      182 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_application_privilege_name.py
+-rw-r--r--   0        0        0      254 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_privilege_name.py
+-rw-r--r--   0        0        0      157 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_repository_admin.py
+-rw-r--r--   0        0        0      191 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_repository_admin_privilege_name.py
+-rw-r--r--   0        0        0      187 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_repository_content_selector.py
+-rw-r--r--   0        0        0      212 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_repository_content_selector_privilege_name.py
+-rw-r--r--   0        0        0      155 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_repository_view.py
+-rw-r--r--   0        0        0      189 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_repository_view_privilege_name.py
+-rw-r--r--   0        0        0      138 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_script.py
+-rw-r--r--   0        0        0      163 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_script_privilege_name.py
+-rw-r--r--   0        0        0      142 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_wildcard.py
+-rw-r--r--   0        0        0      167 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_privileges_wildcard_privilege_name.py
+-rw-r--r--   0        0        0      210 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_realms_active.py
+-rw-r--r--   0        0        0      133 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_realms_available.py
+-rw-r--r--   0        0        0      190 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_roles.py
+-rw-r--r--   0        0        0      282 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_roles_id.py
+-rw-r--r--   0        0        0      267 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_saml.py
+-rw-r--r--   0        0        0      127 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_saml_metadata.py
+-rw-r--r--   0        0        0      117 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_saml_pem.py
+-rw-r--r--   0        0        0      108 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_ssl.py
+-rw-r--r--   0        0        0      216 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_ssl_truststore.py
+-rw-r--r--   0        0        0      143 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_ssl_truststore_id.py
+-rw-r--r--   0        0        0      125 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_user_sources.py
+-rw-r--r--   0        0        0      294 2023-05-26 16:14:06.921424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_user_tokens.py
+-rw-r--r--   0        0        0      190 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_users.py
+-rw-r--r--   0        0        0      218 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_users_user_id.py
+-rw-r--r--   0        0        0      156 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_users_user_id_change_password.py
+-rw-r--r--   0        0        0      186 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_security_users_user_id_realm_user_token_reset.py
+-rw-r--r--   0        0        0      115 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_staging_delete.py
+-rw-r--r--   0        0        0      134 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_staging_move_destination.py
+-rw-r--r--   0        0        0       97 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_status.py
+-rw-r--r--   0        0        0      108 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_status_check.py
+-rw-r--r--   0        0        0      114 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_status_writable.py
+-rw-r--r--   0        0        0      123 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_support_supportzip.py
+-rw-r--r--   0        0        0      131 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_support_supportzippath.py
+-rw-r--r--   0        0        0      274 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_system_license.py
+-rw-r--r--   0        0        0      161 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_tags.py
+-rw-r--r--   0        0        0      224 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_tags_associate_tag_name.py
+-rw-r--r--   0        0        0      251 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_tags_name.py
+-rw-r--r--   0        0        0       95 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_tasks.py
+-rw-r--r--   0        0        0      100 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_tasks_id.py
+-rw-r--r--   0        0        0      110 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_tasks_id_run.py
+-rw-r--r--   0        0        0      112 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/paths/v1_tasks_id_stop.py
+-rw-r--r--   0        0        0     6299 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tag_to_api.py
+-rw-r--r--   0        0        0     1682 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/__init__.py
+-rw-r--r--   0        0        0      691 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/assets_api.py
+-rw-r--r--   0        0        0      587 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/azure_blob_store_api.py
+-rw-r--r--   0        0        0     2077 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/blob_store_api.py
+-rw-r--r--   0        0        0      815 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/components_api.py
+-rw-r--r--   0        0        0     1054 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/content_selectors_api.py
+-rw-r--r--   0        0        0      849 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/email_api.py
+-rw-r--r--   0        0        0      621 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/formats_api.py
+-rw-r--r--   0        0        0      693 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/lifecycle_api.py
+-rw-r--r--   0        0        0      889 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/manage_iq_server_configuration_api.py
+-rw-r--r--   0        0        0      734 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/product_licensing_api.py
+-rw-r--r--   0        0        0      769 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/read_only_api.py
+-rw-r--r--   0        0        0     1110 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/replication_api.py
+-rw-r--r--   0        0        0    15722 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/repository_management_api.py
+-rw-r--r--   0        0        0      936 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/routing_rules_api.py
+-rw-r--r--   0        0        0      852 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/script_api.py
+-rw-r--r--   0        0        0      723 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/search_api.py
+-rw-r--r--   0        0        0      902 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_atlassian_crowd_api.py
+-rw-r--r--   0        0        0      895 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_certificates_api.py
+-rw-r--r--   0        0        0      640 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_anonymous_access_api.py
+-rw-r--r--   0        0        0      575 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_api.py
+-rw-r--r--   0        0        0      563 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_jwt_api.py
+-rw-r--r--   0        0        0     1028 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_ldap_api.py
+-rw-r--r--   0        0        0     2262 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_privileges_api.py
+-rw-r--r--   0        0        0      765 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_realms_api.py
+-rw-r--r--   0        0        0      854 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_roles_api.py
+-rw-r--r--   0        0        0      993 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_saml_api.py
+-rw-r--r--   0        0        0      779 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_user_tokens_api.py
+-rw-r--r--   0        0        0     1031 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_users_api.py
+-rw-r--r--   0        0        0      620 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/staging_api.py
+-rw-r--r--   0        0        0      717 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/status_api.py
+-rw-r--r--   0        0        0      648 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/support_api.py
+-rw-r--r--   0        0        0      965 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/tags_api.py
+-rw-r--r--   0        0        0      734 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/tasks_api.py
+-rw-r--r--   0        0        0    15433 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/configuration.py
+-rw-r--r--   0        0        0     4515 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/exceptions.py
+-rw-r--r--   0        0        0      343 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/__init__.py
+-rw-r--r--   0        0        0     6054 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/abstract_api_repository.py
+-rw-r--r--   0        0        0     5015 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/abstract_api_repository.pyi
+-rw-r--r--   0        0        0     4164 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/anonymous_access_settings_xo.py
+-rw-r--r--   0        0        0     3552 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/anonymous_access_settings_xo.pyi
+-rw-r--r--   0        0        0    10633 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_certificate.py
+-rw-r--r--   0        0        0     9255 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_certificate.pyi
+-rw-r--r--   0        0        0     8568 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_create_user.py
+-rw-r--r--   0        0        0     7129 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_create_user.pyi
+-rw-r--r--   0        0        0    10633 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_email_configuration.py
+-rw-r--r--   0        0        0     9191 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_email_configuration.pyi
+-rw-r--r--   0        0        0     3516 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_email_validation.py
+-rw-r--r--   0        0        0     2994 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_email_validation.pyi
+-rw-r--r--   0        0        0     8387 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_license_details_xo.py
+-rw-r--r--   0        0        0     7235 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_license_details_xo.pyi
+-rw-r--r--   0        0        0     4957 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege.py
+-rw-r--r--   0        0        0     4101 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege.pyi
+-rw-r--r--   0        0        0     7909 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_application_request.py
+-rw-r--r--   0        0        0     6540 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_application_request.pyi
+-rw-r--r--   0        0        0     8564 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_admin_request.py
+-rw-r--r--   0        0        0     7105 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_admin_request.pyi
+-rw-r--r--   0        0        0     9296 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_content_selector_request.py
+-rw-r--r--   0        0        0     7747 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_content_selector_request.pyi
+-rw-r--r--   0        0        0     8562 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_view_request.py
+-rw-r--r--   0        0        0     7103 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_view_request.pyi
+-rw-r--r--   0        0        0     7951 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_script_request.py
+-rw-r--r--   0        0        0     6582 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_script_request.pyi
+-rw-r--r--   0        0        0     4402 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_wildcard_request.py
+-rw-r--r--   0        0        0     3637 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_wildcard_request.pyi
+-rw-r--r--   0        0        0    10951 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_user.py
+-rw-r--r--   0        0        0     9032 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_user.pyi
+-rw-r--r--   0        0        0     3391 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_user_source.py
+-rw-r--r--   0        0        0     2891 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_user_source.pyi
+-rw-r--r--   0        0        0     7650 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_api_repository.py
+-rw-r--r--   0        0        0     6647 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_api_repository.pyi
+-rw-r--r--   0        0        0     2862 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_repositories_attributes.py
+-rw-r--r--   0        0        0     2578 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_repositories_attributes.pyi
+-rw-r--r--   0        0        0     7672 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     6658 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     9725 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_api_repository.py
+-rw-r--r--   0        0        0     8498 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_api_repository.pyi
+-rw-r--r--   0        0        0     3620 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_repositories_attributes.py
+-rw-r--r--   0        0        0     3090 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_repositories_attributes.pyi
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     8457 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     3594 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_signing_repositories_attributes.py
+-rw-r--r--   0        0        0     3072 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_signing_repositories_attributes.pyi
+-rw-r--r--   0        0        0    11166 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/asset_xo.py
+-rw-r--r--   0        0        0     9654 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/asset_xo.pyi
+-rw-r--r--   0        0        0     4550 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_authentication.py
+-rw-r--r--   0        0        0     3858 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_authentication.pyi
+-rw-r--r--   0        0        0     4922 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_bucket_configuration.py
+-rw-r--r--   0        0        0     4167 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_bucket_configuration.pyi
+-rw-r--r--   0        0        0     4732 2023-05-26 16:14:06.925424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_model.py
+-rw-r--r--   0        0        0     4129 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_model.pyi
+-rw-r--r--   0        0        0     5079 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_connection_xo.py
+-rw-r--r--   0        0        0     4377 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_connection_xo.pyi
+-rw-r--r--   0        0        0     4087 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/base_tag_xo.py
+-rw-r--r--   0        0        0     3692 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/base_tag_xo.pyi
+-rw-r--r--   0        0        0     4135 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/blob_store_api_soft_quota.py
+-rw-r--r--   0        0        0     3450 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/blob_store_api_soft_quota.pyi
+-rw-r--r--   0        0        0     4275 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/blob_store_quota_result_xo.py
+-rw-r--r--   0        0        0     3663 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/blob_store_quota_result_xo.pyi
+-rw-r--r--   0        0        0     2993 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_attributes.py
+-rw-r--r--   0        0        0     2701 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_attributes.pyi
+-rw-r--r--   0        0        0     5145 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_group_repository_api_request.py
+-rw-r--r--   0        0        0     4329 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6044 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5168 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     9646 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_proxy_api_repository.py
+-rw-r--r--   0        0        0     8428 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_proxy_api_repository.pyi
+-rw-r--r--   0        0        0     9616 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     8387 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     3903 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/cleanup_policy_attributes.py
+-rw-r--r--   0        0        0     3359 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/cleanup_policy_attributes.pyi
+-rw-r--r--   0        0        0     8945 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/cocoapods_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7776 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/cocoapods_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     2975 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/component_attributes.py
+-rw-r--r--   0        0        0     2673 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/component_attributes.pyi
+-rw-r--r--   0        0        0     7191 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/component_xo.py
+-rw-r--r--   0        0        0     6365 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/component_xo.pyi
+-rw-r--r--   0        0        0     8937 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/conan_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7768 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/conan_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     8937 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/conda_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7768 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/conda_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     4449 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_create_request.py
+-rw-r--r--   0        0        0     3684 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_create_request.pyi
+-rw-r--r--   0        0        0     5195 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_response.py
+-rw-r--r--   0        0        0     4418 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_response.pyi
+-rw-r--r--   0        0        0     3644 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_update_request.py
+-rw-r--r--   0        0        0     3122 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_update_request.pyi
+-rw-r--r--   0        0        0    26439 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/create_ldap_server_xo.py
+-rw-r--r--   0        0        0    22642 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/create_ldap_server_xo.pyi
+-rw-r--r--   0        0        0     7213 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/crowd_api_xo.py
+-rw-r--r--   0        0        0     6163 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/crowd_api_xo.pyi
+-rw-r--r--   0        0        0     5665 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_attributes.py
+-rw-r--r--   0        0        0     4854 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_attributes.pyi
+-rw-r--r--   0        0        0     5849 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_group_api_repository.py
+-rw-r--r--   0        0        0     4984 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_group_api_repository.pyi
+-rw-r--r--   0        0        0     5871 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_group_repository_api_request.py
+-rw-r--r--   0        0        0     4995 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6699 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_api_repository.py
+-rw-r--r--   0        0        0     5774 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_api_repository.pyi
+-rw-r--r--   0        0        0     6779 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5834 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     5964 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_storage_attributes.py
+-rw-r--r--   0        0        0     5130 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_storage_attributes.pyi
+-rw-r--r--   0        0        0    10420 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_api_repository.py
+-rw-r--r--   0        0        0     9142 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_api_repository.pyi
+-rw-r--r--   0        0        0     6830 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_attributes.py
+-rw-r--r--   0        0        0     5759 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_attributes.pyi
+-rw-r--r--   0        0        0    10390 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     9101 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     4237 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_create_request.py
+-rw-r--r--   0        0        0     3654 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_create_request.pyi
+-rw-r--r--   0        0        0     3652 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_model.py
+-rw-r--r--   0        0        0     3159 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_model.pyi
+-rw-r--r--   0        0        0     3668 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_update_request.py
+-rw-r--r--   0        0        0     3175 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_update_request.pyi
+-rw-r--r--   0        0        0     7138 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/generic_blob_store_api_response.py
+-rw-r--r--   0        0        0     6158 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/generic_blob_store_api_response.pyi
+-rw-r--r--   0        0        0     6046 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/git_lfs_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5170 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/git_lfs_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     5147 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/golang_group_repository_api_request.py
+-rw-r--r--   0        0        0     4331 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/golang_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     8939 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/golang_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7770 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/golang_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     3887 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_attributes.py
+-rw-r--r--   0        0        0     3343 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_attributes.pyi
+-rw-r--r--   0        0        0     6475 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_create_request.py
+-rw-r--r--   0        0        0     5437 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_create_request.pyi
+-rw-r--r--   0        0        0     5890 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_model.py
+-rw-r--r--   0        0        0     4942 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_model.pyi
+-rw-r--r--   0        0        0     6465 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_response.py
+-rw-r--r--   0        0        0     5427 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_response.pyi
+-rw-r--r--   0        0        0     5906 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_update_request.py
+-rw-r--r--   0        0        0     4958 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_update_request.pyi
+-rw-r--r--   0        0        0     4746 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_deploy_attributes.py
+-rw-r--r--   0        0        0     3964 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_deploy_attributes.pyi
+-rw-r--r--   0        0        0     6042 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/helm_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5166 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/helm_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     8935 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/helm_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7766 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/helm_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     5277 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/hosted_storage_attributes.py
+-rw-r--r--   0        0        0     4533 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/hosted_storage_attributes.pyi
+-rw-r--r--   0        0        0     5542 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_attributes.py
+-rw-r--r--   0        0        0     4785 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_attributes.pyi
+-rw-r--r--   0        0        0     5730 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_attributes_with_preemptive_auth.py
+-rw-r--r--   0        0        0     4921 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_attributes_with_preemptive_auth.pyi
+-rw-r--r--   0        0        0     6820 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_attributes.py
+-rw-r--r--   0        0        0     5779 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_attributes.pyi
+-rw-r--r--   0        0        0     5880 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_authentication_attributes.py
+-rw-r--r--   0        0        0     5006 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_authentication_attributes.pyi
+-rw-r--r--   0        0        0     6557 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_authentication_attributes_with_preemptive.py
+-rw-r--r--   0        0        0     5593 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_authentication_attributes_with_preemptive.pyi
+-rw-r--r--   0        0        0     3532 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/iq_connection_verification_xo.py
+-rw-r--r--   0        0        0     3010 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/iq_connection_verification_xo.pyi
+-rw-r--r--   0        0        0     8859 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/iq_connection_xo.py
+-rw-r--r--   0        0        0     7568 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/iq_connection_xo.pyi
+-rw-r--r--   0        0        0     5927 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_attributes.py
+-rw-r--r--   0        0        0     5021 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_attributes.pyi
+-rw-r--r--   0        0        0     5145 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_group_repository_api_request.py
+-rw-r--r--   0        0        0     4329 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6677 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_hosted_api_repository.py
+-rw-r--r--   0        0        0     5752 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_hosted_api_repository.pyi
+-rw-r--r--   0        0        0     6699 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5763 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     9622 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_proxy_api_repository.py
+-rw-r--r--   0        0        0     8404 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_proxy_api_repository.pyi
+-rw-r--r--   0        0        0     9748 2023-05-26 16:14:06.929424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     8510 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     3685 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/negative_cache_attributes.py
+-rw-r--r--   0        0        0     3132 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/negative_cache_attributes.pyi
+-rw-r--r--   0        0        0     3924 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_attributes.py
+-rw-r--r--   0        0        0     3383 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_attributes.pyi
+-rw-r--r--   0        0        0     5190 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_group_repository_api_request.py
+-rw-r--r--   0        0        0     4374 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6040 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5164 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     9594 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_proxy_api_repository.py
+-rw-r--r--   0        0        0     8390 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_proxy_api_repository.pyi
+-rw-r--r--   0        0        0     9564 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     8349 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     4218 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_attributes.py
+-rw-r--r--   0        0        0     3592 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_attributes.pyi
+-rw-r--r--   0        0        0     5145 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_group_repository_api_request.py
+-rw-r--r--   0        0        0     4329 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6044 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5168 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     9682 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_proxy_api_repository.py
+-rw-r--r--   0        0        0     8464 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_proxy_api_repository.pyi
+-rw-r--r--   0        0        0     9652 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     8423 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     8931 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/p2_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7762 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/p2_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     4780 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page.py
+-rw-r--r--   0        0        0     3934 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page.pyi
+-rw-r--r--   0        0        0     4392 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_asset_xo.py
+-rw-r--r--   0        0        0     3995 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_asset_xo.pyi
+-rw-r--r--   0        0        0     4474 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_component_xo.py
+-rw-r--r--   0        0        0     4031 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_component_xo.pyi
+-rw-r--r--   0        0        0     4374 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_tag_xo.py
+-rw-r--r--   0        0        0     3977 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_tag_xo.pyi
+-rw-r--r--   0        0        0     4383 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_task_xo.py
+-rw-r--r--   0        0        0     3986 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_task_xo.pyi
+-rw-r--r--   0        0        0     4492 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/proxy_attributes.py
+-rw-r--r--   0        0        0     3837 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/proxy_attributes.pyi
+-rw-r--r--   0        0        0     5143 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_group_repository_api_request.py
+-rw-r--r--   0        0        0     4327 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6042 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5166 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     8935 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7766 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     5137 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_group_repository_api_request.py
+-rw-r--r--   0        0        0     4321 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6036 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5160 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     8929 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7760 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     3358 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_attributes.py
+-rw-r--r--   0        0        0     2984 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_attributes.pyi
+-rw-r--r--   0        0        0     5772 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_group_repository_api_request.py
+-rw-r--r--   0        0        0     4910 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6671 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5749 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     9564 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     8349 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0    26852 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/read_ldap_server_xo.py
+-rw-r--r--   0        0        0    22998 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/read_ldap_server_xo.pyi
+-rw-r--r--   0        0        0     4298 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/read_only_state.py
+-rw-r--r--   0        0        0     3686 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/read_only_state.pyi
+-rw-r--r--   0        0        0     3385 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/realm_api_xo.py
+-rw-r--r--   0        0        0     2885 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/realm_api_xo.pyi
+-rw-r--r--   0        0        0     3900 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_attributes.py
+-rw-r--r--   0        0        0     3370 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_attributes.pyi
+-rw-r--r--   0        0        0    11065 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_connection_xo.py
+-rw-r--r--   0        0        0     9543 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_connection_xo.pyi
+-rw-r--r--   0        0        0     4925 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_enable_xo.py
+-rw-r--r--   0        0        0     4283 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_enable_xo.pyi
+-rw-r--r--   0        0        0     6509 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/repository_xo.py
+-rw-r--r--   0        0        0     5627 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/repository_xo.pyi
+-rw-r--r--   0        0        0     7892 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/result.py
+-rw-r--r--   0        0        0     6851 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/result.pyi
+-rw-r--r--   0        0        0     7494 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/role_xo_request.py
+-rw-r--r--   0        0        0     6123 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/role_xo_request.pyi
+-rw-r--r--   0        0        0     8714 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/role_xo_response.py
+-rw-r--r--   0        0        0     7163 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/role_xo_response.pyi
+-rw-r--r--   0        0        0     6454 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/routing_rule_xo.py
+-rw-r--r--   0        0        0     5260 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/routing_rule_xo.pyi
+-rw-r--r--   0        0        0     5151 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_group_repository_api_request.py
+-rw-r--r--   0        0        0     4335 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6050 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5174 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     8943 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     7774 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     5166 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_advanced_bucket_connection.py
+-rw-r--r--   0        0        0     4427 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_advanced_bucket_connection.pyi
+-rw-r--r--   0        0        0     4833 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket.py
+-rw-r--r--   0        0        0     4089 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket.pyi
+-rw-r--r--   0        0        0     5896 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket_configuration.py
+-rw-r--r--   0        0        0     5200 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket_configuration.pyi
+-rw-r--r--   0        0        0     4945 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket_security.py
+-rw-r--r--   0        0        0     4243 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket_security.pyi
+-rw-r--r--   0        0        0     4260 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_encryption.py
+-rw-r--r--   0        0        0     3599 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_encryption.pyi
+-rw-r--r--   0        0        0     5271 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_model.py
+-rw-r--r--   0        0        0     4578 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_model.pyi
+-rw-r--r--   0        0        0     9042 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/saml_configuration_xo.py
+-rw-r--r--   0        0        0     7871 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/saml_configuration_xo.pyi
+-rw-r--r--   0        0        0     3467 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/script_result_xo.py
+-rw-r--r--   0        0        0     2945 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/script_result_xo.pyi
+-rw-r--r--   0        0        0     4273 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/script_xo.py
+-rw-r--r--   0        0        0     3508 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/script_xo.pyi
+-rw-r--r--   0        0        0     5186 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_group_deploy_repository.py
+-rw-r--r--   0        0        0     4381 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_group_deploy_repository.pyi
+-rw-r--r--   0        0        0     5125 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_group_repository.py
+-rw-r--r--   0        0        0     4320 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_group_repository.pyi
+-rw-r--r--   0        0        0     6024 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_hosted_repository.py
+-rw-r--r--   0        0        0     5159 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_hosted_repository.pyi
+-rw-r--r--   0        0        0     8969 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_proxy_repository.py
+-rw-r--r--   0        0        0     7811 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_proxy_repository.pyi
+-rw-r--r--   0        0        0     5552 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/stack_trace_element.py
+-rw-r--r--   0        0        0     4760 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/stack_trace_element.pyi
+-rw-r--r--   0        0        0     3975 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/storage_attributes.py
+-rw-r--r--   0        0        0     3445 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/storage_attributes.pyi
+-rw-r--r--   0        0        0     9980 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/support_zip_generator_request.py
+-rw-r--r--   0        0        0     8602 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/support_zip_generator_request.pyi
+-rw-r--r--   0        0        0     4642 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/support_zip_xo.py
+-rw-r--r--   0        0        0     3940 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/support_zip_xo.pyi
+-rw-r--r--   0        0        0     6508 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/tag_xo.py
+-rw-r--r--   0        0        0     5462 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/tag_xo.pyi
+-rw-r--r--   0        0        0     7159 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/task_xo.py
+-rw-r--r--   0        0        0     6119 2023-05-26 16:14:06.933424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/task_xo.pyi
+-rw-r--r--   0        0        0     7206 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/throwable.py
+-rw-r--r--   0        0        0     6591 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/throwable.pyi
+-rw-r--r--   0        0        0    26960 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/update_ldap_server_xo.py
+-rw-r--r--   0        0        0    23095 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/update_ldap_server_xo.pyi
+-rw-r--r--   0        0        0     6835 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/upload_definition_xo.py
+-rw-r--r--   0        0        0     6241 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/upload_definition_xo.pyi
+-rw-r--r--   0        0        0     5324 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/upload_field_definition_xo.py
+-rw-r--r--   0        0        0     4532 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/upload_field_definition_xo.pyi
+-rw-r--r--   0        0        0     3622 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/user_tokens_api_model.py
+-rw-r--r--   0        0        0     3100 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/user_tokens_api_model.pyi
+-rw-r--r--   0        0        0     4373 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_attributes.py
+-rw-r--r--   0        0        0     3664 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_attributes.pyi
+-rw-r--r--   0        0        0     6022 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_group_repository_api_request.py
+-rw-r--r--   0        0        0     5115 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_group_repository_api_request.pyi
+-rw-r--r--   0        0        0     6605 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_hosted_api_repository.py
+-rw-r--r--   0        0        0     5708 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_hosted_api_repository.pyi
+-rw-r--r--   0        0        0     6627 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_hosted_repository_api_request.py
+-rw-r--r--   0        0        0     5719 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_hosted_repository_api_request.pyi
+-rw-r--r--   0        0        0     8741 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_proxy_repository_api_request.py
+-rw-r--r--   0        0        0     8554 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_proxy_repository_api_request.pyi
+-rw-r--r--   0        0        0     3072 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_signing_repositories_attributes.py
+-rw-r--r--   0        0        0     3072 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_signing_repositories_attributes.pyi
+-rw-r--r--   0        0        0    13448 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/models/__init__.py
+-rw-r--r--   0        0        0    13274 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/__init__.py
+-rw-r--r--   0        0        0     6485 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/get.py
+-rw-r--r--   0        0        0     6371 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/get.pyi
+-rw-r--r--   0        0        0    10757 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/post.py
+-rw-r--r--   0        0        0    10613 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/post.pyi
+-rw-r--r--   0        0        0      341 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/__init__.py
+-rw-r--r--   0        0        0     9022 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/delete.py
+-rw-r--r--   0        0        0     8847 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/delete.pyi
+-rw-r--r--   0        0        0     8970 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/get.py
+-rw-r--r--   0        0        0     8795 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/get.pyi
+-rw-r--r--   0        0        0    13200 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/put.py
+-rw-r--r--   0        0        0    13026 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/put.pyi
+-rw-r--r--   0        0        0      357 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_enable/__init__.py
+-rw-r--r--   0        0        0    11023 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_enable/put.py
+-rw-r--r--   0        0        0    10849 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_enable/put.pyi
+-rw-r--r--   0        0        0      389 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/__init__.py
+-rw-r--r--   0        0        0     9106 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/delete.py
+-rw-r--r--   0        0        0     8931 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/delete.pyi
+-rw-r--r--   0        0        0      295 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets/__init__.py
+-rw-r--r--   0        0        0    10679 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets/get.py
+-rw-r--r--   0        0        0    10565 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets/get.pyi
+-rw-r--r--   0        0        0      301 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/__init__.py
+-rw-r--r--   0        0        0     8763 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/delete.py
+-rw-r--r--   0        0        0     8618 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/delete.pyi
+-rw-r--r--   0        0        0    10408 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/get.py
+-rw-r--r--   0        0        0    10264 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/get.pyi
+-rw-r--r--   0        0        0      342 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_azureblobstore_test_connection/__init__.py
+-rw-r--r--   0        0        0    10907 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_azureblobstore_test_connection/post.py
+-rw-r--r--   0        0        0    10763 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_azureblobstore_test_connection/post.pyi
+-rw-r--r--   0        0        0      303 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores/__init__.py
+-rw-r--r--   0        0        0     8340 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores/get.py
+-rw-r--r--   0        0        0     8287 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores/get.pyi
+-rw-r--r--   0        0        0      315 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure/__init__.py
+-rw-r--r--   0        0        0    10603 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure/post.py
+-rw-r--r--   0        0        0    10489 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure/post.pyi
+-rw-r--r--   0        0        0      325 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/__init__.py
+-rw-r--r--   0        0        0    10498 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/get.py
+-rw-r--r--   0        0        0    10354 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/get.pyi
+-rw-r--r--   0        0        0    13068 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/put.py
+-rw-r--r--   0        0        0    12924 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/put.pyi
+-rw-r--r--   0        0        0      313 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file/__init__.py
+-rw-r--r--   0        0        0    10395 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file/post.py
+-rw-r--r--   0        0        0    10302 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file/post.pyi
+-rw-r--r--   0        0        0      323 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/__init__.py
+-rw-r--r--   0        0        0    10401 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/get.py
+-rw-r--r--   0        0        0    10287 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/get.pyi
+-rw-r--r--   0        0        0    12860 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/put.py
+-rw-r--r--   0        0        0    12737 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/put.pyi
+-rw-r--r--   0        0        0      315 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group/__init__.py
+-rw-r--r--   0        0        0    10412 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group/post.py
+-rw-r--r--   0        0        0    10319 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group/post.pyi
+-rw-r--r--   0        0        0      385 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/__init__.py
+-rw-r--r--   0        0        0    10709 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/post.py
+-rw-r--r--   0        0        0    10595 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/post.pyi
+-rw-r--r--   0        0        0      325 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/__init__.py
+-rw-r--r--   0        0        0    10416 2023-05-26 16:14:06.937424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/get.py
+-rw-r--r--   0        0        0    10302 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/get.pyi
+-rw-r--r--   0        0        0    12877 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/put.py
+-rw-r--r--   0        0        0    12754 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/put.pyi
+-rw-r--r--   0        0        0      313 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name/__init__.py
+-rw-r--r--   0        0        0     8260 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name/delete.py
+-rw-r--r--   0        0        0     8197 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name/delete.pyi
+-rw-r--r--   0        0        0      338 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name_quota_status/__init__.py
+-rw-r--r--   0        0        0     9596 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name_quota_status/get.py
+-rw-r--r--   0        0        0     9542 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name_quota_status/get.pyi
+-rw-r--r--   0        0        0      309 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3/__init__.py
+-rw-r--r--   0        0        0    10578 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3/post.py
+-rw-r--r--   0        0        0    10464 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3/post.pyi
+-rw-r--r--   0        0        0      319 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/__init__.py
+-rw-r--r--   0        0        0    10474 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/get.py
+-rw-r--r--   0        0        0    10330 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/get.pyi
+-rw-r--r--   0        0        0    13043 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/put.py
+-rw-r--r--   0        0        0    12899 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/put.pyi
+-rw-r--r--   0        0        0      303 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/__init__.py
+-rw-r--r--   0        0        0    10739 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/get.py
+-rw-r--r--   0        0        0    10625 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/get.pyi
+-rw-r--r--   0        0        0    12630 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/post.py
+-rw-r--r--   0        0        0    12546 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/__init__.py
+-rw-r--r--   0        0        0     8811 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/delete.py
+-rw-r--r--   0        0        0     8666 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/delete.pyi
+-rw-r--r--   0        0        0    10468 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/get.py
+-rw-r--r--   0        0        0    10324 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/__init__.py
+-rw-r--r--   0        0        0     6121 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/delete.py
+-rw-r--r--   0        0        0     6067 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/delete.pyi
+-rw-r--r--   0        0        0     8036 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/get.py
+-rw-r--r--   0        0        0     7952 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/get.pyi
+-rw-r--r--   0        0        0    10009 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/put.py
+-rw-r--r--   0        0        0     9895 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/put.pyi
+-rw-r--r--   0        0        0      307 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email_verify/__init__.py
+-rw-r--r--   0        0        0    11555 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email_verify/post.py
+-rw-r--r--   0        0        0    11471 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email_verify/post.pyi
+-rw-r--r--   0        0        0      336 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_format_upload_specs/__init__.py
+-rw-r--r--   0        0        0     9522 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_format_upload_specs/get.py
+-rw-r--r--   0        0        0     9468 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_format_upload_specs/get.pyi
+-rw-r--r--   0        0        0      322 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_upload_specs/__init__.py
+-rw-r--r--   0        0        0     8180 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_upload_specs/get.py
+-rw-r--r--   0        0        0     8127 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_upload_specs/get.pyi
+-rw-r--r--   0        0        0      287 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/__init__.py
+-rw-r--r--   0        0        0     5991 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/get.py
+-rw-r--r--   0        0        0     5937 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/get.pyi
+-rw-r--r--   0        0        0    10025 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/put.py
+-rw-r--r--   0        0        0     9971 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/put.pyi
+-rw-r--r--   0        0        0      303 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_disable/__init__.py
+-rw-r--r--   0        0        0     6198 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_disable/post.py
+-rw-r--r--   0        0        0     6114 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_disable/post.pyi
+-rw-r--r--   0        0        0      301 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_enable/__init__.py
+-rw-r--r--   0        0        0     6186 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_enable/post.py
+-rw-r--r--   0        0        0     6102 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_enable/post.pyi
+-rw-r--r--   0        0        0      322 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_verify_connection/__init__.py
+-rw-r--r--   0        0        0     5997 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_verify_connection/post.py
+-rw-r--r--   0        0        0     5943 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_verify_connection/post.pyi
+-rw-r--r--   0        0        0      315 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_bounce/__init__.py
+-rw-r--r--   0        0        0    10009 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_bounce/put.py
+-rw-r--r--   0        0        0     9946 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_bounce/put.pyi
+-rw-r--r--   0        0        0      313 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/__init__.py
+-rw-r--r--   0        0        0     7474 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/get.py
+-rw-r--r--   0        0        0     7419 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/get.pyi
+-rw-r--r--   0        0        0    10052 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/put.py
+-rw-r--r--   0        0        0     9989 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/put.pyi
+-rw-r--r--   0        0        0      300 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only/__init__.py
+-rw-r--r--   0        0        0     7485 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only/get.py
+-rw-r--r--   0        0        0     7431 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only/get.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_force_release/__init__.py
+-rw-r--r--   0        0        0     6528 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_force_release/post.py
+-rw-r--r--   0        0        0     6414 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_force_release/post.pyi
+-rw-r--r--   0        0        0      314 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_freeze/__init__.py
+-rw-r--r--   0        0        0     6442 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_freeze/post.py
+-rw-r--r--   0        0        0     6328 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_freeze/post.pyi
+-rw-r--r--   0        0        0      316 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_release/__init__.py
+-rw-r--r--   0        0        0     6454 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_release/post.py
+-rw-r--r--   0        0        0     6340 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_release/post.pyi
+-rw-r--r--   0        0        0      307 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories/__init__.py
+-rw-r--r--   0        0        0     8241 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories/get.py
+-rw-r--r--   0        0        0     8188 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories/get.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted/__init__.py
+-rw-r--r--   0        0        0    10924 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted/post.py
+-rw-r--r--   0        0        0    10771 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9675 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9621 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    13151 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12998 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy/__init__.py
+-rw-r--r--   0        0        0    10920 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy/post.py
+-rw-r--r--   0        0        0    10767 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy/post.pyi
+-rw-r--r--   0        0        0      359 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9672 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9618 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    13147 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12994 2023-05-26 16:14:06.941424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group/__init__.py
+-rw-r--r--   0        0        0    10653 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group/post.py
+-rw-r--r--   0        0        0    10530 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12880 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/put.py
+-rw-r--r--   0        0        0    12757 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      333 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted/__init__.py
+-rw-r--r--   0        0        0    10657 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted/post.py
+-rw-r--r--   0        0        0    10534 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted/post.pyi
+-rw-r--r--   0        0        0      365 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12884 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12761 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy/__init__.py
+-rw-r--r--   0        0        0    10653 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy/post.py
+-rw-r--r--   0        0        0    10530 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9689 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9635 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12880 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12757 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      339 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy/__init__.py
+-rw-r--r--   0        0        0    10957 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy/post.py
+-rw-r--r--   0        0        0    10804 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy/post.pyi
+-rw-r--r--   0        0        0      371 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12896 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12773 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy/__init__.py
+-rw-r--r--   0        0        0    10941 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy/post.py
+-rw-r--r--   0        0        0    10788 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    13168 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    13015 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy/__init__.py
+-rw-r--r--   0        0        0    10941 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy/post.py
+-rw-r--r--   0        0        0    10788 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12880 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12757 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      333 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group/__init__.py
+-rw-r--r--   0        0        0    10657 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group/post.py
+-rw-r--r--   0        0        0    10534 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group/post.pyi
+-rw-r--r--   0        0        0      365 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    13172 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/put.py
+-rw-r--r--   0        0        0    13019 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      335 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted/__init__.py
+-rw-r--r--   0        0        0    10661 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted/post.py
+-rw-r--r--   0        0        0    10538 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted/post.pyi
+-rw-r--r--   0        0        0      367 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    13176 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    13023 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      333 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy/__init__.py
+-rw-r--r--   0        0        0    10657 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy/post.py
+-rw-r--r--   0        0        0    10534 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy/post.pyi
+-rw-r--r--   0        0        0      365 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    13172 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    13019 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      335 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted/__init__.py
+-rw-r--r--   0        0        0    10663 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted/post.py
+-rw-r--r--   0        0        0    10540 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted/post.pyi
+-rw-r--r--   0        0        0      367 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12890 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12767 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      325 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group/__init__.py
+-rw-r--r--   0        0        0    10943 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group/post.py
+-rw-r--r--   0        0        0    10790 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group/post.pyi
+-rw-r--r--   0        0        0      357 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    13170 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/put.py
+-rw-r--r--   0        0        0    13017 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      325 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy/__init__.py
+-rw-r--r--   0        0        0    10943 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy/post.py
+-rw-r--r--   0        0        0    10790 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy/post.pyi
+-rw-r--r--   0        0        0      357 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    13170 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    13017 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted/__init__.py
+-rw-r--r--   0        0        0    10941 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted/post.py
+-rw-r--r--   0        0        0    10788 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12880 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12757 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy/__init__.py
+-rw-r--r--   0        0        0    10937 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy/post.py
+-rw-r--r--   0        0        0    10784 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12876 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12753 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group/__init__.py
+-rw-r--r--   0        0        0    10627 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group/post.py
+-rw-r--r--   0        0        0    10504 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9681 2023-05-26 16:14:06.945424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/get.py
+-rw-r--r--   0        0        0     9627 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12854 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/put.py
+-rw-r--r--   0        0        0    12731 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      333 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted/__init__.py
+-rw-r--r--   0        0        0    10644 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted/post.py
+-rw-r--r--   0        0        0    10521 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted/post.pyi
+-rw-r--r--   0        0        0      365 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9681 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9627 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12871 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12748 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy/__init__.py
+-rw-r--r--   0        0        0    10640 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy/post.py
+-rw-r--r--   0        0        0    10517 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9678 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9624 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12867 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12744 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group/__init__.py
+-rw-r--r--   0        0        0    10632 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group/post.py
+-rw-r--r--   0        0        0    10509 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group/post.pyi
+-rw-r--r--   0        0        0      359 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9709 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/get.py
+-rw-r--r--   0        0        0     9646 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12859 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/put.py
+-rw-r--r--   0        0        0    12736 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted/__init__.py
+-rw-r--r--   0        0        0    10636 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted/post.py
+-rw-r--r--   0        0        0    10513 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12863 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12740 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy/__init__.py
+-rw-r--r--   0        0        0    10645 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy/post.py
+-rw-r--r--   0        0        0    10522 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy/post.pyi
+-rw-r--r--   0        0        0      359 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9683 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9629 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12872 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12749 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group/__init__.py
+-rw-r--r--   0        0        0    10653 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group/post.py
+-rw-r--r--   0        0        0    10530 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12880 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/put.py
+-rw-r--r--   0        0        0    12757 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      333 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted/__init__.py
+-rw-r--r--   0        0        0    10657 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted/post.py
+-rw-r--r--   0        0        0    10534 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted/post.pyi
+-rw-r--r--   0        0        0      365 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12884 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12761 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy/__init__.py
+-rw-r--r--   0        0        0    10653 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy/post.py
+-rw-r--r--   0        0        0    10530 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9689 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9635 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12880 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12757 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      325 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy/__init__.py
+-rw-r--r--   0        0        0    10920 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy/post.py
+-rw-r--r--   0        0        0    10776 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy/post.pyi
+-rw-r--r--   0        0        0      357 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12859 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12745 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group/__init__.py
+-rw-r--r--   0        0        0    10649 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group/post.py
+-rw-r--r--   0        0        0    10526 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12876 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/put.py
+-rw-r--r--   0        0        0    12753 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted/__init__.py
+-rw-r--r--   0        0        0    10653 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted/post.py
+-rw-r--r--   0        0        0    10530 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12880 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12757 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy/__init__.py
+-rw-r--r--   0        0        0    10649 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy/post.py
+-rw-r--r--   0        0        0    10526 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12876 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12753 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      323 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group/__init__.py
+-rw-r--r--   0        0        0    10916 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group/post.py
+-rw-r--r--   0        0        0    10772 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group/post.pyi
+-rw-r--r--   0        0        0      355 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12855 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/put.py
+-rw-r--r--   0        0        0    12741 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      325 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted/__init__.py
+-rw-r--r--   0        0        0    10920 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted/post.py
+-rw-r--r--   0        0        0    10776 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted/post.pyi
+-rw-r--r--   0        0        0      357 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12859 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12745 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      323 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy/__init__.py
+-rw-r--r--   0        0        0    10916 2023-05-26 16:14:06.949424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy/post.py
+-rw-r--r--   0        0        0    10772 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy/post.pyi
+-rw-r--r--   0        0        0      355 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    13143 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12999 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group/__init__.py
+-rw-r--r--   0        0        0    10632 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group/post.py
+-rw-r--r--   0        0        0    10509 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group/post.pyi
+-rw-r--r--   0        0        0      359 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9681 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/get.py
+-rw-r--r--   0        0        0     9627 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12859 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/put.py
+-rw-r--r--   0        0        0    12736 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted/__init__.py
+-rw-r--r--   0        0        0    10636 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted/post.py
+-rw-r--r--   0        0        0    10513 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9684 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9630 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12863 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12740 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy/__init__.py
+-rw-r--r--   0        0        0    10632 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy/post.py
+-rw-r--r--   0        0        0    10509 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy/post.pyi
+-rw-r--r--   0        0        0      359 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9681 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9627 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12859 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12736 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      339 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/__init__.py
+-rw-r--r--   0        0        0     8914 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/delete.py
+-rw-r--r--   0        0        0     8769 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/delete.pyi
+-rw-r--r--   0        0        0    10504 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/get.py
+-rw-r--r--   0        0        0    10360 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/get.pyi
+-rw-r--r--   0        0        0      364 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/__init__.py
+-rw-r--r--   0        0        0     9092 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/delete.py
+-rw-r--r--   0        0        0     8947 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/delete.pyi
+-rw-r--r--   0        0        0     9356 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/post.py
+-rw-r--r--   0        0        0     9181 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/post.pyi
+-rw-r--r--   0        0        0      372 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/__init__.py
+-rw-r--r--   0        0        0     9210 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/post.py
+-rw-r--r--   0        0        0     9035 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/post.pyi
+-rw-r--r--   0        0        0      366 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/__init__.py
+-rw-r--r--   0        0        0     9213 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/post.py
+-rw-r--r--   0        0        0     9038 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/post.pyi
+-rw-r--r--   0        0        0      337 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group/__init__.py
+-rw-r--r--   0        0        0    10666 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group/post.py
+-rw-r--r--   0        0        0    10543 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group/post.pyi
+-rw-r--r--   0        0        0      369 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12893 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/put.py
+-rw-r--r--   0        0        0    12770 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      339 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted/__init__.py
+-rw-r--r--   0        0        0    10670 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted/post.py
+-rw-r--r--   0        0        0    10547 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted/post.pyi
+-rw-r--r--   0        0        0      371 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9695 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9641 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12897 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12774 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      337 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy/__init__.py
+-rw-r--r--   0        0        0    10666 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy/post.py
+-rw-r--r--   0        0        0    10543 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy/post.pyi
+-rw-r--r--   0        0        0      369 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12893 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12770 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group/__init__.py
+-rw-r--r--   0        0        0    10645 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group/post.py
+-rw-r--r--   0        0        0    10522 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group/post.pyi
+-rw-r--r--   0        0        0      359 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/get.pyi
+-rw-r--r--   0        0        0    12872 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/put.py
+-rw-r--r--   0        0        0    12749 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/put.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted/__init__.py
+-rw-r--r--   0        0        0    10649 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted/post.py
+-rw-r--r--   0        0        0    10526 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/__init__.py
+-rw-r--r--   0        0        0     9686 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/get.py
+-rw-r--r--   0        0        0     9632 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/get.pyi
+-rw-r--r--   0        0        0    12876 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/put.py
+-rw-r--r--   0        0        0    12753 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy/__init__.py
+-rw-r--r--   0        0        0    10645 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy/post.py
+-rw-r--r--   0        0        0    10522 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy/post.pyi
+-rw-r--r--   0        0        0      359 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/__init__.py
+-rw-r--r--   0        0        0     9692 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/get.py
+-rw-r--r--   0        0        0     9638 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/get.pyi
+-rw-r--r--   0        0        0    12872 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/put.py
+-rw-r--r--   0        0        0    12749 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/put.pyi
+-rw-r--r--   0        0        0      321 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repository_settings/__init__.py
+-rw-r--r--   0        0        0     8870 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repository_settings/get.py
+-rw-r--r--   0        0        0     8757 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repository_settings/get.pyi
+-rw-r--r--   0        0        0      308 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/__init__.py
+-rw-r--r--   0        0        0     8537 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/get.py
+-rw-r--r--   0        0        0     8454 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/get.pyi
+-rw-r--r--   0        0        0    10279 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/post.py
+-rw-r--r--   0        0        0    10165 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/post.pyi
+-rw-r--r--   0        0        0      318 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/__init__.py
+-rw-r--r--   0        0        0     8572 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/delete.py
+-rw-r--r--   0        0        0     8457 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/delete.pyi
+-rw-r--r--   0        0        0    10172 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/get.py
+-rw-r--r--   0        0        0    10058 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/get.pyi
+-rw-r--r--   0        0        0    12722 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/put.py
+-rw-r--r--   0        0        0    12578 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/put.pyi
+-rw-r--r--   0        0        0      295 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/__init__.py
+-rw-r--r--   0        0        0     8099 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/get.py
+-rw-r--r--   0        0        0     8046 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/get.pyi
+-rw-r--r--   0        0        0    10067 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/post.py
+-rw-r--r--   0        0        0     9983 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/post.pyi
+-rw-r--r--   0        0        0      305 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/__init__.py
+-rw-r--r--   0        0        0     8154 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/delete.py
+-rw-r--r--   0        0        0     8069 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/delete.pyi
+-rw-r--r--   0        0        0     9750 2023-05-26 16:14:06.953424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/get.py
+-rw-r--r--   0        0        0     9666 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/get.pyi
+-rw-r--r--   0        0        0    12535 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/put.py
+-rw-r--r--   0        0        0    12421 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/put.pyi
+-rw-r--r--   0        0        0      313 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name_run/__init__.py
+-rw-r--r--   0        0        0    16672 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name_run/post.py
+-rw-r--r--   0        0        0    16558 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name_run/post.pyi
+-rw-r--r--   0        0        0      295 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search/__init__.py
+-rw-r--r--   0        0        0    22446 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search/get.py
+-rw-r--r--   0        0        0    22080 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search/get.pyi
+-rw-r--r--   0        0        0      309 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets/__init__.py
+-rw-r--r--   0        0        0    22506 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets/get.py
+-rw-r--r--   0        0        0    22140 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets/get.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets_download/__init__.py
+-rw-r--r--   0        0        0    20854 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets_download/get.py
+-rw-r--r--   0        0        0    20457 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets_download/get.pyi
+-rw-r--r--   0        0        0      319 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/__init__.py
+-rw-r--r--   0        0        0     7831 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/get.py
+-rw-r--r--   0        0        0     7747 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/get.pyi
+-rw-r--r--   0        0        0    11892 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/put.py
+-rw-r--r--   0        0        0    11808 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/put.pyi
+-rw-r--r--   0        0        0      330 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/__init__.py
+-rw-r--r--   0        0        0     6568 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/get.py
+-rw-r--r--   0        0        0     6454 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/get.pyi
+-rw-r--r--   0        0        0    10218 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/put.py
+-rw-r--r--   0        0        0    10104 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/put.pyi
+-rw-r--r--   0        0        0      353 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/__init__.py
+-rw-r--r--   0        0        0     6507 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/post.py
+-rw-r--r--   0        0        0     6393 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/post.pyi
+-rw-r--r--   0        0        0      365 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/__init__.py
+-rw-r--r--   0        0        0    10539 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/post.py
+-rw-r--r--   0        0        0    10395 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/post.pyi
+-rw-r--r--   0        0        0      334 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/__init__.py
+-rw-r--r--   0        0        0     8677 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/get.py
+-rw-r--r--   0        0        0     8594 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/get.pyi
+-rw-r--r--   0        0        0    10707 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/post.py
+-rw-r--r--   0        0        0    10584 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/post.pyi
+-rw-r--r--   0        0        0      344 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/__init__.py
+-rw-r--r--   0        0        0     8613 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/delete.py
+-rw-r--r--   0        0        0     8498 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/delete.pyi
+-rw-r--r--   0        0        0     9973 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/get.py
+-rw-r--r--   0        0        0     9889 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/get.pyi
+-rw-r--r--   0        0        0    12858 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/put.py
+-rw-r--r--   0        0        0    12735 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/put.pyi
+-rw-r--r--   0        0        0      307 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_jwt/__init__.py
+-rw-r--r--   0        0        0     6187 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_jwt/put.py
+-rw-r--r--   0        0        0     6103 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_jwt/put.pyi
+-rw-r--r--   0        0        0      309 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/__init__.py
+-rw-r--r--   0        0        0     6545 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/get.py
+-rw-r--r--   0        0        0     6431 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/get.pyi
+-rw-r--r--   0        0        0    10582 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/post.py
+-rw-r--r--   0        0        0    10468 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/post.pyi
+-rw-r--r--   0        0        0      334 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_change_order/__init__.py
+-rw-r--r--   0        0        0    11198 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_change_order/post.py
+-rw-r--r--   0        0        0    11083 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_change_order/post.pyi
+-rw-r--r--   0        0        0      319 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/__init__.py
+-rw-r--r--   0        0        0     8839 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/delete.py
+-rw-r--r--   0        0        0     8694 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/delete.pyi
+-rw-r--r--   0        0        0     8785 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/get.py
+-rw-r--r--   0        0        0     8640 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/get.pyi
+-rw-r--r--   0        0        0    13025 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/put.py
+-rw-r--r--   0        0        0    12881 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/put.pyi
+-rw-r--r--   0        0        0      321 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges/__init__.py
+-rw-r--r--   0        0        0     8509 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges/get.py
+-rw-r--r--   0        0        0     8426 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges/get.pyi
+-rw-r--r--   0        0        0      345 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application/__init__.py
+-rw-r--r--   0        0        0    10247 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application/post.py
+-rw-r--r--   0        0        0    10154 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application/post.pyi
+-rw-r--r--   0        0        0      375 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application_privilege_name/__init__.py
+-rw-r--r--   0        0        0    12755 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application_privilege_name/put.py
+-rw-r--r--   0        0        0    12632 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application_privilege_name/put.pyi
+-rw-r--r--   0        0        0      351 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/__init__.py
+-rw-r--r--   0        0        0     8514 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/delete.py
+-rw-r--r--   0        0        0     8399 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/delete.pyi
+-rw-r--r--   0        0        0    10205 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/get.py
+-rw-r--r--   0        0        0    10091 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/get.pyi
+-rw-r--r--   0        0        0      354 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin/__init__.py
+-rw-r--r--   0        0        0    10264 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin/post.py
+-rw-r--r--   0        0        0    10171 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin/post.pyi
+-rw-r--r--   0        0        0      384 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/__init__.py
+-rw-r--r--   0        0        0    12772 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/put.py
+-rw-r--r--   0        0        0    12649 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/put.pyi
+-rw-r--r--   0        0        0      375 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector/__init__.py
+-rw-r--r--   0        0        0    10306 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector/post.py
+-rw-r--r--   0        0        0    10213 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector/post.pyi
+-rw-r--r--   0        0        0      405 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/__init__.py
+-rw-r--r--   0        0        0    12814 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/put.py
+-rw-r--r--   0        0        0    12691 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/put.pyi
+-rw-r--r--   0        0        0      352 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view/post.py
+-rw-r--r--   0        0        0    10167 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view/post.pyi
+-rw-r--r--   0        0        0      382 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/__init__.py
+-rw-r--r--   0        0        0    12768 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/put.py
+-rw-r--r--   0        0        0    12645 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/put.pyi
+-rw-r--r--   0        0        0      335 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script/__init__.py
+-rw-r--r--   0        0        0    10217 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script/post.py
+-rw-r--r--   0        0        0    10133 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script/post.pyi
+-rw-r--r--   0        0        0      365 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script_privilege_name/__init__.py
+-rw-r--r--   0        0        0    12725 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script_privilege_name/put.py
+-rw-r--r--   0        0        0    12611 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script_privilege_name/put.pyi
+-rw-r--r--   0        0        0      339 2023-05-26 16:14:06.957424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard/__init__.py
+-rw-r--r--   0        0        0    10212 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard/post.py
+-rw-r--r--   0        0        0    10128 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard/post.pyi
+-rw-r--r--   0        0        0      369 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/__init__.py
+-rw-r--r--   0        0        0    12720 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/put.py
+-rw-r--r--   0        0        0    12606 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/__init__.py
+-rw-r--r--   0        0        0     8163 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/get.py
+-rw-r--r--   0        0        0     8109 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/get.pyi
+-rw-r--r--   0        0        0    11017 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/put.py
+-rw-r--r--   0        0        0    10954 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/put.pyi
+-rw-r--r--   0        0        0      333 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_available/__init__.py
+-rw-r--r--   0        0        0     8159 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_available/get.py
+-rw-r--r--   0        0        0     8106 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_available/get.pyi
+-rw-r--r--   0        0        0      311 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/__init__.py
+-rw-r--r--   0        0        0    10892 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/get.py
+-rw-r--r--   0        0        0    10778 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/get.pyi
+-rw-r--r--   0        0        0    11580 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/post.py
+-rw-r--r--   0        0        0    11496 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/post.pyi
+-rw-r--r--   0        0        0      317 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/__init__.py
+-rw-r--r--   0        0        0     8022 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/delete.py
+-rw-r--r--   0        0        0     7937 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/delete.pyi
+-rw-r--r--   0        0        0    12499 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/get.py
+-rw-r--r--   0        0        0    12355 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/get.pyi
+-rw-r--r--   0        0        0    11862 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/put.py
+-rw-r--r--   0        0        0    11778 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/put.pyi
+-rw-r--r--   0        0        0      309 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/__init__.py
+-rw-r--r--   0        0        0     6670 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/delete.py
+-rw-r--r--   0        0        0     6556 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/delete.pyi
+-rw-r--r--   0        0        0     6904 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/get.py
+-rw-r--r--   0        0        0     6760 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/get.pyi
+-rw-r--r--   0        0        0    11465 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/put.py
+-rw-r--r--   0        0        0    11291 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/put.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_metadata/__init__.py
+-rw-r--r--   0        0        0     6815 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_metadata/get.py
+-rw-r--r--   0        0        0     6671 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_metadata/get.pyi
+-rw-r--r--   0        0        0      317 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_pem/__init__.py
+-rw-r--r--   0        0        0     7087 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_pem/get.py
+-rw-r--r--   0        0        0     6943 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_pem/get.pyi
+-rw-r--r--   0        0        0      307 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl/__init__.py
+-rw-r--r--   0        0        0    11057 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl/get.py
+-rw-r--r--   0        0        0    10943 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl/get.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/__init__.py
+-rw-r--r--   0        0        0     8702 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/get.py
+-rw-r--r--   0        0        0     8619 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/get.pyi
+-rw-r--r--   0        0        0    11994 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/post.py
+-rw-r--r--   0        0        0    11880 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/post.pyi
+-rw-r--r--   0        0        0      335 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore_id/__init__.py
+-rw-r--r--   0        0        0     7894 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore_id/delete.py
+-rw-r--r--   0        0        0     7839 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore_id/delete.pyi
+-rw-r--r--   0        0        0      324 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_sources/__init__.py
+-rw-r--r--   0        0        0     8554 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_sources/get.py
+-rw-r--r--   0        0        0     8471 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_sources/get.pyi
+-rw-r--r--   0        0        0      322 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/__init__.py
+-rw-r--r--   0        0        0     6347 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/delete.py
+-rw-r--r--   0        0        0     6285 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/delete.pyi
+-rw-r--r--   0        0        0     7653 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/get.py
+-rw-r--r--   0        0        0     7599 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/get.pyi
+-rw-r--r--   0        0        0    11738 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/put.py
+-rw-r--r--   0        0        0    11684 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/put.pyi
+-rw-r--r--   0        0        0      311 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/__init__.py
+-rw-r--r--   0        0        0    11219 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/get.py
+-rw-r--r--   0        0        0    11105 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/get.pyi
+-rw-r--r--   0        0        0    12249 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/post.py
+-rw-r--r--   0        0        0    12135 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/post.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/__init__.py
+-rw-r--r--   0        0        0     8397 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/delete.py
+-rw-r--r--   0        0        0     8282 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/delete.pyi
+-rw-r--r--   0        0        0    12535 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/put.py
+-rw-r--r--   0        0        0    12421 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/put.pyi
+-rw-r--r--   0        0        0      358 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_change_password/__init__.py
+-rw-r--r--   0        0        0    12489 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_change_password/put.py
+-rw-r--r--   0        0        0    12374 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_change_password/put.pyi
+-rw-r--r--   0        0        0      371 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/__init__.py
+-rw-r--r--   0        0        0     9005 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/delete.py
+-rw-r--r--   0        0        0     8860 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/delete.pyi
+-rw-r--r--   0        0        0      311 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_delete/__init__.py
+-rw-r--r--   0        0        0    19869 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_delete/post.py
+-rw-r--r--   0        0        0    19694 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_delete/post.pyi
+-rw-r--r--   0        0        0      331 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_move_destination/__init__.py
+-rw-r--r--   0        0        0    21847 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_move_destination/post.py
+-rw-r--r--   0        0        0    21672 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_move_destination/post.pyi
+-rw-r--r--   0        0        0      295 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status/get.py
+-rw-r--r--   0        0        0     6185 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status/get.pyi
+-rw-r--r--   0        0        0      307 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_check/__init__.py
+-rw-r--r--   0        0        0     8565 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_check/get.py
+-rw-r--r--   0        0        0     8512 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_check/get.pyi
+-rw-r--r--   0        0        0      313 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_writable/__init__.py
+-rw-r--r--   0        0        0     6268 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_writable/get.py
+-rw-r--r--   0        0        0     6184 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_writable/get.pyi
+-rw-r--r--   0        0        0      319 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzip/__init__.py
+-rw-r--r--   0        0        0    10244 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzip/post.py
+-rw-r--r--   0        0        0    10182 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzip/post.pyi
+-rw-r--r--   0        0        0      327 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzippath/__init__.py
+-rw-r--r--   0        0        0    11771 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzippath/post.py
+-rw-r--r--   0        0        0    11717 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzippath/post.pyi
+-rw-r--r--   0        0        0      311 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/__init__.py
+-rw-r--r--   0        0        0     6265 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/delete.py
+-rw-r--r--   0        0        0     6203 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/delete.pyi
+-rw-r--r--   0        0        0     7679 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/get.py
+-rw-r--r--   0        0        0     7625 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/get.pyi
+-rw-r--r--   0        0        0    12254 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/post.py
+-rw-r--r--   0        0        0    12200 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/post.pyi
+-rw-r--r--   0        0        0      291 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/__init__.py
+-rw-r--r--   0        0        0     9750 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/get.py
+-rw-r--r--   0        0        0     9696 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/get.pyi
+-rw-r--r--   0        0        0    10106 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/post.py
+-rw-r--r--   0        0        0    10022 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/post.pyi
+-rw-r--r--   0        0        0      329 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/__init__.py
+-rw-r--r--   0        0        0    21076 2023-05-26 16:14:06.961424 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/delete.py
+-rw-r--r--   0        0        0    20991 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/delete.pyi
+-rw-r--r--   0        0        0    21292 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/post.py
+-rw-r--r--   0        0        0    21207 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/post.pyi
+-rw-r--r--   0        0        0      301 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/__init__.py
+-rw-r--r--   0        0        0     8138 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/delete.py
+-rw-r--r--   0        0        0     8053 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/delete.pyi
+-rw-r--r--   0        0        0     9713 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/get.py
+-rw-r--r--   0        0        0     9629 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/get.pyi
+-rw-r--r--   0        0        0    14319 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/put.py
+-rw-r--r--   0        0        0    14205 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/put.pyi
+-rw-r--r--   0        0        0      293 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks/__init__.py
+-rw-r--r--   0        0        0     9672 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks/get.py
+-rw-r--r--   0        0        0     9618 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks/get.pyi
+-rw-r--r--   0        0        0      299 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id/__init__.py
+-rw-r--r--   0        0        0     9823 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id/get.py
+-rw-r--r--   0        0        0     9739 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id/get.pyi
+-rw-r--r--   0        0        0      307 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_run/__init__.py
+-rw-r--r--   0        0        0     8352 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_run/post.py
+-rw-r--r--   0        0        0     8237 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_run/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_stop/__init__.py
+-rw-r--r--   0        0        0     8364 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_stop/post.py
+-rw-r--r--   0        0        0     8249 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_stop/post.pyi
+-rw-r--r--   0        0        0    10722 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/rest.py
+-rw-r--r--   0        0        0    97679 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/nexus_sdk/schemas.py
+-rw-r--r--   0        0        0      674 2023-05-26 16:14:06.965425 sonatype_nexus_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0   101895 1970-01-01 00:00:00.000000 sonatype_nexus_sdk-0.1.3/PKG-INFO
```

### Comparing `sonatype_nexus_sdk-0.1.0/README.md` & `sonatype_nexus_sdk-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,44 @@
+Metadata-Version: 2.1
+Name: sonatype-nexus-sdk
+Version: 0.1.3
+Summary: Python SDK for Sonatype Products such as Nexus Repository Manager, Lifecycle and IQ Server 
+License: MIT
+Author: Justin Bailey
+Author-email: justthered63@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
+Requires-Dist: frozendict (>=2.3.8,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: setuptools (>=67.8.0,<68.0.0)
+Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
+Requires-Dist: urllib3 (>=2.0.2,<3.0.0)
+Description-Content-Type: text/markdown
+
 # Sonatype Nexus SDK for Python
 
 ## Requirements
 
 Python `^3.9`
 
 ## Installation & Usage
 
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install sonatype-nexus-sdk
 ```
 
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-
-Then import the package:
-
-```python
-import nexus_sdk
-```
-
-### Setuptools
-
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-
-```sh
-python setup.py install --user
-```
-
-(or `sudo python setup.py install` to install the package for all users)
-
 Then import the package:
 
 ```python
 import nexus_sdk
 ```
 
 ## Getting Started
@@ -68,16 +71,14 @@
         api_instance.delete_asset(id)
     except nexus_sdk.ApiException as e:
         print("Exception when calling AssetsApi->delete_asset: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to _<http://localhost/service/rest>_
-
 | Class                                  | Method                                                                                                                       | HTTP request                                                                | Description                                                                                                   |
 | -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
 | _AssetsApi_                            | [**delete_asset**](docs/apis/tags/AssetsApi.md#delete_asset)                                                                 | **delete** /v1/assets/{id}                                                  | Delete a single asset                                                                                         |
 | _AssetsApi_                            | [**get_asset_by_id**](docs/apis/tags/AssetsApi.md#get_asset_by_id)                                                           | **get** /v1/assets/{id}                                                     | Get a single asset                                                                                            |
 | _AssetsApi_                            | [**get_assets**](docs/apis/tags/AssetsApi.md#get_assets)                                                                     | **get** /v1/assets                                                          | List assets                                                                                                   |
 | _AzureBlobStoreApi_                    | [**verify_connection2**](docs/apis/tags/AzureBlobStoreApi.md#verify_connection2)                                             | **post** /v1/azureblobstore/test-connection                                 | Verify connection using supplied Azure Blob Store settings                                                    |
 | _BlobStoreApi_                         | [**convert_blob_store_to_group**](docs/apis/tags/BlobStoreApi.md#convert_blob_store_to_group)                                | **post** /v1/blobstores/group/convert/{name}/{newNameForOriginal}           | Convert a blob store to a group blob store                                                                    |
@@ -348,194 +349,7 @@
 | _TagsApi_                              | [**get_tags**](docs/apis/tags/TagsApi.md#get_tags)                                                                           | **get** /v1/tags                                                            | List tags                                                                                                     |
 | _TagsApi_                              | [**replace**](docs/apis/tags/TagsApi.md#replace)                                                                             | **put** /v1/tags/{name}                                                     | Update a tags attributes                                                                                      |
 | _TasksApi_                             | [**get_task_by_id**](docs/apis/tags/TasksApi.md#get_task_by_id)                                                              | **get** /v1/tasks/{id}                                                      | Get a single task by id                                                                                       |
 | _TasksApi_                             | [**get_tasks**](docs/apis/tags/TasksApi.md#get_tasks)                                                                        | **get** /v1/tasks                                                           | List tasks                                                                                                    |
 | _TasksApi_                             | [**run**](docs/apis/tags/TasksApi.md#run)                                                                                    | **post** /v1/tasks/{id}/run                                                 | Run task                                                                                                      |
 | _TasksApi_                             | [**stop**](docs/apis/tags/TasksApi.md#stop)                                                                                  | **post** /v1/tasks/{id}/stop                                                | Stop task                                                                                                     |
 
-## Documentation For Models
-
-- [AbstractApiRepository](docs/models/AbstractApiRepository.md)
-- [AnonymousAccessSettingsXO](docs/models/AnonymousAccessSettingsXO.md)
-- [ApiCertificate](docs/models/ApiCertificate.md)
-- [ApiCreateUser](docs/models/ApiCreateUser.md)
-- [ApiEmailConfiguration](docs/models/ApiEmailConfiguration.md)
-- [ApiEmailValidation](docs/models/ApiEmailValidation.md)
-- [ApiLicenseDetailsXO](docs/models/ApiLicenseDetailsXO.md)
-- [ApiPrivilege](docs/models/ApiPrivilege.md)
-- [ApiPrivilegeApplicationRequest](docs/models/ApiPrivilegeApplicationRequest.md)
-- [ApiPrivilegeRepositoryAdminRequest](docs/models/ApiPrivilegeRepositoryAdminRequest.md)
-- [ApiPrivilegeRepositoryContentSelectorRequest](docs/models/ApiPrivilegeRepositoryContentSelectorRequest.md)
-- [ApiPrivilegeRepositoryViewRequest](docs/models/ApiPrivilegeRepositoryViewRequest.md)
-- [ApiPrivilegeScriptRequest](docs/models/ApiPrivilegeScriptRequest.md)
-- [ApiPrivilegeWildcardRequest](docs/models/ApiPrivilegeWildcardRequest.md)
-- [ApiUser](docs/models/ApiUser.md)
-- [ApiUserSource](docs/models/ApiUserSource.md)
-- [AptHostedApiRepository](docs/models/AptHostedApiRepository.md)
-- [AptHostedRepositoriesAttributes](docs/models/AptHostedRepositoriesAttributes.md)
-- [AptHostedRepositoryApiRequest](docs/models/AptHostedRepositoryApiRequest.md)
-- [AptProxyApiRepository](docs/models/AptProxyApiRepository.md)
-- [AptProxyRepositoriesAttributes](docs/models/AptProxyRepositoriesAttributes.md)
-- [AptProxyRepositoryApiRequest](docs/models/AptProxyRepositoryApiRequest.md)
-- [AptSigningRepositoriesAttributes](docs/models/AptSigningRepositoriesAttributes.md)
-- [AssetXO](docs/models/AssetXO.md)
-- [AzureBlobStoreApiAuthentication](docs/models/AzureBlobStoreApiAuthentication.md)
-- [AzureBlobStoreApiBucketConfiguration](docs/models/AzureBlobStoreApiBucketConfiguration.md)
-- [AzureBlobStoreApiModel](docs/models/AzureBlobStoreApiModel.md)
-- [AzureConnectionXO](docs/models/AzureConnectionXO.md)
-- [BaseTagXO](docs/models/BaseTagXO.md)
-- [BlobStoreApiSoftQuota](docs/models/BlobStoreApiSoftQuota.md)
-- [BlobStoreQuotaResultXO](docs/models/BlobStoreQuotaResultXO.md)
-- [BowerAttributes](docs/models/BowerAttributes.md)
-- [BowerGroupRepositoryApiRequest](docs/models/BowerGroupRepositoryApiRequest.md)
-- [BowerHostedRepositoryApiRequest](docs/models/BowerHostedRepositoryApiRequest.md)
-- [BowerProxyApiRepository](docs/models/BowerProxyApiRepository.md)
-- [BowerProxyRepositoryApiRequest](docs/models/BowerProxyRepositoryApiRequest.md)
-- [CleanupPolicyAttributes](docs/models/CleanupPolicyAttributes.md)
-- [CocoapodsProxyRepositoryApiRequest](docs/models/CocoapodsProxyRepositoryApiRequest.md)
-- [ComponentAttributes](docs/models/ComponentAttributes.md)
-- [ComponentXO](docs/models/ComponentXO.md)
-- [ConanProxyRepositoryApiRequest](docs/models/ConanProxyRepositoryApiRequest.md)
-- [CondaProxyRepositoryApiRequest](docs/models/CondaProxyRepositoryApiRequest.md)
-- [ContentSelectorApiCreateRequest](docs/models/ContentSelectorApiCreateRequest.md)
-- [ContentSelectorApiResponse](docs/models/ContentSelectorApiResponse.md)
-- [ContentSelectorApiUpdateRequest](docs/models/ContentSelectorApiUpdateRequest.md)
-- [CreateLdapServerXo](docs/models/CreateLdapServerXo.md)
-- [CrowdApiXO](docs/models/CrowdApiXO.md)
-- [DockerAttributes](docs/models/DockerAttributes.md)
-- [DockerGroupApiRepository](docs/models/DockerGroupApiRepository.md)
-- [DockerGroupRepositoryApiRequest](docs/models/DockerGroupRepositoryApiRequest.md)
-- [DockerHostedApiRepository](docs/models/DockerHostedApiRepository.md)
-- [DockerHostedRepositoryApiRequest](docs/models/DockerHostedRepositoryApiRequest.md)
-- [DockerHostedStorageAttributes](docs/models/DockerHostedStorageAttributes.md)
-- [DockerProxyApiRepository](docs/models/DockerProxyApiRepository.md)
-- [DockerProxyAttributes](docs/models/DockerProxyAttributes.md)
-- [DockerProxyRepositoryApiRequest](docs/models/DockerProxyRepositoryApiRequest.md)
-- [FileBlobStoreApiCreateRequest](docs/models/FileBlobStoreApiCreateRequest.md)
-- [FileBlobStoreApiModel](docs/models/FileBlobStoreApiModel.md)
-- [FileBlobStoreApiUpdateRequest](docs/models/FileBlobStoreApiUpdateRequest.md)
-- [GenericBlobStoreApiResponse](docs/models/GenericBlobStoreApiResponse.md)
-- [GitLfsHostedRepositoryApiRequest](docs/models/GitLfsHostedRepositoryApiRequest.md)
-- [GolangGroupRepositoryApiRequest](docs/models/GolangGroupRepositoryApiRequest.md)
-- [GolangProxyRepositoryApiRequest](docs/models/GolangProxyRepositoryApiRequest.md)
-- [GroupAttributes](docs/models/GroupAttributes.md)
-- [GroupBlobStoreApiCreateRequest](docs/models/GroupBlobStoreApiCreateRequest.md)
-- [GroupBlobStoreApiModel](docs/models/GroupBlobStoreApiModel.md)
-- [GroupBlobStoreApiResponse](docs/models/GroupBlobStoreApiResponse.md)
-- [GroupBlobStoreApiUpdateRequest](docs/models/GroupBlobStoreApiUpdateRequest.md)
-- [GroupDeployAttributes](docs/models/GroupDeployAttributes.md)
-- [HelmHostedRepositoryApiRequest](docs/models/HelmHostedRepositoryApiRequest.md)
-- [HelmProxyRepositoryApiRequest](docs/models/HelmProxyRepositoryApiRequest.md)
-- [HostedStorageAttributes](docs/models/HostedStorageAttributes.md)
-- [HttpClientAttributes](docs/models/HttpClientAttributes.md)
-- [HttpClientAttributesWithPreemptiveAuth](docs/models/HttpClientAttributesWithPreemptiveAuth.md)
-- [HttpClientConnectionAttributes](docs/models/HttpClientConnectionAttributes.md)
-- [HttpClientConnectionAuthenticationAttributes](docs/models/HttpClientConnectionAuthenticationAttributes.md)
-- [HttpClientConnectionAuthenticationAttributesWithPreemptive](docs/models/HttpClientConnectionAuthenticationAttributesWithPreemptive.md)
-- [IqConnectionVerificationXo](docs/models/IqConnectionVerificationXo.md)
-- [IqConnectionXo](docs/models/IqConnectionXo.md)
-- [MavenAttributes](docs/models/MavenAttributes.md)
-- [MavenGroupRepositoryApiRequest](docs/models/MavenGroupRepositoryApiRequest.md)
-- [MavenHostedApiRepository](docs/models/MavenHostedApiRepository.md)
-- [MavenHostedRepositoryApiRequest](docs/models/MavenHostedRepositoryApiRequest.md)
-- [MavenProxyApiRepository](docs/models/MavenProxyApiRepository.md)
-- [MavenProxyRepositoryApiRequest](docs/models/MavenProxyRepositoryApiRequest.md)
-- [NegativeCacheAttributes](docs/models/NegativeCacheAttributes.md)
-- [NpmAttributes](docs/models/NpmAttributes.md)
-- [NpmGroupRepositoryApiRequest](docs/models/NpmGroupRepositoryApiRequest.md)
-- [NpmHostedRepositoryApiRequest](docs/models/NpmHostedRepositoryApiRequest.md)
-- [NpmProxyApiRepository](docs/models/NpmProxyApiRepository.md)
-- [NpmProxyRepositoryApiRequest](docs/models/NpmProxyRepositoryApiRequest.md)
-- [NugetAttributes](docs/models/NugetAttributes.md)
-- [NugetGroupRepositoryApiRequest](docs/models/NugetGroupRepositoryApiRequest.md)
-- [NugetHostedRepositoryApiRequest](docs/models/NugetHostedRepositoryApiRequest.md)
-- [NugetProxyApiRepository](docs/models/NugetProxyApiRepository.md)
-- [NugetProxyRepositoryApiRequest](docs/models/NugetProxyRepositoryApiRequest.md)
-- [P2ProxyRepositoryApiRequest](docs/models/P2ProxyRepositoryApiRequest.md)
-- [Page](docs/models/Page.md)
-- [PageAssetXO](docs/models/PageAssetXO.md)
-- [PageComponentXO](docs/models/PageComponentXO.md)
-- [PageTagXO](docs/models/PageTagXO.md)
-- [PageTaskXO](docs/models/PageTaskXO.md)
-- [ProxyAttributes](docs/models/ProxyAttributes.md)
-- [PypiGroupRepositoryApiRequest](docs/models/PypiGroupRepositoryApiRequest.md)
-- [PypiHostedRepositoryApiRequest](docs/models/PypiHostedRepositoryApiRequest.md)
-- [PypiProxyRepositoryApiRequest](docs/models/PypiProxyRepositoryApiRequest.md)
-- [RGroupRepositoryApiRequest](docs/models/RGroupRepositoryApiRequest.md)
-- [RHostedRepositoryApiRequest](docs/models/RHostedRepositoryApiRequest.md)
-- [RProxyRepositoryApiRequest](docs/models/RProxyRepositoryApiRequest.md)
-- [RawAttributes](docs/models/RawAttributes.md)
-- [RawGroupRepositoryApiRequest](docs/models/RawGroupRepositoryApiRequest.md)
-- [RawHostedRepositoryApiRequest](docs/models/RawHostedRepositoryApiRequest.md)
-- [RawProxyRepositoryApiRequest](docs/models/RawProxyRepositoryApiRequest.md)
-- [ReadLdapServerXo](docs/models/ReadLdapServerXo.md)
-- [ReadOnlyState](docs/models/ReadOnlyState.md)
-- [RealmApiXO](docs/models/RealmApiXO.md)
-- [ReplicationAttributes](docs/models/ReplicationAttributes.md)
-- [ReplicationConnectionXO](docs/models/ReplicationConnectionXO.md)
-- [ReplicationEnableXO](docs/models/ReplicationEnableXO.md)
-- [RepositoryXO](docs/models/RepositoryXO.md)
-- [Result](docs/models/Result.md)
-- [RoleXORequest](docs/models/RoleXORequest.md)
-- [RoleXOResponse](docs/models/RoleXOResponse.md)
-- [RoutingRuleXO](docs/models/RoutingRuleXO.md)
-- [RubyGemsGroupRepositoryApiRequest](docs/models/RubyGemsGroupRepositoryApiRequest.md)
-- [RubyGemsHostedRepositoryApiRequest](docs/models/RubyGemsHostedRepositoryApiRequest.md)
-- [RubyGemsProxyRepositoryApiRequest](docs/models/RubyGemsProxyRepositoryApiRequest.md)
-- [S3BlobStoreApiAdvancedBucketConnection](docs/models/S3BlobStoreApiAdvancedBucketConnection.md)
-- [S3BlobStoreApiBucket](docs/models/S3BlobStoreApiBucket.md)
-- [S3BlobStoreApiBucketConfiguration](docs/models/S3BlobStoreApiBucketConfiguration.md)
-- [S3BlobStoreApiBucketSecurity](docs/models/S3BlobStoreApiBucketSecurity.md)
-- [S3BlobStoreApiEncryption](docs/models/S3BlobStoreApiEncryption.md)
-- [S3BlobStoreApiModel](docs/models/S3BlobStoreApiModel.md)
-- [SamlConfigurationXO](docs/models/SamlConfigurationXO.md)
-- [ScriptResultXO](docs/models/ScriptResultXO.md)
-- [ScriptXO](docs/models/ScriptXO.md)
-- [SimpleApiGroupDeployRepository](docs/models/SimpleApiGroupDeployRepository.md)
-- [SimpleApiGroupRepository](docs/models/SimpleApiGroupRepository.md)
-- [SimpleApiHostedRepository](docs/models/SimpleApiHostedRepository.md)
-- [SimpleApiProxyRepository](docs/models/SimpleApiProxyRepository.md)
-- [StackTraceElement](docs/models/StackTraceElement.md)
-- [StorageAttributes](docs/models/StorageAttributes.md)
-- [SupportZipGeneratorRequest](docs/models/SupportZipGeneratorRequest.md)
-- [SupportZipXO](docs/models/SupportZipXO.md)
-- [TagXO](docs/models/TagXO.md)
-- [TaskXO](docs/models/TaskXO.md)
-- [Throwable](docs/models/Throwable.md)
-- [UpdateLdapServerXo](docs/models/UpdateLdapServerXo.md)
-- [UploadDefinitionXO](docs/models/UploadDefinitionXO.md)
-- [UploadFieldDefinitionXO](docs/models/UploadFieldDefinitionXO.md)
-- [UserTokensApiModel](docs/models/UserTokensApiModel.md)
-- [YumAttributes](docs/models/YumAttributes.md)
-- [YumGroupRepositoryApiRequest](docs/models/YumGroupRepositoryApiRequest.md)
-- [YumHostedApiRepository](docs/models/YumHostedApiRepository.md)
-- [YumHostedRepositoryApiRequest](docs/models/YumHostedRepositoryApiRequest.md)
-- [YumProxyRepositoryApiRequest](docs/models/YumProxyRepositoryApiRequest.md)
-- [YumSigningRepositoriesAttributes](docs/models/YumSigningRepositoriesAttributes.md)
-
-## Documentation For Authorization
-
-Endpoints do not require authorization.
-
-## Author
-
-## Notes for Large OpenAPI documents
-
-If the OpenAPI document is large, imports in nexus_sdk.apis and nexus_sdk.models may fail with a
-RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
-
-Solution 1:
-Use specific imports for apis and models like:
-
-- `from nexus_sdk.apis.default_api import DefaultApi`
-- `from nexus_sdk.model.pet import Pet`
-
-Solution 1:
-Before importing the package, adjust the maximum recursion limit as shown below:
-
-```
-import sys
-sys.setrecursionlimit(1500)
-import nexus_sdk
-from nexus_sdk.apis import *
-from nexus_sdk.models import *
-```
```

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/__init__.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/api_client.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/path_to_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tag_to_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/__init__.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/assets_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/assets_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/azure_blob_store_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/azure_blob_store_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/blob_store_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/blob_store_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/components_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/components_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/content_selectors_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/content_selectors_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/email_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/email_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/formats_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/formats_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/lifecycle_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/lifecycle_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/manage_iq_server_configuration_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/manage_iq_server_configuration_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/product_licensing_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/product_licensing_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/read_only_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/read_only_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/replication_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/replication_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/repository_management_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/repository_management_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/routing_rules_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/routing_rules_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/script_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/script_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/search_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/search_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_atlassian_crowd_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_atlassian_crowd_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_certificates_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_certificates_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_anonymous_access_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_anonymous_access_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_jwt_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_jwt_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_ldap_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_ldap_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_privileges_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_privileges_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_realms_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_realms_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_roles_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_roles_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_saml_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_saml_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_user_tokens_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_user_tokens_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/security_management_users_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/security_management_users_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/staging_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/staging_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/status_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/status_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/support_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/support_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/tags_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/tags_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/apis/tags/tasks_api.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/apis/tags/tasks_api.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/configuration.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/exceptions.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/abstract_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/abstract_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/abstract_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/abstract_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/anonymous_access_settings_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/anonymous_access_settings_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/anonymous_access_settings_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/anonymous_access_settings_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_certificate.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_certificate.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_certificate.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_certificate.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_create_user.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_create_user.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_create_user.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_create_user.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_email_configuration.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_email_configuration.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_email_configuration.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_email_configuration.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_email_validation.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_email_validation.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_email_validation.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_email_validation.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_license_details_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_license_details_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_license_details_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_license_details_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_application_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_application_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_application_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_application_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_admin_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_admin_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_admin_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_admin_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_content_selector_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_content_selector_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_content_selector_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_content_selector_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_view_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_view_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_repository_view_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_repository_view_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_script_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_script_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_script_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_script_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_wildcard_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_wildcard_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_privilege_wildcard_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_privilege_wildcard_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_user.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_user.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_user.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_user.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_user_source.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_user_source.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/api_user_source.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/api_user_source.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_repositories_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_repositories_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_repositories_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_repositories_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_repositories_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_repositories_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_repositories_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_repositories_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_signing_repositories_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_signing_repositories_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/apt_signing_repositories_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/apt_signing_repositories_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/asset_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/asset_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/asset_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/asset_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_authentication.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_authentication.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_authentication.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_authentication.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_bucket_configuration.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_bucket_configuration.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_bucket_configuration.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_bucket_configuration.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_model.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_blob_store_api_model.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_blob_store_api_model.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_connection_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_connection_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/azure_connection_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/azure_connection_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/base_tag_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/base_tag_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/base_tag_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/base_tag_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/blob_store_api_soft_quota.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/blob_store_api_soft_quota.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/blob_store_api_soft_quota.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/blob_store_api_soft_quota.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/blob_store_quota_result_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/blob_store_quota_result_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/blob_store_quota_result_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/blob_store_quota_result_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_proxy_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_proxy_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_proxy_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/bower_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/bower_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/cleanup_policy_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/cleanup_policy_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/cleanup_policy_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/cleanup_policy_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/cocoapods_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/cocoapods_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/cocoapods_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/cocoapods_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/component_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/component_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/component_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/component_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/component_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/component_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/component_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/component_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/conan_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/conan_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/conan_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/conan_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/conda_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/conda_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/conda_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/conda_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_create_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_create_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_create_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_create_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_response.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_response.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_response.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_response.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_update_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_update_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/content_selector_api_update_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/content_selector_api_update_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/create_ldap_server_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/create_ldap_server_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/create_ldap_server_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/create_ldap_server_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/crowd_api_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/crowd_api_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/crowd_api_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/crowd_api_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_group_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_group_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_group_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_group_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_storage_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_storage_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_hosted_storage_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_hosted_storage_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/docker_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/docker_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_create_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_create_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_create_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_create_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_model.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_model.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_model.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_update_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_update_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/file_blob_store_api_update_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/file_blob_store_api_update_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/generic_blob_store_api_response.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/generic_blob_store_api_response.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/generic_blob_store_api_response.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/generic_blob_store_api_response.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/git_lfs_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/git_lfs_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/git_lfs_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/git_lfs_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/golang_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/golang_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/golang_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/golang_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/golang_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/golang_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/golang_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/golang_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_create_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_create_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_create_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_create_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_model.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_model.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_model.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_response.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_response.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_response.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_response.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_update_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_update_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_blob_store_api_update_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_blob_store_api_update_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_deploy_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_deploy_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/group_deploy_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/group_deploy_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/helm_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/helm_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/helm_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/helm_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/helm_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/helm_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/helm_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/helm_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/hosted_storage_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/hosted_storage_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/hosted_storage_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/hosted_storage_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_attributes_with_preemptive_auth.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_attributes_with_preemptive_auth.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_attributes_with_preemptive_auth.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_attributes_with_preemptive_auth.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_authentication_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_authentication_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_authentication_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_authentication_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_authentication_attributes_with_preemptive.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_authentication_attributes_with_preemptive.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/http_client_connection_authentication_attributes_with_preemptive.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/http_client_connection_authentication_attributes_with_preemptive.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/iq_connection_verification_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/iq_connection_verification_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/iq_connection_verification_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/iq_connection_verification_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/iq_connection_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/iq_connection_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/iq_connection_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/iq_connection_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_hosted_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_hosted_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_hosted_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_hosted_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_proxy_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_proxy_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_proxy_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/maven_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/maven_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/negative_cache_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/negative_cache_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/negative_cache_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/negative_cache_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_proxy_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_proxy_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_proxy_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/npm_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/npm_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_proxy_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_proxy_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_proxy_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_proxy_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/nuget_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/nuget_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/p2_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/p2_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/p2_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/p2_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_asset_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_asset_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_asset_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_asset_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_component_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_component_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_component_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_component_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_tag_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_tag_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_tag_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_tag_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_task_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_task_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/page_task_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/page_task_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/proxy_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/proxy_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/proxy_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/proxy_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/pypi_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/pypi_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/r_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/r_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/raw_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/raw_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/read_ldap_server_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/read_ldap_server_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/read_ldap_server_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/read_ldap_server_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/read_only_state.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/read_only_state.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/read_only_state.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/read_only_state.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/realm_api_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/realm_api_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/realm_api_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/realm_api_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_connection_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_connection_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_connection_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_connection_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_enable_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_enable_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/replication_enable_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/replication_enable_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/repository_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/repository_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/repository_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/repository_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/result.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/result.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/result.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/result.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/role_xo_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/role_xo_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/role_xo_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/role_xo_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/role_xo_response.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/role_xo_response.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/role_xo_response.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/role_xo_response.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/routing_rule_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/routing_rule_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/routing_rule_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/routing_rule_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/ruby_gems_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/ruby_gems_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_advanced_bucket_connection.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_advanced_bucket_connection.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_advanced_bucket_connection.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_advanced_bucket_connection.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket_configuration.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket_configuration.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket_configuration.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket_configuration.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket_security.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket_security.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_bucket_security.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_bucket_security.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_encryption.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_encryption.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_encryption.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_encryption.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_model.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/s3_blob_store_api_model.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/s3_blob_store_api_model.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/saml_configuration_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/saml_configuration_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/saml_configuration_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/saml_configuration_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/script_result_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/script_result_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/script_result_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/script_result_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/script_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/script_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/script_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/script_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_group_deploy_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_group_deploy_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_group_deploy_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_group_deploy_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_group_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_group_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_group_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_group_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_hosted_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_hosted_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_hosted_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_hosted_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_proxy_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_proxy_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/simple_api_proxy_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/simple_api_proxy_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/stack_trace_element.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/stack_trace_element.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/stack_trace_element.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/storage_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/storage_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/storage_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/storage_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/support_zip_generator_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/support_zip_generator_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/support_zip_generator_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/support_zip_generator_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/support_zip_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/support_zip_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/support_zip_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/support_zip_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/tag_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/tag_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/tag_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/tag_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/task_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/task_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/task_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/task_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/throwable.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/throwable.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/throwable.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/throwable.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/update_ldap_server_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/update_ldap_server_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/update_ldap_server_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/update_ldap_server_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/upload_definition_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/upload_definition_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/upload_definition_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/upload_definition_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/upload_field_definition_xo.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/upload_field_definition_xo.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/upload_field_definition_xo.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/upload_field_definition_xo.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/user_tokens_api_model.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/user_tokens_api_model.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/user_tokens_api_model.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/user_tokens_api_model.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_group_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_group_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_group_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_group_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_hosted_api_repository.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_hosted_api_repository.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_hosted_api_repository.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_hosted_api_repository.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_hosted_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_hosted_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_hosted_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_hosted_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_proxy_repository_api_request.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_proxy_repository_api_request.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_proxy_repository_api_request.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_proxy_repository_api_request.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_signing_repositories_attributes.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_signing_repositories_attributes.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/model/yum_signing_repositories_attributes.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/model/yum_signing_repositories_attributes.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/models/__init__.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/__init__.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replication_connection_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replication_connection_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_enable/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_enable/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_enable/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_enable/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/beta_replicationtarget_repository_repository_name_enable/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_assets_id/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_assets_id/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_azureblobstore_test_connection/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_azureblobstore_test_connection/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_azureblobstore_test_connection/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_azureblobstore_test_connection/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_azure_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_azure_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_file_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_file_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_convert_name_new_name_for_original/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_group_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_group_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name_quota_status/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name_quota_status/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_name_quota_status/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_name_quota_status/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_blobstores_s3_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_blobstores_s3_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_components_id/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_components_id/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email_verify/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email_verify/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_email_verify/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_email_verify/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_format_upload_specs/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_format_upload_specs/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_format_upload_specs/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_format_upload_specs/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_upload_specs/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_upload_specs/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_formats_upload_specs/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_formats_upload_specs/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_disable/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_disable/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_disable/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_disable/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_enable/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_enable/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_enable/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_enable/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_verify_connection/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_verify_connection/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_iq_verify_connection/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_iq_verify_connection/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_bounce/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_bounce/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_bounce/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_bounce/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_lifecycle_phase/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_lifecycle_phase/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_force_release/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_force_release/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_force_release/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_force_release/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_freeze/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_freeze/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_freeze/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_freeze/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_release/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_release/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_read_only_release/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_read_only_release/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_apt_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_bower_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_cocoapods_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conan_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_conda_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_docker_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_gitlfs_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_go_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_helm_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_maven_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_npm_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_nuget_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_p2_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_pypi_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_r_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_raw_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_health_check/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_health_check/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_invalidate_cache/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_repository_name_rebuild_index/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_rubygems_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_group_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_group_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_hosted_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repositories_yum_proxy_repository_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repository_settings/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repository_settings/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_repository_settings/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_repository_settings/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_routing_rules_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_routing_rules_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name_run/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name_run/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_script_name_run/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_script_name_run/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets_download/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets_download/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_search_assets_download/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_search_assets_download/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_anonymous/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_anonymous/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_clear_cache/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_atlassian_crowd_verify_connection/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_content_selectors_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_content_selectors_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_jwt/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_jwt/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_jwt/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_jwt/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_change_order/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_change_order/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_change_order/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_change_order/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ldap_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ldap_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application_privilege_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application_privilege_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_application_privilege_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_application_privilege_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_privilege_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_privilege_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_admin_privilege_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_content_selector_privilege_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_repository_view_privilege_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script_privilege_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script_privilege_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_script_privilege_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_script_privilege_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_privileges_wildcard_privilege_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_active/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_active/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_available/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_available/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_realms_available/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_realms_available/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_roles_id/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_roles_id/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_metadata/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_metadata/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_metadata/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_metadata/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_pem/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_pem/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_saml_pem/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_saml_pem/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore_id/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore_id/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_ssl_truststore_id/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_ssl_truststore_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_sources/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_sources/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_sources/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_sources/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_user_tokens/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_user_tokens/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_change_password/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_change_password/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_change_password/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_change_password/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_security_users_user_id_realm_user_token_reset/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_delete/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_delete/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_delete/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_delete/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_move_destination/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_move_destination/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_staging_move_destination/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_staging_move_destination/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_check/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_check/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_check/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_check/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_writable/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_writable/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_status_writable/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_status_writable/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzip/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzip/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzip/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzip/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzippath/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzippath/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_support_supportzippath/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_support_supportzippath/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_system_license/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_system_license/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_associate_tag_name/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_associate_tag_name/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/delete.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/delete.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/delete.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/delete.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/put.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/put.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tags_name/put.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tags_name/put.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id/get.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id/get.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id/get.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id/get.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_run/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_run/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_run/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_run/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_stop/post.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_stop/post.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/paths/v1_tasks_id_stop/post.pyi` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/paths/v1_tasks_id_stop/post.pyi`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/rest.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/nexus_sdk/schemas.py` & `sonatype_nexus_sdk-0.1.3/nexus_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `sonatype_nexus_sdk-0.1.0/pyproject.toml` & `sonatype_nexus_sdk-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sonatype-nexus-sdk"
-version = "0.1.0"
-description = "Python SDK for Sonatype Nexus Products"
+version = "0.1.3"
+description = "Python SDK for Sonatype Products such as Nexus Repository Manager, Lifecycle and IQ Server "
 authors = ["Justin Bailey <justthered63@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nexus_sdk" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `sonatype_nexus_sdk-0.1.0/PKG-INFO` & `sonatype_nexus_sdk-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,23 @@
-Metadata-Version: 2.1
-Name: sonatype-nexus-sdk
-Version: 0.1.0
-Summary: Python SDK for Sonatype Nexus Products
-License: MIT
-Author: Justin Bailey
-Author-email: justthered63@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
-Requires-Dist: frozendict (>=2.3.8,<3.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: setuptools (>=67.8.0,<68.0.0)
-Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
-Requires-Dist: urllib3 (>=2.0.2,<3.0.0)
-Description-Content-Type: text/markdown
-
 # Sonatype Nexus SDK for Python
 
 ## Requirements
 
 Python `^3.9`
 
 ## Installation & Usage
 
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install sonatype-nexus-sdk
 ```
 
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-
-Then import the package:
-
-```python
-import nexus_sdk
-```
-
-### Setuptools
-
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-
-```sh
-python setup.py install --user
-```
-
-(or `sudo python setup.py install` to install the package for all users)
-
 Then import the package:
 
 ```python
 import nexus_sdk
 ```
 
 ## Getting Started
@@ -89,16 +50,14 @@
         api_instance.delete_asset(id)
     except nexus_sdk.ApiException as e:
         print("Exception when calling AssetsApi->delete_asset: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to _<http://localhost/service/rest>_
-
 | Class                                  | Method                                                                                                                       | HTTP request                                                                | Description                                                                                                   |
 | -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
 | _AssetsApi_                            | [**delete_asset**](docs/apis/tags/AssetsApi.md#delete_asset)                                                                 | **delete** /v1/assets/{id}                                                  | Delete a single asset                                                                                         |
 | _AssetsApi_                            | [**get_asset_by_id**](docs/apis/tags/AssetsApi.md#get_asset_by_id)                                                           | **get** /v1/assets/{id}                                                     | Get a single asset                                                                                            |
 | _AssetsApi_                            | [**get_assets**](docs/apis/tags/AssetsApi.md#get_assets)                                                                     | **get** /v1/assets                                                          | List assets                                                                                                   |
 | _AzureBlobStoreApi_                    | [**verify_connection2**](docs/apis/tags/AzureBlobStoreApi.md#verify_connection2)                                             | **post** /v1/azureblobstore/test-connection                                 | Verify connection using supplied Azure Blob Store settings                                                    |
 | _BlobStoreApi_                         | [**convert_blob_store_to_group**](docs/apis/tags/BlobStoreApi.md#convert_blob_store_to_group)                                | **post** /v1/blobstores/group/convert/{name}/{newNameForOriginal}           | Convert a blob store to a group blob store                                                                    |
@@ -368,196 +327,7 @@
 | _TagsApi_                              | [**get3**](docs/apis/tags/TagsApi.md#get3)                                                                                   | **get** /v1/tags/{name}                                                     | Get a tag                                                                                                     |
 | _TagsApi_                              | [**get_tags**](docs/apis/tags/TagsApi.md#get_tags)                                                                           | **get** /v1/tags                                                            | List tags                                                                                                     |
 | _TagsApi_                              | [**replace**](docs/apis/tags/TagsApi.md#replace)                                                                             | **put** /v1/tags/{name}                                                     | Update a tags attributes                                                                                      |
 | _TasksApi_                             | [**get_task_by_id**](docs/apis/tags/TasksApi.md#get_task_by_id)                                                              | **get** /v1/tasks/{id}                                                      | Get a single task by id                                                                                       |
 | _TasksApi_                             | [**get_tasks**](docs/apis/tags/TasksApi.md#get_tasks)                                                                        | **get** /v1/tasks                                                           | List tasks                                                                                                    |
 | _TasksApi_                             | [**run**](docs/apis/tags/TasksApi.md#run)                                                                                    | **post** /v1/tasks/{id}/run                                                 | Run task                                                                                                      |
 | _TasksApi_                             | [**stop**](docs/apis/tags/TasksApi.md#stop)                                                                                  | **post** /v1/tasks/{id}/stop                                                | Stop task                                                                                                     |
-
-## Documentation For Models
-
-- [AbstractApiRepository](docs/models/AbstractApiRepository.md)
-- [AnonymousAccessSettingsXO](docs/models/AnonymousAccessSettingsXO.md)
-- [ApiCertificate](docs/models/ApiCertificate.md)
-- [ApiCreateUser](docs/models/ApiCreateUser.md)
-- [ApiEmailConfiguration](docs/models/ApiEmailConfiguration.md)
-- [ApiEmailValidation](docs/models/ApiEmailValidation.md)
-- [ApiLicenseDetailsXO](docs/models/ApiLicenseDetailsXO.md)
-- [ApiPrivilege](docs/models/ApiPrivilege.md)
-- [ApiPrivilegeApplicationRequest](docs/models/ApiPrivilegeApplicationRequest.md)
-- [ApiPrivilegeRepositoryAdminRequest](docs/models/ApiPrivilegeRepositoryAdminRequest.md)
-- [ApiPrivilegeRepositoryContentSelectorRequest](docs/models/ApiPrivilegeRepositoryContentSelectorRequest.md)
-- [ApiPrivilegeRepositoryViewRequest](docs/models/ApiPrivilegeRepositoryViewRequest.md)
-- [ApiPrivilegeScriptRequest](docs/models/ApiPrivilegeScriptRequest.md)
-- [ApiPrivilegeWildcardRequest](docs/models/ApiPrivilegeWildcardRequest.md)
-- [ApiUser](docs/models/ApiUser.md)
-- [ApiUserSource](docs/models/ApiUserSource.md)
-- [AptHostedApiRepository](docs/models/AptHostedApiRepository.md)
-- [AptHostedRepositoriesAttributes](docs/models/AptHostedRepositoriesAttributes.md)
-- [AptHostedRepositoryApiRequest](docs/models/AptHostedRepositoryApiRequest.md)
-- [AptProxyApiRepository](docs/models/AptProxyApiRepository.md)
-- [AptProxyRepositoriesAttributes](docs/models/AptProxyRepositoriesAttributes.md)
-- [AptProxyRepositoryApiRequest](docs/models/AptProxyRepositoryApiRequest.md)
-- [AptSigningRepositoriesAttributes](docs/models/AptSigningRepositoriesAttributes.md)
-- [AssetXO](docs/models/AssetXO.md)
-- [AzureBlobStoreApiAuthentication](docs/models/AzureBlobStoreApiAuthentication.md)
-- [AzureBlobStoreApiBucketConfiguration](docs/models/AzureBlobStoreApiBucketConfiguration.md)
-- [AzureBlobStoreApiModel](docs/models/AzureBlobStoreApiModel.md)
-- [AzureConnectionXO](docs/models/AzureConnectionXO.md)
-- [BaseTagXO](docs/models/BaseTagXO.md)
-- [BlobStoreApiSoftQuota](docs/models/BlobStoreApiSoftQuota.md)
-- [BlobStoreQuotaResultXO](docs/models/BlobStoreQuotaResultXO.md)
-- [BowerAttributes](docs/models/BowerAttributes.md)
-- [BowerGroupRepositoryApiRequest](docs/models/BowerGroupRepositoryApiRequest.md)
-- [BowerHostedRepositoryApiRequest](docs/models/BowerHostedRepositoryApiRequest.md)
-- [BowerProxyApiRepository](docs/models/BowerProxyApiRepository.md)
-- [BowerProxyRepositoryApiRequest](docs/models/BowerProxyRepositoryApiRequest.md)
-- [CleanupPolicyAttributes](docs/models/CleanupPolicyAttributes.md)
-- [CocoapodsProxyRepositoryApiRequest](docs/models/CocoapodsProxyRepositoryApiRequest.md)
-- [ComponentAttributes](docs/models/ComponentAttributes.md)
-- [ComponentXO](docs/models/ComponentXO.md)
-- [ConanProxyRepositoryApiRequest](docs/models/ConanProxyRepositoryApiRequest.md)
-- [CondaProxyRepositoryApiRequest](docs/models/CondaProxyRepositoryApiRequest.md)
-- [ContentSelectorApiCreateRequest](docs/models/ContentSelectorApiCreateRequest.md)
-- [ContentSelectorApiResponse](docs/models/ContentSelectorApiResponse.md)
-- [ContentSelectorApiUpdateRequest](docs/models/ContentSelectorApiUpdateRequest.md)
-- [CreateLdapServerXo](docs/models/CreateLdapServerXo.md)
-- [CrowdApiXO](docs/models/CrowdApiXO.md)
-- [DockerAttributes](docs/models/DockerAttributes.md)
-- [DockerGroupApiRepository](docs/models/DockerGroupApiRepository.md)
-- [DockerGroupRepositoryApiRequest](docs/models/DockerGroupRepositoryApiRequest.md)
-- [DockerHostedApiRepository](docs/models/DockerHostedApiRepository.md)
-- [DockerHostedRepositoryApiRequest](docs/models/DockerHostedRepositoryApiRequest.md)
-- [DockerHostedStorageAttributes](docs/models/DockerHostedStorageAttributes.md)
-- [DockerProxyApiRepository](docs/models/DockerProxyApiRepository.md)
-- [DockerProxyAttributes](docs/models/DockerProxyAttributes.md)
-- [DockerProxyRepositoryApiRequest](docs/models/DockerProxyRepositoryApiRequest.md)
-- [FileBlobStoreApiCreateRequest](docs/models/FileBlobStoreApiCreateRequest.md)
-- [FileBlobStoreApiModel](docs/models/FileBlobStoreApiModel.md)
-- [FileBlobStoreApiUpdateRequest](docs/models/FileBlobStoreApiUpdateRequest.md)
-- [GenericBlobStoreApiResponse](docs/models/GenericBlobStoreApiResponse.md)
-- [GitLfsHostedRepositoryApiRequest](docs/models/GitLfsHostedRepositoryApiRequest.md)
-- [GolangGroupRepositoryApiRequest](docs/models/GolangGroupRepositoryApiRequest.md)
-- [GolangProxyRepositoryApiRequest](docs/models/GolangProxyRepositoryApiRequest.md)
-- [GroupAttributes](docs/models/GroupAttributes.md)
-- [GroupBlobStoreApiCreateRequest](docs/models/GroupBlobStoreApiCreateRequest.md)
-- [GroupBlobStoreApiModel](docs/models/GroupBlobStoreApiModel.md)
-- [GroupBlobStoreApiResponse](docs/models/GroupBlobStoreApiResponse.md)
-- [GroupBlobStoreApiUpdateRequest](docs/models/GroupBlobStoreApiUpdateRequest.md)
-- [GroupDeployAttributes](docs/models/GroupDeployAttributes.md)
-- [HelmHostedRepositoryApiRequest](docs/models/HelmHostedRepositoryApiRequest.md)
-- [HelmProxyRepositoryApiRequest](docs/models/HelmProxyRepositoryApiRequest.md)
-- [HostedStorageAttributes](docs/models/HostedStorageAttributes.md)
-- [HttpClientAttributes](docs/models/HttpClientAttributes.md)
-- [HttpClientAttributesWithPreemptiveAuth](docs/models/HttpClientAttributesWithPreemptiveAuth.md)
-- [HttpClientConnectionAttributes](docs/models/HttpClientConnectionAttributes.md)
-- [HttpClientConnectionAuthenticationAttributes](docs/models/HttpClientConnectionAuthenticationAttributes.md)
-- [HttpClientConnectionAuthenticationAttributesWithPreemptive](docs/models/HttpClientConnectionAuthenticationAttributesWithPreemptive.md)
-- [IqConnectionVerificationXo](docs/models/IqConnectionVerificationXo.md)
-- [IqConnectionXo](docs/models/IqConnectionXo.md)
-- [MavenAttributes](docs/models/MavenAttributes.md)
-- [MavenGroupRepositoryApiRequest](docs/models/MavenGroupRepositoryApiRequest.md)
-- [MavenHostedApiRepository](docs/models/MavenHostedApiRepository.md)
-- [MavenHostedRepositoryApiRequest](docs/models/MavenHostedRepositoryApiRequest.md)
-- [MavenProxyApiRepository](docs/models/MavenProxyApiRepository.md)
-- [MavenProxyRepositoryApiRequest](docs/models/MavenProxyRepositoryApiRequest.md)
-- [NegativeCacheAttributes](docs/models/NegativeCacheAttributes.md)
-- [NpmAttributes](docs/models/NpmAttributes.md)
-- [NpmGroupRepositoryApiRequest](docs/models/NpmGroupRepositoryApiRequest.md)
-- [NpmHostedRepositoryApiRequest](docs/models/NpmHostedRepositoryApiRequest.md)
-- [NpmProxyApiRepository](docs/models/NpmProxyApiRepository.md)
-- [NpmProxyRepositoryApiRequest](docs/models/NpmProxyRepositoryApiRequest.md)
-- [NugetAttributes](docs/models/NugetAttributes.md)
-- [NugetGroupRepositoryApiRequest](docs/models/NugetGroupRepositoryApiRequest.md)
-- [NugetHostedRepositoryApiRequest](docs/models/NugetHostedRepositoryApiRequest.md)
-- [NugetProxyApiRepository](docs/models/NugetProxyApiRepository.md)
-- [NugetProxyRepositoryApiRequest](docs/models/NugetProxyRepositoryApiRequest.md)
-- [P2ProxyRepositoryApiRequest](docs/models/P2ProxyRepositoryApiRequest.md)
-- [Page](docs/models/Page.md)
-- [PageAssetXO](docs/models/PageAssetXO.md)
-- [PageComponentXO](docs/models/PageComponentXO.md)
-- [PageTagXO](docs/models/PageTagXO.md)
-- [PageTaskXO](docs/models/PageTaskXO.md)
-- [ProxyAttributes](docs/models/ProxyAttributes.md)
-- [PypiGroupRepositoryApiRequest](docs/models/PypiGroupRepositoryApiRequest.md)
-- [PypiHostedRepositoryApiRequest](docs/models/PypiHostedRepositoryApiRequest.md)
-- [PypiProxyRepositoryApiRequest](docs/models/PypiProxyRepositoryApiRequest.md)
-- [RGroupRepositoryApiRequest](docs/models/RGroupRepositoryApiRequest.md)
-- [RHostedRepositoryApiRequest](docs/models/RHostedRepositoryApiRequest.md)
-- [RProxyRepositoryApiRequest](docs/models/RProxyRepositoryApiRequest.md)
-- [RawAttributes](docs/models/RawAttributes.md)
-- [RawGroupRepositoryApiRequest](docs/models/RawGroupRepositoryApiRequest.md)
-- [RawHostedRepositoryApiRequest](docs/models/RawHostedRepositoryApiRequest.md)
-- [RawProxyRepositoryApiRequest](docs/models/RawProxyRepositoryApiRequest.md)
-- [ReadLdapServerXo](docs/models/ReadLdapServerXo.md)
-- [ReadOnlyState](docs/models/ReadOnlyState.md)
-- [RealmApiXO](docs/models/RealmApiXO.md)
-- [ReplicationAttributes](docs/models/ReplicationAttributes.md)
-- [ReplicationConnectionXO](docs/models/ReplicationConnectionXO.md)
-- [ReplicationEnableXO](docs/models/ReplicationEnableXO.md)
-- [RepositoryXO](docs/models/RepositoryXO.md)
-- [Result](docs/models/Result.md)
-- [RoleXORequest](docs/models/RoleXORequest.md)
-- [RoleXOResponse](docs/models/RoleXOResponse.md)
-- [RoutingRuleXO](docs/models/RoutingRuleXO.md)
-- [RubyGemsGroupRepositoryApiRequest](docs/models/RubyGemsGroupRepositoryApiRequest.md)
-- [RubyGemsHostedRepositoryApiRequest](docs/models/RubyGemsHostedRepositoryApiRequest.md)
-- [RubyGemsProxyRepositoryApiRequest](docs/models/RubyGemsProxyRepositoryApiRequest.md)
-- [S3BlobStoreApiAdvancedBucketConnection](docs/models/S3BlobStoreApiAdvancedBucketConnection.md)
-- [S3BlobStoreApiBucket](docs/models/S3BlobStoreApiBucket.md)
-- [S3BlobStoreApiBucketConfiguration](docs/models/S3BlobStoreApiBucketConfiguration.md)
-- [S3BlobStoreApiBucketSecurity](docs/models/S3BlobStoreApiBucketSecurity.md)
-- [S3BlobStoreApiEncryption](docs/models/S3BlobStoreApiEncryption.md)
-- [S3BlobStoreApiModel](docs/models/S3BlobStoreApiModel.md)
-- [SamlConfigurationXO](docs/models/SamlConfigurationXO.md)
-- [ScriptResultXO](docs/models/ScriptResultXO.md)
-- [ScriptXO](docs/models/ScriptXO.md)
-- [SimpleApiGroupDeployRepository](docs/models/SimpleApiGroupDeployRepository.md)
-- [SimpleApiGroupRepository](docs/models/SimpleApiGroupRepository.md)
-- [SimpleApiHostedRepository](docs/models/SimpleApiHostedRepository.md)
-- [SimpleApiProxyRepository](docs/models/SimpleApiProxyRepository.md)
-- [StackTraceElement](docs/models/StackTraceElement.md)
-- [StorageAttributes](docs/models/StorageAttributes.md)
-- [SupportZipGeneratorRequest](docs/models/SupportZipGeneratorRequest.md)
-- [SupportZipXO](docs/models/SupportZipXO.md)
-- [TagXO](docs/models/TagXO.md)
-- [TaskXO](docs/models/TaskXO.md)
-- [Throwable](docs/models/Throwable.md)
-- [UpdateLdapServerXo](docs/models/UpdateLdapServerXo.md)
-- [UploadDefinitionXO](docs/models/UploadDefinitionXO.md)
-- [UploadFieldDefinitionXO](docs/models/UploadFieldDefinitionXO.md)
-- [UserTokensApiModel](docs/models/UserTokensApiModel.md)
-- [YumAttributes](docs/models/YumAttributes.md)
-- [YumGroupRepositoryApiRequest](docs/models/YumGroupRepositoryApiRequest.md)
-- [YumHostedApiRepository](docs/models/YumHostedApiRepository.md)
-- [YumHostedRepositoryApiRequest](docs/models/YumHostedRepositoryApiRequest.md)
-- [YumProxyRepositoryApiRequest](docs/models/YumProxyRepositoryApiRequest.md)
-- [YumSigningRepositoriesAttributes](docs/models/YumSigningRepositoriesAttributes.md)
-
-## Documentation For Authorization
-
-Endpoints do not require authorization.
-
-## Author
-
-## Notes for Large OpenAPI documents
-
-If the OpenAPI document is large, imports in nexus_sdk.apis and nexus_sdk.models may fail with a
-RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
-
-Solution 1:
-Use specific imports for apis and models like:
-
-- `from nexus_sdk.apis.default_api import DefaultApi`
-- `from nexus_sdk.model.pet import Pet`
-
-Solution 1:
-Before importing the package, adjust the maximum recursion limit as shown below:
-
-```
-import sys
-sys.setrecursionlimit(1500)
-import nexus_sdk
-from nexus_sdk.apis import *
-from nexus_sdk.models import *
-```
-
```


# Comparing `tmp/akerbp.mlops-3.1.2a0.tar.gz` & `tmp/akerbp.mlops-3.1.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-l861yfsg/akerbp.mlops-3.1.2a0.tar", last modified: Mon May 22 17:17:11 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-l9dc4bu3/akerbp.mlops-3.1.2a1.tar", last modified: Fri May 26 08:09:46 2023, max compression
```

## Comparing `akerbp.mlops-3.1.2a0.tar` & `akerbp.mlops-3.1.2a1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.649086 akerbp.mlops-3.1.2a0/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-22 17:17:11.649086 akerbp.mlops-3.1.2a0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35941 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4060 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3739 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/install.sh
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.641086 akerbp.mlops-3.1.2a0/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/model_artifact/dummy.joblib
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.641086 akerbp.mlops-3.1.2a0/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     2850 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-22 17:17:11.649086 akerbp.mlops-3.1.2a0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.637086 akerbp.mlops-3.1.2a0/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.637086 akerbp.mlops-3.1.2a0/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.641086 akerbp.mlops-3.1.2a0/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-22 17:17:11.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.641086 akerbp.mlops-3.1.2a0/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38633 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.645086 akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16951 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.645086 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     6555 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21689 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.645086 akerbp.mlops-3.1.2a0/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22521 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.645086 akerbp.mlops-3.1.2a0/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.641086 akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-22 17:17:11.000000 akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-05-22 17:17:11.000000 akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 17:17:11.000000 akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-22 17:17:11.000000 akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-22 17:17:11.000000 akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-22 17:17:11.000000 akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.645086 akerbp.mlops-3.1.2a0/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 17:17:11.649086 akerbp.mlops-3.1.2a0/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3562 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/test/test_version_increment.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-05-22 17:16:46.000000 akerbp.mlops-3.1.2a0/upload_dummy_artifacts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.302561 akerbp.mlops-3.1.2a1/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-26 08:09:46.302561 akerbp.mlops-3.1.2a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35941 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4060 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3739 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.294561 akerbp.mlops-3.1.2a1/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/model_artifact/mlpet_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.294561 akerbp.mlops-3.1.2a1/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     5236 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-26 08:09:46.302561 akerbp.mlops-3.1.2a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.282560 akerbp.mlops-3.1.2a1/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.282560 akerbp.mlops-3.1.2a1/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.294561 akerbp.mlops-3.1.2a1/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-26 08:09:46.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.298560 akerbp.mlops-3.1.2a1/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38633 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.298560 akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16951 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.298560 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6555 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21689 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.298560 akerbp.mlops-3.1.2a1/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22521 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.302561 akerbp.mlops-3.1.2a1/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.294561 akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-26 08:09:46.000000 akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-26 08:09:46.000000 akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-26 08:09:46.000000 akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-26 08:09:46.000000 akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-26 08:09:46.000000 akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-26 08:09:46.000000 akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.302561 akerbp.mlops-3.1.2a1/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 08:09:46.302561 akerbp.mlops-3.1.2a1/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/test/test_version_increment.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-05-26 08:09:20.000000 akerbp.mlops-3.1.2a1/upload_dummy_artifacts.py
```

### Comparing `akerbp.mlops-3.1.2a0/.flake8` & `akerbp.mlops-3.1.2a1/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/.pre-commit-config.yaml` & `akerbp.mlops-3.1.2a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/LICENSE` & `akerbp.mlops-3.1.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/PKG-INFO` & `akerbp.mlops-3.1.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.1.2a0
+Version: 3.1.2a1
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.1.2a0/README.md` & `akerbp.mlops-3.1.2a1/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/bitbucket-pipelines.yml` & `akerbp.mlops-3.1.2a1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/build.sh` & `akerbp.mlops-3.1.2a1/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/increment_package_version.py` & `akerbp.mlops-3.1.2a1/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/mlops_settings.yaml` & `akerbp.mlops-3.1.2a1/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/pyproject.toml` & `akerbp.mlops-3.1.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/services/prediction.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.1.2a1/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.1.2a0
+Version: 3.1.2a1
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.1.2a0/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.1.2a1/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 mypy.ini
 promote_dummy_artifacts.py
 pyproject.toml
 remove_dummy_artifacts.py
 setup.py
 upload_dummy_artifacts.py
 model_artifact/README.md
-model_artifact/dummy.joblib
+model_artifact/mlpet_settings.yaml
 model_code/model.py
 model_code/requirements.model
 model_code/test_model.py
 src/akerbp.mlops.egg-info/PKG-INFO
 src/akerbp.mlops.egg-info/SOURCES.txt
 src/akerbp.mlops.egg-info/dependency_links.txt
 src/akerbp.mlops.egg-info/entry_points.txt
```

### Comparing `akerbp.mlops-3.1.2a0/test/test_data_validation.py` & `akerbp.mlops-3.1.2a1/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_install_requirements.py` & `akerbp.mlops-3.1.2a1/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_metadata_validation.py` & `akerbp.mlops-3.1.2a1/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.1.2a1/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.1.2a1/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.1.2a1/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.1.2a1/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.1.2a1/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.1.2a1/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.1.2a1/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.1.2a1/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a0/test/test_version_increment.py` & `akerbp.mlops-3.1.2a1/test/test_version_increment.py`

 * *Files identical despite different names*


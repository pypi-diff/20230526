# Comparing `tmp/trojai-sdk-0.2.3.4.tar.gz` & `tmp/trojai-sdk-0.2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Barrie Tomilson\Documents\github (2)\sdk\troj-sdk\dist\.tmp-kv1vjbs5\trojai-sdk-0.2.3.4.tar", last modified: Thu Apr  6 13:53:04 2023, max compression
+gzip compressed data, was "C:\Users\Barrie Tomilson\Documents\github (2)\sdk\troj-sdk\dist\.tmp-qr2i5l5e\trojai-sdk-0.2.3.6.tar", last modified: Fri May 26 13:23:10 2023, max compression
```

## Comparing `trojai-sdk-0.2.3.4.tar` & `trojai-sdk-0.2.3.6.tar`

### file list

```diff
@@ -1,92 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.709624 trojai-sdk-0.2.3.4/
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.480621 trojai-sdk-0.2.3.4/.github/
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.519622 trojai-sdk-0.2.3.4/.github/workflows/
--rw-rw-rw-   0        0        0     1213 2023-03-28 21:13:31.000000 trojai-sdk-0.2.3.4/.github/workflows/python-app.yml
--rw-rw-rw-   0        0        0      104 2023-04-05 17:10:54.000000 trojai-sdk-0.2.3.4/.gitignore
--rw-rw-rw-   0        0        0     1525 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/.gitlab-ci.yml
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.521620 trojai-sdk-0.2.3.4/.vscode/
--rw-rw-rw-   0        0        0      510 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/.vscode/launch.json
--rw-rw-rw-   0        0        0      167 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3104 2023-04-06 13:53:04.708621 trojai-sdk-0.2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2505 2023-04-05 17:10:54.000000 trojai-sdk-0.2.3.4/README.md
--rw-rw-rw-   0        0        0      372 2023-04-05 17:10:54.000000 trojai-sdk-0.2.3.4/auth_config_dev.json
--rw-rw-rw-   0        0        0      102 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 13:53:04.710620 trojai-sdk-0.2.3.4/setup.cfg
--rw-rw-rw-   0        0        0      995 2023-04-06 13:51:19.000000 trojai-sdk-0.2.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.484621 trojai-sdk-0.2.3.4/test_proj/
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.485622 trojai-sdk-0.2.3.4/test_proj/credit_dataset/
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.555620 trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/
--rw-rw-rw-   0        0        0     1296 2023-04-06 13:17:36.000000 trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/attacks.json
--rw-rw-rw-   0        0        0      154 2023-04-06 13:17:36.000000 trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/auth.json
--rw-rw-rw-   0        0        0      808 2023-04-06 13:17:36.000000 trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/base.json
--rw-rw-rw-   0        0        0      169 2023-04-06 13:17:36.000000 trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/docker_config.json
--rw-rw-rw-   0        0        0      266 2023-04-06 13:17:36.000000 trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/k8s_config.json
--rw-rw-rw-   0        0        0      257 2023-04-06 13:17:36.000000 trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/model_config.json
--rw-rw-rw-   0        0        0      356 2023-04-06 13:17:35.000000 trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/test_config.json
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.586618 trojai-sdk-0.2.3.4/trojai_sdk.egg-info/
--rw-rw-rw-   0        0        0     3104 2023-04-06 13:53:04.000000 trojai-sdk-0.2.3.4/trojai_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2623 2023-04-06 13:53:04.000000 trojai-sdk-0.2.3.4/trojai_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 13:53:04.000000 trojai-sdk-0.2.3.4/trojai_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 13:53:04.000000 trojai-sdk-0.2.3.4/trojai_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2023-04-06 13:53:04.000000 trojai-sdk-0.2.3.4/trojai_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 13:53:04.000000 trojai-sdk-0.2.3.4/trojai_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.599619 trojai-sdk-0.2.3.4/trojsdk/
--rw-rw-rw-   0        0        0        0 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/__init__.py
--rw-rw-rw-   0        0        0     7328 2023-03-30 14:02:46.000000 trojai-sdk-0.2.3.4/trojsdk/client.py
--rw-rw-rw-   0        0        0     2937 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.612619 trojai-sdk-0.2.3.4/trojsdk/config/
--rw-rw-rw-   0        0        0        0 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/config/__init__.py
--rw-rw-rw-   0        0        0     4640 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/config/auth.py
--rw-rw-rw-   0        0        0     4558 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/config/base.py
--rw-rw-rw-   0        0        0     2064 2023-03-30 14:02:52.000000 trojai-sdk-0.2.3.4/trojsdk/config/nlp.py
--rw-rw-rw-   0        0        0     2067 2023-01-27 14:50:38.000000 trojai-sdk-0.2.3.4/trojsdk/config/tabular.py
--rw-rw-rw-   0        0        0     2818 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/config/vision.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.618622 trojai-sdk-0.2.3.4/trojsdk/configs/
--rw-rw-rw-   0        0        0     3239 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/configs/auth_config.json
--rw-rw-rw-   0        0        0     2397 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/configs/auth_config_dev.json
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.631622 trojai-sdk-0.2.3.4/trojsdk/configs/s3_test/
--rw-rw-rw-   0        0        0     1080 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/configs/s3_test/all_pipe_transform_config.json
--rw-rw-rw-   0        0        0      414 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/configs/s3_test/s3_classification_config.json
--rw-rw-rw-   0        0        0      198 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/configs/s3_test/s3_starKNN_config.json
--rw-rw-rw-   0        0        0      383 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/configs/s3_test/s3_stars_validation_config.json
--rw-rw-rw-   0        0        0     3238 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/configs/s3_test/troj_dev_auth.json
--rw-rw-rw-   0        0        0     1173 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/configs/testing_config.json
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.645621 trojai-sdk-0.2.3.4/trojsdk/core/
--rw-rw-rw-   0        0        0        0 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.647621 trojai-sdk-0.2.3.4/trojsdk/core/__pycache__/
--rw-rw-rw-   0        0        0     3398 2023-04-06 13:15:21.000000 trojai-sdk-0.2.3.4/trojsdk/core/__pycache__/data_utils.cpython-38.pyc
--rw-rw-rw-   0        0        0     7244 2023-03-30 14:02:46.000000 trojai-sdk-0.2.3.4/trojsdk/core/client_utils.py
--rw-rw-rw-   0        0        0     5401 2023-04-06 13:14:32.000000 trojai-sdk-0.2.3.4/trojsdk/core/data_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.649618 trojai-sdk-0.2.3.4/trojsdk/core/experiment_tools/
--rw-rw-rw-   0        0        0    14187 2023-04-06 13:17:07.000000 trojai-sdk-0.2.3.4/trojsdk/core/experiment_tools/__init__.py
--rw-rw-rw-   0        0        0     3670 2023-04-06 13:12:22.000000 trojai-sdk-0.2.3.4/trojsdk/core/test_experiment_gen.py
--rw-rw-rw-   0        0        0     1431 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/core/troj_error.py
--rw-rw-rw-   0        0        0      330 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/core/troj_logging.py
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.675619 trojai-sdk-0.2.3.4/trojsdk/examples/
--rw-rw-rw-   0        0        0     3239 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/auth_config.json
--rw-rw-rw-   0        0        0      469 2023-04-05 17:56:30.000000 trojai-sdk-0.2.3.4/trojsdk/examples/auth_config_dev.json
--rw-rw-rw-   0        0        0      216 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/examples/docker_meta.json
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.677619 trojai-sdk-0.2.3.4/trojsdk/examples/gcloud_tests/
--rw-rw-rw-   0        0        0      640 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/gcloud_tests/gcloud_auth.json
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.689622 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/
--rw-rw-rw-   0        0        0      280 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/attacks.json
--rw-rw-rw-   0        0        0     2337 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/label_map_num.json
--rw-rw-rw-   0        0        0      116 2023-04-05 17:10:54.000000 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/model_config.json
--rw-rw-rw-   0        0        0      276 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/test_config.json
--rw-rw-rw-   0        0        0      281 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/train_config.json
--rw-rw-rw-   0        0        0      572 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/troj_config.json
--rw-rw-rw-   0        0        0     4594 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil_test.json
--rw-rw-rw-   0        0        0     1216 2023-04-05 17:10:54.000000 trojai-sdk-0.2.3.4/trojsdk/examples/nlp_test_main.json
--rw-rw-rw-   0        0        0    24617 2023-03-28 21:13:25.000000 trojai-sdk-0.2.3.4/trojsdk/examples/s3_small_classification_pt_config.json
--rw-rw-rw-   0        0        0     1524 2023-04-05 17:10:54.000000 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_SMOTETomek_logistic_base.json
--rw-rw-rw-   0        0        0     3071 2023-04-05 17:10:54.000000 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_medical_insurance_config.json
-drwxrwxrwx   0        0        0        0 2023-04-06 13:53:04.705623 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/
--rw-rw-rw-   0        0        0     1080 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/all_pipe_transform_config.json
--rw-rw-rw-   0        0        0      435 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/s3_classification_config.json
--rw-rw-rw-   0        0        0      212 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/s3_starKNN_config.json
--rw-rw-rw-   0        0        0      381 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/s3_stars_validation_config.json
--rw-rw-rw-   0        0        0     2006 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/tabular_test_main.json
--rw-rw-rw-   0        0        0     2406 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/troj_dev_auth.json
--rw-rw-rw-   0        0        0     1183 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/examples/testing_config.json
--rw-rw-rw-   0        0        0      989 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.4/trojsdk/setup.py
--rw-rw-rw-   0        0        0      745 2023-04-05 17:10:54.000000 trojai-sdk-0.2.3.4/trojsdk/test_sdk.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.485613 trojai-sdk-0.2.3.6/
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.015618 trojai-sdk-0.2.3.6/.github/
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.070649 trojai-sdk-0.2.3.6/.github/workflows/
+-rw-rw-rw-   0        0        0     1487 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/.github/workflows/pytest.yml
+-rw-rw-rw-   0        0        0     1550 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/.github/workflows/python-app.yml
+-rw-rw-rw-   0        0        0      113 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/.gitignore
+-rw-rw-rw-   0        0        0     1525 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/.gitlab-ci.yml
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.079617 trojai-sdk-0.2.3.6/.vscode/
+-rw-rw-rw-   0        0        0      510 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/.vscode/launch.json
+-rw-rw-rw-   0        0        0      205 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4488 2023-05-26 13:23:10.485613 trojai-sdk-0.2.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3891 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/README.md
+-rw-rw-rw-   0        0        0      372 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/auth_config_dev.json
+-rw-rw-rw-   0        0        0      117 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 13:23:10.486613 trojai-sdk-0.2.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1068 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.099651 trojai-sdk-0.2.3.6/trojai_sdk.egg-info/
+-rw-rw-rw-   0        0        0     4488 2023-05-26 13:23:09.000000 trojai-sdk-0.2.3.6/trojai_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2531 2023-05-26 13:23:10.000000 trojai-sdk-0.2.3.6/trojai_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 13:23:09.000000 trojai-sdk-0.2.3.6/trojai_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 13:23:09.000000 trojai-sdk-0.2.3.6/trojai_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      108 2023-05-26 13:23:09.000000 trojai-sdk-0.2.3.6/trojai_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 13:23:09.000000 trojai-sdk-0.2.3.6/trojai_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.134617 trojai-sdk-0.2.3.6/trojsdk/
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/__init__.py
+-rw-rw-rw-   0        0        0     8893 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/client.py
+-rw-rw-rw-   0        0        0     5348 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.176617 trojai-sdk-0.2.3.6/trojsdk/config/
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/config/__init__.py
+-rw-rw-rw-   0        0        0     4658 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/config/auth.py
+-rw-rw-rw-   0        0        0     4584 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/config/base.py
+-rw-rw-rw-   0        0        0     2066 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/config/nlp.py
+-rw-rw-rw-   0        0        0     2063 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/config/tabular.py
+-rw-rw-rw-   0        0        0     2815 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/config/vision.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.197617 trojai-sdk-0.2.3.6/trojsdk/configs/
+-rw-rw-rw-   0        0        0     3239 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/configs/auth_config.json
+-rw-rw-rw-   0        0        0     2397 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/configs/auth_config_dev.json
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.234650 trojai-sdk-0.2.3.6/trojsdk/configs/s3_test/
+-rw-rw-rw-   0        0        0     1080 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/configs/s3_test/all_pipe_transform_config.json
+-rw-rw-rw-   0        0        0      414 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/configs/s3_test/s3_classification_config.json
+-rw-rw-rw-   0        0        0      198 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/configs/s3_test/s3_starKNN_config.json
+-rw-rw-rw-   0        0        0      383 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/configs/s3_test/s3_stars_validation_config.json
+-rw-rw-rw-   0        0        0     3238 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/configs/s3_test/troj_dev_auth.json
+-rw-rw-rw-   0        0        0     1173 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/configs/testing_config.json
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.278650 trojai-sdk-0.2.3.6/trojsdk/core/
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.281616 trojai-sdk-0.2.3.6/trojsdk/core/__pycache__/
+-rw-rw-rw-   0        0        0     3477 2023-05-25 17:00:34.000000 trojai-sdk-0.2.3.6/trojsdk/core/__pycache__/data_utils.cpython-38.pyc
+-rw-rw-rw-   0        0        0    12587 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/core/client_utils.py
+-rw-rw-rw-   0        0        0     5633 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/core/data_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.291618 trojai-sdk-0.2.3.6/trojsdk/core/experiment_tools/
+-rw-rw-rw-   0        0        0    16211 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/core/experiment_tools/__init__.py
+-rw-rw-rw-   0        0        0     4559 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/core/test_experiment_gen.py
+-rw-rw-rw-   0        0        0     1431 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/core/troj_error.py
+-rw-rw-rw-   0        0        0      330 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/core/troj_logging.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.368652 trojai-sdk-0.2.3.6/trojsdk/examples/
+-rw-rw-rw-   0        0        0     3239 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/auth_config.json
+-rw-rw-rw-   0        0        0      461 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/auth_config_dev.json
+-rw-rw-rw-   0        0        0      216 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/docker_meta.json
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.376651 trojai-sdk-0.2.3.6/trojsdk/examples/gcloud_tests/
+-rw-rw-rw-   0        0        0      640 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/gcloud_tests/gcloud_auth.json
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.406616 trojai-sdk-0.2.3.6/trojsdk/examples/local_files/
+-rw-rw-rw-   0        0        0    14096 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/local_files/StarKNNPipe.pkl
+-rw-rw-rw-   0        0        0     2445 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/local_files/StarKNNWrapper.py
+-rw-rw-rw-   0        0        0    14201 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/local_files/stars_train.csv
+-rw-rw-rw-   0        0        0     3610 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/local_files/stars_validation.csv
+-rw-rw-rw-   0        0        0   314247 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/new_sdk_features.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.447614 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/
+-rw-rw-rw-   0        0        0      280 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/attacks.json
+-rw-rw-rw-   0        0        0     2337 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/label_map_num.json
+-rw-rw-rw-   0        0        0      116 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/model_config.json
+-rw-rw-rw-   0        0        0      276 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/test_config.json
+-rw-rw-rw-   0        0        0      281 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/train_config.json
+-rw-rw-rw-   0        0        0      572 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/troj_config.json
+-rw-rw-rw-   0        0        0     4594 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil_test.json
+-rw-rw-rw-   0        0        0     1216 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/nlp_test_main.json
+-rw-rw-rw-   0        0        0    24617 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/s3_small_classification_pt_config.json
+-rw-rw-rw-   0        0        0     1296 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/star_attacks.json
+-rw-rw-rw-   0        0        0     1524 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_SMOTETomek_logistic_base.json
+-rw-rw-rw-   0        0        0     3071 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_medical_insurance_config.json
+drwxrwxrwx   0        0        0        0 2023-05-26 13:23:10.483617 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/
+-rw-rw-rw-   0        0        0     1080 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/all_pipe_transform_config.json
+-rw-rw-rw-   0        0        0      435 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/s3_classification_config.json
+-rw-rw-rw-   0        0        0      212 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/s3_starKNN_config.json
+-rw-rw-rw-   0        0        0      381 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/s3_stars_validation_config.json
+-rw-rw-rw-   0        0        0     2006 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/tabular_test_main.json
+-rw-rw-rw-   0        0        0     2406 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/troj_dev_auth.json
+-rw-rw-rw-   0        0        0     1183 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/examples/testing_config.json
+-rw-rw-rw-   0        0        0      989 2023-01-18 17:57:56.000000 trojai-sdk-0.2.3.6/trojsdk/setup.py
+-rw-rw-rw-   0        0        0      744 2023-05-26 13:22:01.000000 trojai-sdk-0.2.3.6/trojsdk/test_sdk.py
```

### Comparing `trojai-sdk-0.2.3.4/.gitlab-ci.yml` & `trojai-sdk-0.2.3.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/setup.py` & `trojai-sdk-0.2.3.6/trojsdk/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-
 setup(
-    name="trojai-sdk",
-    version="0.2.3.4",
+    name="trojsdk",
+    version="0.1",
     packages=find_packages(),
     author="TrojAI",
     author_email="stan.petley@troj.ai",
     description="TrojAI provides the troj Python convenience package to allow users to integrate TrojAI adversarial protections and robustness metrics seamlessly into their AI development pipelines.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://troj.ai",
@@ -18,9 +17,9 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=open("requirements.txt").readlines(),
     python_requires=">=3.6",
-    entry_points={"console_scripts": ["tsdk = trojsdk.cmd:main"]},
+    entry_points={"console_scripts": ["trojsdk = trojsdk.cmd:main"]},
 )
```

### Comparing `trojai-sdk-0.2.3.4/test_proj/credit_dataset/logistic_model/attacks.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/star_attacks.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojai_sdk.egg-info/SOURCES.txt` & `trojai-sdk-0.2.3.6/trojai_sdk.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 .gitignore
 .gitlab-ci.yml
 MANIFEST.in
 README.md
 auth_config_dev.json
 requirements.txt
 setup.py
+.github/workflows/pytest.yml
 .github/workflows/python-app.yml
 .vscode/launch.json
-test_proj/credit_dataset/logistic_model/attacks.json
-test_proj/credit_dataset/logistic_model/auth.json
-test_proj/credit_dataset/logistic_model/base.json
-test_proj/credit_dataset/logistic_model/docker_config.json
-test_proj/credit_dataset/logistic_model/k8s_config.json
-test_proj/credit_dataset/logistic_model/model_config.json
-test_proj/credit_dataset/logistic_model/test_config.json
 trojai_sdk.egg-info/PKG-INFO
 trojai_sdk.egg-info/SOURCES.txt
 trojai_sdk.egg-info/dependency_links.txt
 trojai_sdk.egg-info/entry_points.txt
 trojai_sdk.egg-info/requires.txt
 trojai_sdk.egg-info/top_level.txt
 trojsdk/__init__.py
@@ -46,21 +40,27 @@
 trojsdk/core/troj_error.py
 trojsdk/core/troj_logging.py
 trojsdk/core/__pycache__/data_utils.cpython-38.pyc
 trojsdk/core/experiment_tools/__init__.py
 trojsdk/examples/auth_config.json
 trojsdk/examples/auth_config_dev.json
 trojsdk/examples/docker_meta.json
+trojsdk/examples/new_sdk_features.ipynb
 trojsdk/examples/nlp_phil_test.json
 trojsdk/examples/nlp_test_main.json
 trojsdk/examples/s3_small_classification_pt_config.json
+trojsdk/examples/star_attacks.json
 trojsdk/examples/tabular_SMOTETomek_logistic_base.json
 trojsdk/examples/tabular_medical_insurance_config.json
 trojsdk/examples/testing_config.json
 trojsdk/examples/gcloud_tests/gcloud_auth.json
+trojsdk/examples/local_files/StarKNNPipe.pkl
+trojsdk/examples/local_files/StarKNNWrapper.py
+trojsdk/examples/local_files/stars_train.csv
+trojsdk/examples/local_files/stars_validation.csv
 trojsdk/examples/nlp_phil/attacks.json
 trojsdk/examples/nlp_phil/label_map_num.json
 trojsdk/examples/nlp_phil/model_config.json
 trojsdk/examples/nlp_phil/test_config.json
 trojsdk/examples/nlp_phil/train_config.json
 trojsdk/examples/nlp_phil/troj_config.json
 trojsdk/examples/tabular_test/all_pipe_transform_config.json
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/client.py` & `trojai-sdk-0.2.3.6/trojsdk/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 """
 Troj Client class handls all requests made to a passed endpoint
 """
 
 
 class TrojClient:
-
     api_endpoint: str = None
     refresh_url: str = None
     nossl: bool = False
 
     _auth_config: TrojAuthConfig = None
 
     _creds_api_key: str = None
@@ -152,35 +151,14 @@
             # verify=not self.nossl,
         )
 
         self.raise_resp_exception_error(r)
 
         return {"status_code": r.status_code, "data": r.json()}
 
-    def get_job_status(self, job_id: str) -> dict:
-        """
-        The job_id can be retrieved from the return value of client.post_job(), or from client.get_jobs().
-        Set the client's auth with client.set_credentials() to provide context.
-
-        :param job_id: The id of the desired job.
-        :type job_id: str
-        :return: The status of the job within a requests.Response's JSON data.
-        :rtype: dict
-        """
-        r = requests_retry.get(
-            f"{self.api_endpoint}/sdk/job/{job_id}",
-            headers=self._get_creds_headers(),
-            verify=not self.nossl,
-        )
-
-        print("GET /job/job_id response:", r.json())
-        self.raise_resp_exception_error(r)
-
-        return {"status_code": r.status_code, "data": r.json()}
-
     def raise_resp_exception_error(self, resp):
         if not resp.ok:
             message = None
             try:
                 r_body = resp.json()
                 message = r_body.get("message") or r_body.get("msg")
             except:
@@ -201,7 +179,64 @@
                     raise Exception(
                         f"HTTP Error received: {resp.reason}: {str(resp.status_code)}"
                     )
                 else:
                     raise Exception(
                         f"HTTP Error received: {resp.reason}: {str(resp.status_code)} | {resp.json()['detail']}"
                     )
+
+    def list_stress_test_jobs(
+        self, project_name=None, dataset_name=None, test_run_name=None, status="ALL"
+    ):
+        """
+        Takes in optional proj/dataset/test run, pings backend job table for results of jobs that fit the criteria. Specific statuses can be sent also
+        """
+        r = requests_retry.get(
+            f"{self.api_endpoint}/sdk/jobs/",
+            headers=self._get_creds_headers(),
+            verify=not self.nossl,
+        )
+        decoded_response = json.loads(r.content)
+        if status != "ALL":
+            decoded_response = self.filter_jobs("state", status, decoded_response)
+        if project_name != None:
+            decoded_response = self.filter_jobs(
+                "project_name", project_name, decoded_response
+            )
+        if test_run_name != None:
+            decoded_response = self.filter_jobs(
+                "test_run_name", test_run_name, decoded_response
+            )
+        return decoded_response
+
+    def filter_jobs(self, field, value, decoded_response):
+        built_response = []
+        for pod in decoded_response:
+            if value in pod.get(field):
+                built_response.append(pod)
+        decoded_response = built_response
+        return decoded_response
+
+    def download_test_run(self, job_name):
+        """
+        First gets all the uuids of a given test run name, then uses those to pull the run output back to the sdk
+        """
+        r = requests_retry.get(
+            f"{self.api_endpoint}/sdk/job/{job_name}",
+            headers=self._get_creds_headers(),
+            verify=not self.nossl,
+        )
+        decoded_response = json.loads(r.content)
+        proj = decoded_response.get("project_uuid")
+        dset = decoded_response.get("TestRun").get("dataset_uuid")
+        test = decoded_response.get("TestRun").get("test_run_uuid")
+        if proj is None or dset is None or test is None:
+            raise (
+                Exception("Kubernetes pod errored! Check the logs for the errored pod.")
+            )
+        r2 = requests_retry.get(
+            f"{self.api_endpoint}/sdk/projects/{proj}/datasets/{dset}/test-runs/{test}/download-output",
+            headers=self._get_creds_headers(),
+            verify=not self.nossl,
+        )
+
+        return json.loads(r2.content)
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/config/auth.py` & `trojai-sdk-0.2.3.6/trojsdk/config/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,14 @@
             pass
         return config
 
     @classmethod
     def config_from_json(
         cls, json_path: Union[str, Path], sub_jsons: bool = True
     ) -> "TrojAuthConfig":
-
         """
         This method is needed to read a config dictionary from a JSON file on disk
         and assign the values from the JSON to the fields of the class by corresponding
         keys. Note that the keys in the JSON file must be exactly the same as the names
         of the class fields.
 
         This method through inheritance will be used to construct task-specific configs
@@ -89,20 +88,21 @@
                 + "The following files are in the working directory:"
                 + "\n"
                 + str(os.listdir())
             )
             raise err
 
         try:
-
             config = cls.from_dict(config_dict)
             config = cls._checkGAC(config)
 
-            config.api_endpoint = re.sub(r"/+$", r"", config.api_endpoint) #Remove any "/" characters at the end
-            
+            config.api_endpoint = re.sub(
+                r"/+$", r"", config.api_endpoint
+            )  # Remove any "/" characters at the end
+
             return config
 
         except KeyError as err:
             raise TrojConfigError(
                 f'\n\nKey "{err.args[0]}" missing from json.'
                 "Make sure all required key-value pairs are "
                 "present in the json"
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/config/base.py` & `trojai-sdk-0.2.3.6/trojsdk/config/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 
     test_run_name: str
     task_type: str
     attacks: Any
     dataset: Any
     model: Any
     auth_config: TrojAuthConfig
+    docker_metadata: Optional[Dict] = None
 
     @classmethod
     def config_from_json(
         cls,
         json_path: Union[str, Path],
         sub_jsons: bool = True,
         auth_config: TrojAuthConfig = None,
     ) -> "BaseTrojConfig":
-
         """
         This method is needed to read a config dictionary from a JSON file on disk
         and assign the values from the JSON to the fields of the class by corresponding
         keys. Note that the keys in the JSON file must be exactly the same as the names
         of the class fields.
 
         This method through inheritance will be used to construct task-specific configs
@@ -58,19 +58,18 @@
         return cls.config_from_dict(config_dict, sub_jsons, auth_config)
 
     @classmethod
     def config_from_dict(
         cls, config_dict: dict, auth_config: TrojAuthConfig = None
     ) -> "BaseTrojConfig":
         """Given a dictionary, initializes fields with values from corresponding keys"""
-        
+
         invalid_paths = data_utils.test_paths(config_dict)
 
         if len(invalid_paths) > 0:
-
             err = TrojConfigError(
                 "\n\nSome paths provided were invalid!"
                 + "\n"
                 + "Please ensure the following paths are correct:"
                 + "\n"
                 + str(invalid_paths)
                 + "\n\n"
@@ -114,17 +113,14 @@
             )
             unknown_dict = ast.literal_eval(dict_substring)
             raise TrojConfigError(
                 f'\n\nGot unexpected key(s) in json: "{list(unknown_dict)}"\n'
             )
 
 
-
-
-
 @dataclass_json(undefined=Undefined.RAISE)
 @dataclass
 class BaseTrojDataset(DataClassJsonMixin, JsonSchemaMixin):
 
     """Base dataset class to be extended by dataset classes in the task-specific submodules."""
 
     name: str
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/config/nlp.py` & `trojai-sdk-0.2.3.6/trojsdk/config/nlp.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from dataclasses import dataclass
 from trojsdk.config.base import BaseTrojConfig
 from trojsdk.config.auth import TrojAuthConfig
 from dataclasses_json import dataclass_json, DataClassJsonMixin, Undefined
 from dataclasses_jsonschema import JsonSchemaMixin
 
 
-
 """
 #TODO make support checks. Attacks and dataset should not be enforced, and an extra attribute should be added
 which is an (optional) instance of a checks config (instantiated from some collection of checks Jsons).
 If attacks is None, just the checks are ran. If the check config is None, the attacks must not be None and then
 just the attacks are ran. If both are not None, the checks and the attacks are ran, with a special option of
 adversarial checks which are special in that they take in the results of the attacks and return checks results.
 """
 
 ALLOWED_SUBTASKS = tuple(["classification"])
 
+
 @dataclass_json(undefined=Undefined.RAISE)
 @dataclass
 class NLPTrojConfig(BaseTrojConfig, DataClassJsonMixin, JsonSchemaMixin):
 
     """
     NLP-specific config class to hold info about the users run (including dataset and model).
     Inherits from base class and JSON dataclass.
@@ -47,8 +47,8 @@
     custom_check: t.Optional[str] = None
     custom_evaluator_function: t.Optional[str] = None
     custom_evaluator_args: t.Optional[dict] = None
     custom_attacks: t.Optional[t.Any] = None
 
     save_path: t.Union[str, None] = None
 
-    auth_config: TrojAuthConfig = None
+    auth_config: TrojAuthConfig = None
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/config/tabular.py` & `trojai-sdk-0.2.3.6/trojsdk/config/tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,25 +41,23 @@
     custom_evaluator_function: Optional[str] = None
     custom_evaluator_args: Optional[str] = None
 
     save_path: Union[str, None] = None
     auth_config: Union[TrojAuthConfig, None] = None
 
     def __post_init__(self):
-
         self.task_type = "tabular"
 
         if self.subtask not in ALLOWED_SUBTASKS:
             raise TrojConfigError(
                 f"Subtask {self.subtask} is not supported yet. "
                 f"Currently supported subtasks are: {ALLOWED_SUBTASKS}"
             )
 
     def get_schema(self):
-
         """
         Functionality from JsonSchemaMixin.
         Dump attributes of self as a json schema
 
         :return:
         """
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/config/vision.py` & `trojai-sdk-0.2.3.6/trojsdk/config/vision.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 VISION_ATT_DICT = [
     "corruptions",
     "fgsm",
     "pgd",
     "adaptive_pgd",
     "regularized_pgd",
     "adaptive_regularized_pgd",
-    "min_corruption_search"
+    "min_corruption_search",
 ]
 
 VISION_ATTACK_KEYS = tuple(VISION_ATT_DICT)
 
+
 @dataclass_json(undefined=Undefined.RAISE)
 @dataclass
 class VisionTrojConfig(BaseTrojConfig, DataClassJsonMixin, JsonSchemaMixin):
 
     """Vision config class. Stores all relevant info about the user's run. Inherit from base and JSON dataclass"""
 
     test_run_name: str
@@ -43,31 +44,27 @@
     custom_evaluator_args: Optional[dict] = None
     custom_attacks: Optional[Any] = None
 
     auth_config: TrojAuthConfig = None
     save_path: Optional[str] = None
 
     def __post_init__(self):
-
         """Let the dataset know what the framework is going to be, and create data loader with that info"""
 
         self.task_type = "vision"
 
         if self.subtask is not None:
             self.subtask = self.subtask.casefold()
             if self.subtask not in ALLOWED_SUBTASKS:
                 raise TrojConfigError(
                     f'Provided subtask "{self.subtask}" not supported. '
                     f"Currently supported subtasks are: {ALLOWED_SUBTASKS}"
                 )
 
 
-
-
-
 @dataclass_json(undefined=Undefined.RAISE)
 @dataclass
 class VisionTrojDataset(BaseTrojDataset, DataClassJsonMixin, JsonSchemaMixin):
     """Dataset class to wrap around the user's data stored on disk. Constructed from the user's config file"""
 
     """
     This class is a high-level wrapper for the user's dataset.
@@ -78,8 +75,8 @@
     name: str
     path_to_data: str
     path_to_annotations: str
     data_loader_config: dict
     data_loader: Optional[Any] = None
     metadata: Optional[Any] = None
     classes_dictionary: Optional[Union[Dict[str, int], str]] = None
-    column_defs: Optional[list] = None
+    column_defs: Optional[list] = None
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/configs/auth_config.json` & `trojai-sdk-0.2.3.6/trojsdk/configs/auth_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/configs/auth_config_dev.json` & `trojai-sdk-0.2.3.6/trojsdk/configs/auth_config_dev.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/configs/s3_test/all_pipe_transform_config.json` & `trojai-sdk-0.2.3.6/trojsdk/configs/s3_test/all_pipe_transform_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/configs/s3_test/troj_dev_auth.json` & `trojai-sdk-0.2.3.6/trojsdk/configs/s3_test/troj_dev_auth.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/configs/testing_config.json` & `trojai-sdk-0.2.3.6/trojsdk/configs/testing_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/core/__pycache__/data_utils.cpython-38.pyc` & `trojai-sdk-0.2.3.6/trojsdk/core/__pycache__/data_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr  6 13:14:32 2023 UTC, .py size: 5401 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 b8c5 2e64 1915 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 b962 6e64 0116 0000  U........bnd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6404  ..d.d.l.m.Z...d.
 00000060: 6405 6702 5a07 6406 6407 8400 5a08 6414  d.g.Z.d.d...Z.d.
 00000070: 6504 6509 650a 6409 9c03 640a 640b 8405  e.e.e.d...d.d...
@@ -152,62 +152,67 @@
 00000970: 7272 2000 0000 da04 7265 7072 7203 0000  rr .....reprr...
 00000980: 00da 0877 6172 6e69 6e67 73da 0477 6172  ...warnings..war
 00000990: 6eda 0e52 756e 7469 6d65 5761 726e 696e  n..RuntimeWarnin
 000009a0: 6729 0872 1900 0000 721a 0000 00da 0166  g).r....r......f
 000009b0: 5a09 6a73 6f6e 5f64 6174 6172 1500 0000  Z.json_datar....
 000009c0: 7216 0000 00da 0365 7272 7220 0000 0072  r......errr ...r
 000009d0: 1700 0000 7217 0000 0072 1800 0000 7229  ....r....r....r)
-000009e0: 0000 0033 0000 0073 4800 0000 000f 0201  ...3...sH.......
+000009e0: 0000 0033 0000 0073 4800 0000 000e 0201  ...3...sH.......
 000009f0: 0e01 0a02 0801 1402 0802 0203 0aff 0202  ................
 00000a00: 0efe 0203 0afd 0207 1003 0802 0cff 0202  ................
 00000a10: 0efe 0203 0afd 0205 1203 1201 1201 0a01  ................
 00000a20: 0803 18ff 0208 1a02 0601 0401 0201 0201  ................
 00000a30: 02fd 0606 7229 0000 0029 01da 054d 696e  ....r)...)...Min
 00000a40: 696f fa12 6d69 6e69 6f61 7069 2e74 726f  io..minioapi.tro
 00000a50: 6a61 6964 6576 da04 7072 6f6a da07 6461  jaidev..proj..da
 00000a60: 7461 7365 74da 056d 6f64 656c fa12 7472  taset..model..tr
 00000a70: 6f6a 2d75 7365 722d 6461 7461 7365 7473  oj-user-datasets
 00000a80: 6308 0000 0000 0000 0000 0000 000a 0000  c...............
-00000a90: 0007 0000 0043 0000 0073 9000 0000 7c05  .....C...s....|.
+00000a90: 0007 0000 0043 0000 0073 9800 0000 7c05  .....C...s....|.
 00000aa0: 6400 6b08 7214 7c06 6400 6b08 7214 6401  d.k.r.|.d.k.r.d.
 00000ab0: 8201 7400 7c01 7c05 7c06 6402 6400 6403  ..t.|.|.|.d.d.d.
-00000ac0: 8d05 7d08 7401 6a02 a003 7c00 a101 723e  ..}.t.j...|...r>
-00000ad0: 7401 6a02 a004 7c00 a101 7d09 7c08 a005  t.j...|...}.|...
-00000ae0: 7c07 6404 7c02 1700 6404 1700 7c03 1700  |.d.|...d...|...
-00000af0: 6404 1700 7c04 1700 6404 1700 7c09 1700  d...|...d...|...
-00000b00: 7c00 a103 0100 6405 7c07 1700 6404 1700  |.....d.|...d...
-00000b10: 7c02 1700 6404 1700 7c03 1700 6404 1700  |...d...|...d...
-00000b20: 7c04 1700 6404 1700 7c09 1700 5300 2906  |...d...|...S.).
-00000b30: 4e7a 6a4e 6f20 6d69 6e69 6f20 6372 6564  NzjNo minio cred
-00000b40: 656e 7469 616c 7320 7375 7070 6c69 6564  entials supplied
-00000b50: 2066 6f72 2065 7870 6572 696d 656e 7465   for experimente
-00000b60: 722e 2050 6c65 6173 6520 7061 7373 2074  r. Please pass t
-00000b70: 6865 206b 6579 7320 746f 2074 6865 2065  he keys to the e
-00000b80: 7870 6572 696d 656e 7465 7220 636c 6173  xperimenter clas
-00000b90: 732e 2045 7869 7469 6e67 2e2e 2e46 2902  s. Exiting...F).
-00000ba0: 5a06 7365 6375 7265 5a06 7265 6769 6f6e  Z.secureZ.region
-00000bb0: fa01 2f72 0500 0000 2906 7234 0000 0072  ../r....).r4...r
-00000bc0: 0b00 0000 7213 0000 0072 1400 0000 da08  ....r....r......
-00000bd0: 6261 7365 6e61 6d65 5a0b 6670 7574 5f6f  basenameZ.fput_o
-00000be0: 626a 6563 7429 0a5a 0f6c 6f63 616c 5f66  bject).Z.local_f
-00000bf0: 696c 655f 7061 7468 5a0a 7570 6c6f 6164  ile_pathZ.upload
-00000c00: 5f75 726c 5a07 7072 6f6a 6563 7472 3700  _urlZ.projectr7.
-00000c10: 0000 7238 0000 005a 0a6d 696e 696f 5f75  ..r8...Z.minio_u
-00000c20: 7365 725a 0a6d 696e 696f 5f70 6173 735a  serZ.minio_passZ
-00000c30: 0662 7563 6b65 745a 0663 6c69 656e 74da  .bucketZ.client.
-00000c40: 0966 696c 655f 6e61 6d65 7217 0000 0072  .file_namer....r
-00000c50: 1700 0000 7218 0000 00da 0c6d 696e 696f  ....r......minio
-00000c60: 5f75 706c 6f61 647f 0000 0073 0e00 0000  _upload....s....
-00000c70: 0001 1001 0401 1202 0c01 0c02 2a01 723d  ............*.r=
-00000c80: 0000 0029 0154 2907 7235 0000 0072 3600  ...).T).r5...r6.
-00000c90: 0000 7237 0000 0072 3800 0000 4e4e 7239  ..r7...r8...NNr9
-00000ca0: 0000 0029 0f72 0b00 0000 7208 0000 0072  ...).r....r....r
-00000cb0: 2f00 0000 da07 7061 7468 6c69 6272 0200  /.....pathlibr..
-00000cc0: 0000 5a17 7472 6f6a 7364 6b2e 636f 7265  ..Z.trojsdk.core
-00000cd0: 2e74 726f 6a5f 6572 726f 7272 0300 0000  .troj_errorr....
-00000ce0: 7227 0000 0072 0e00 0000 da04 626f 6f6c  r'...r......bool
-00000cf0: 720d 0000 0072 2900 0000 5a05 6d69 6e69  r....r)...Z.mini
-00000d00: 6f72 3400 0000 723d 0000 0072 1700 0000  or4...r=...r....
-00000d10: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
-00000d20: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
-00000d30: 0000 0801 0801 0801 0c01 0c04 0803 0827  ...............'
-00000d40: 1447 0c01 0804                           .G....
+00000ac0: 8d05 7d08 7401 7c00 8301 0100 7402 6a03  ..}.t.|.....t.j.
+00000ad0: a004 7c00 a101 7246 7402 6a03 a005 7c00  ..|...rFt.j...|.
+00000ae0: a101 7d09 7c08 a006 7c07 6404 7c02 1700  ..}.|...|.d.|...
+00000af0: 6404 1700 7c03 1700 6404 1700 7c04 1700  d...|...d...|...
+00000b00: 6404 1700 7c09 1700 7c00 a103 0100 6405  d...|...|.....d.
+00000b10: 7c07 1700 6404 1700 7c02 1700 6404 1700  |...d...|...d...
+00000b20: 7c03 1700 6404 1700 7c04 1700 6404 1700  |...d...|...d...
+00000b30: 7c09 1700 5300 2906 4e7a 6a4e 6f20 6d69  |...S.).NzjNo mi
+00000b40: 6e69 6f20 6372 6564 656e 7469 616c 7320  nio credentials 
+00000b50: 7375 7070 6c69 6564 2066 6f72 2065 7870  supplied for exp
+00000b60: 6572 696d 656e 7465 722e 2050 6c65 6173  erimenter. Pleas
+00000b70: 6520 7061 7373 2074 6865 206b 6579 7320  e pass the keys 
+00000b80: 746f 2074 6865 2065 7870 6572 696d 656e  to the experimen
+00000b90: 7465 7220 636c 6173 732e 2045 7869 7469  ter class. Exiti
+00000ba0: 6e67 2e2e 2e46 2902 5a06 7365 6375 7265  ng...F).Z.secure
+00000bb0: 5a06 7265 6769 6f6e fa01 2f72 0500 0000  Z.region../r....
+00000bc0: 2907 7234 0000 00da 0570 7269 6e74 720b  ).r4.....printr.
+00000bd0: 0000 0072 1300 0000 7214 0000 00da 0862  ...r....r......b
+00000be0: 6173 656e 616d 655a 0b66 7075 745f 6f62  asenameZ.fput_ob
+00000bf0: 6a65 6374 290a 5a0f 6c6f 6361 6c5f 6669  ject).Z.local_fi
+00000c00: 6c65 5f70 6174 685a 0a75 706c 6f61 645f  le_pathZ.upload_
+00000c10: 7572 6c5a 0770 726f 6a65 6374 7237 0000  urlZ.projectr7..
+00000c20: 0072 3800 0000 5a0a 6d69 6e69 6f5f 7573  .r8...Z.minio_us
+00000c30: 6572 5a0a 6d69 6e69 6f5f 7061 7373 5a06  erZ.minio_passZ.
+00000c40: 6275 636b 6574 5a06 636c 6965 6e74 da09  bucketZ.client..
+00000c50: 6669 6c65 5f6e 616d 6572 1700 0000 7217  file_namer....r.
+00000c60: 0000 0072 1800 0000 da0c 6d69 6e69 6f5f  ...r......minio_
+00000c70: 7570 6c6f 6164 7c00 0000 7340 0000 0000  upload|...s@....
+00000c80: 0a10 0202 ff02 0312 0108 010c 010c 0204  ................
+00000c90: 0102 011e 0102 fd04 0602 0102 ff02 0202  ................
+00000ca0: fe02 0302 fd02 0402 fc02 0502 fb02 0602  ................
+00000cb0: fa02 0702 f902 0802 f802 0902 f702 ff72  ...............r
+00000cc0: 3e00 0000 2901 5429 0772 3500 0000 7236  >...).T).r5...r6
+00000cd0: 0000 0072 3700 0000 7238 0000 004e 4e72  ...r7...r8...NNr
+00000ce0: 3900 0000 290f 720b 0000 0072 0800 0000  9...).r....r....
+00000cf0: 722f 0000 00da 0770 6174 686c 6962 7202  r/.....pathlibr.
+00000d00: 0000 005a 1774 726f 6a73 646b 2e63 6f72  ...Z.trojsdk.cor
+00000d10: 652e 7472 6f6a 5f65 7272 6f72 7203 0000  e.troj_errorr...
+00000d20: 0072 2700 0000 720e 0000 00da 0462 6f6f  .r'...r......boo
+00000d30: 6c72 0d00 0000 7229 0000 005a 056d 696e  lr....r)...Z.min
+00000d40: 696f 7234 0000 0072 3e00 0000 7217 0000  ior4...r>...r...
+00000d50: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000d60: da08 3c6d 6f64 756c 653e 0100 0000 7322  ..<module>....s"
+00000d70: 0000 0008 0108 0108 010c 010c 0408 0308  ................
+00000d80: 2714 450c 0108 0500 0100 0100 0100 0100  '.E.............
+00000d90: 0100 0100 f8                             .....
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/core/data_utils.py` & `trojai-sdk-0.2.3.6/trojsdk/core/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,14 @@
                 if not path_valid:
                     invalid_paths.append(value)
 
     return invalid_paths
 
 
 def load_json_from_disk(json_path: Path, sub_jsons: bool = True) -> dict:
-
     """
     Given a path to the JSON file in pathlib.Path format, (recursively) read and return the
     dictionary stored in the file.
 
     Note that when sub_jsons == True and an excluded name is encountered, the contents of the JSON file will not be
     loaded and the path itself will be stored.
 
@@ -114,24 +113,47 @@
             RuntimeWarning,
             stacklevel=2,
         )
 
     return json_data
 
 
-
 from minio import Minio
 import os
 
 
-
-def minio_upload(local_file_path, upload_url = "minioapi.trojaidev", project = "proj", dataset = "dataset", model = "model",minio_user = None, minio_pass = None, bucket = "troj-user-datasets"):
+def minio_upload(
+    local_file_path,
+    upload_url="minioapi.trojaidev",
+    project="proj",
+    dataset="dataset",
+    model="model",
+    minio_user=None,
+    minio_pass=None,
+    bucket="troj-user-datasets",
+):
     if minio_user is None and minio_pass is None:
-        raise("No minio credentials supplied for experimenter. Please pass the keys to the experimenter class. Exiting...")
-    client = Minio(upload_url, minio_user, minio_pass, secure = False, region=None)
-
+        raise (
+            "No minio credentials supplied for experimenter. Please pass the keys to the experimenter class. Exiting..."
+        )
+    client = Minio(upload_url, minio_user, minio_pass, secure=False, region=None)
+    print(local_file_path)
     if os.path.exists(local_file_path):
         file_name = os.path.basename(local_file_path)
 
-    client.fput_object(bucket, "/"+project +"/"+dataset +"/"+model +"/"+file_name, local_file_path)
-    return "minio://"+bucket+"/"+project +"/"+dataset +"/"+model +"/"+file_name
-
+    client.fput_object(
+        bucket,
+        "/" + project + "/" + dataset + "/" + model + "/" + file_name,
+        local_file_path,
+    )
+    return (
+        "minio://"
+        + bucket
+        + "/"
+        + project
+        + "/"
+        + dataset
+        + "/"
+        + model
+        + "/"
+        + file_name
+    )
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/core/experiment_tools/__init__.py` & `trojai-sdk-0.2.3.6/trojsdk/core/experiment_tools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import json
 from pathlib import Path
 import os
 import shutil
 import pickle
 from trojsdk.core.data_utils import minio_upload
+import stat
 
 
 class TrojExperimenter:
-    #could use JSON lines here but meh
-    '''
-    Used for making experiments more reproducible within the troj platform. 
+    """
+    Used for making experiments more reproducible within the troj platform.
+
+    """
 
-    '''
     def __init__(self, auth_path):
-        '''
+        """
         Takes in an authentication json which contains the api endpoint and keys for Troj, a bucket name, and a local
         path to save runs to. i.e
         :param auth_path: path to the authentication json.
-        '''
+        """
         with open(auth_path, "r") as fp:
             data = json.load(fp)
         self.api_endpoint = data["api_endpoint"]
         self.auth_keys = data["auth_keys"]
         self.secrets = data["secrets"]
         self.docker_metadata = None
         self.k8s_metadata = None
@@ -35,173 +36,255 @@
         if "MINIO_SECRET_KEY" in self.secrets:
             self.minio_pass = self.secrets["MINIO_SECRET_KEY"]
         else:
             self.minio_pass = None
         # Default local dev link
         self.minio_url = "minioapi.trojaidev"
 
-    def create_experiment(self, project_name, dataset_name, model_name, local_save_path = "./",subtask="classification", delete_existing=False):
-        '''
+    def create_experiment(
+        self,
+        project_name,
+        dataset_name,
+        model_name,
+        local_save_path="./",
+        subtask="classification",
+        delete_existing=False,
+    ):
+        """
         Creates the "experiment" folder locally and on S3
 
         :param project_name: Name of the project for the troj platform
         :param dataset_name: name of the dataset on the troj platform
         :param model_name: The desired name of the model.
         :param subtask: Subtask type. Default is classification.
         :param delete_existing: If true, will delete previous experiments with the same name. If false, will error
         if names are duplicated.
 
         :return:
-        '''
+        """
+
+        """
+        TODO readd delete existing
+        """
         self.local = local_save_path
         self.subtask = subtask
         self.model_name = model_name
         self.dataset_name = dataset_name
         self.project_name = project_name
-        self.experiment_name = "{}/{}/{}/".format(project_name, dataset_name, model_name)
+        self.experiment_name = "{}/{}/{}/".format(
+            project_name, dataset_name, model_name
+        )
         self.local_exp_path = os.path.join(self.local, self.experiment_name)
-        Path(self.local_exp_path).mkdir(parents=True, exist_ok=True, mode=777)
-
-
-    def log_data(self, data_file_path, label_column, split, classes_dictionary=None, batch_size=16, shuffle=False):
-        '''
+        if delete_existing and os.path.isdir(self.local_exp_path):
+            shutil.rmtree(self.local_exp_path)
+        os.makedirs(self.local_exp_path, mode=stat.S_IRWXU | stat.S_IRWXG)
+        # Path(self.local_exp_path).mkdir(parents=True, exist_ok=True, mode=777)
+
+    def log_data(
+        self,
+        data_file_path,
+        label_column,
+        split,
+        classes_dictionary=None,
+        batch_size=16,
+        shuffle=False,
+    ):
+        """
         Generic function for saving data to the appropriate run file for upload and creating config.
 
         :param data_file_path: path to data.
         :param label_column: The name of the label column.
         :param split: the split name, used in naming the dataset in the config.
         :param classes_dictionary: Dictionary of class names
         :param batch_size: Desired batch size in config.
         :param shuffle: Whether or not to shuffle the dataframe.
         :return:
-        '''
+        """
         if not data_file_path.startswith(("s3://", "gs://", "minio://")):
             # upload data to minio, local data file
-            upload_res = minio_upload(data_file_path, upload_url = self.minio_url, project = self.project_name, dataset = self.dataset_name, model = self.model_name, minio_user=self.minio_user, minio_pass=self.minio_pass)
+            upload_res = minio_upload(
+                data_file_path,
+                upload_url=self.minio_url,
+                project=self.project_name,
+                dataset=self.dataset_name,
+                model=self.model_name,
+                minio_user=self.minio_user,
+                minio_pass=self.minio_pass,
+            )
             data_file_path = upload_res
-        dloader_config = {"batch_size": batch_size, "shuffle":shuffle}
-        data_config = {"name":self.dataset_name+"_"+split, "path_to_data":data_file_path,
-                       "data_loader_config":dloader_config, "label_column":label_column}
+        dloader_config = {"batch_size": batch_size, "shuffle": shuffle}
+        data_config = {
+            "name": self.dataset_name + "_" + split,
+            "path_to_data": data_file_path,
+            "data_loader_config": dloader_config,
+            "label_column": label_column,
+        }
         if classes_dictionary is not None:
             print("No classes dictionary supplied, loading from data config")
             try:
                 data_config["classes_dictionary"] = classes_dictionary
             except Exception as e:
                 print("No classes dictionary in data config")
-                raise(e)
-            
+                raise (e)
 
         return data_config
 
-    def log_training_data(self, path_to_dset_file, label_column, classes_dictionary=None, batch_size=16, shuffle=False):
-        '''
+    def log_training_data(
+        self,
+        path_to_dset_file,
+        label_column,
+        classes_dictionary=None,
+        batch_size=16,
+        shuffle=False,
+    ):
+        """
         Logs the training data and automatically sets the config.
 
         :param new_file_name:
         :param path_to_file:
         :param label_column:
         :param classes_dictionary:
         :param batch_size:
         :param shuffle:
         :return:
-        '''
-        self.train_data_conf = self.log_data(path_to_dset_file, label_column,
-                                             classes_dictionary=classes_dictionary, batch_size=batch_size, shuffle=shuffle, split="train")
+        """
+        self.train_data_conf = self.log_data(
+            path_to_dset_file,
+            label_column,
+            classes_dictionary=classes_dictionary,
+            batch_size=batch_size,
+            shuffle=shuffle,
+            split="train",
+        )
         save_path = os.path.join(self.local_exp_path, "train_config.json")
-        with open(save_path, "w+") as fp:
+        with open(save_path, "w") as fp:
             json.dump(self.train_data_conf, fp)
 
-    def log_testing_data(self, path_to_dset_file, label_column, classes_dictionary=None, batch_size=16, shuffle=False):
-        '''
+    def log_testing_data(
+        self,
+        path_to_dset_file,
+        label_column,
+        classes_dictionary=None,
+        batch_size=16,
+        shuffle=False,
+    ):
+        """
         logs testing data and automatically sets the config.
 
         :param new_file_name:
         :param path_to_file:
         :param label_column:
         :param classes_dictionary:
         :param batch_size:
         :param shuffle:
         :return:
-        '''
-        self.test_data_conf = self.log_data(path_to_dset_file, label_column,
-                                             classes_dictionary=classes_dictionary, batch_size=batch_size, shuffle=shuffle, split="test")
+        """
+        self.test_data_conf = self.log_data(
+            path_to_dset_file,
+            label_column,
+            classes_dictionary=classes_dictionary,
+            batch_size=batch_size,
+            shuffle=shuffle,
+            split="test",
+        )
         save_path = os.path.join(self.local_exp_path, "test_config.json")
-        with open(save_path, "w+") as fp:
+        with open(save_path, "w") as fp:
             json.dump(self.test_data_conf, fp)
 
-
     def log_model(self, model, model_wrapper_file, **model_kwargs):
-        '''
+        """
         Saves model and makes the model config.
 
         :param model: Either a picklable model, or a path to a model file.
         :param model_wrapper_file: The path to the model wrapper file.
         :param model_kwargs: Any model keyword arguments
         :return: Saves model, and makes model json.
-        '''
+        """
         model_file_res = model_wrapper_file
         model_res = model
 
         # if model not hosted on s3 or minio, upload to minio
         if not model_wrapper_file.startswith(("s3://", "gs://", "minio://")):
-            model_file_res = minio_upload(model_wrapper_file, upload_url = self.minio_url, project = self.project_name, dataset = self.dataset_name, model = self.model_name, minio_user=self.minio_user, minio_pass=self.minio_pass)
+            model_file_res = minio_upload(
+                model_wrapper_file,
+                upload_url=self.minio_url,
+                project=self.project_name,
+                dataset=self.dataset_name,
+                model=self.model_name,
+                minio_user=self.minio_user,
+                minio_pass=self.minio_pass,
+            )
             if not model.startswith(("s3://", "gs://", "minio://")):
-                model_res = minio_upload(model, upload_url = self.minio_url, project = self.project_name, dataset = self.dataset_name, model = self.model_name, minio_user=self.minio_user, minio_pass=self.minio_pass)
-
-
-        self.model_config = {"name":self.model_name, "path_to_model_file":model_file_res, "model_args_dict":{**model_kwargs, "model_file": model_res}}
+                model_res = minio_upload(
+                    model,
+                    upload_url=self.minio_url,
+                    project=self.project_name,
+                    dataset=self.dataset_name,
+                    model=self.model_name,
+                    minio_user=self.minio_user,
+                    minio_pass=self.minio_pass,
+                )
+
+        self.model_config = {
+            "name": self.model_name,
+            "path_to_model_file": model_file_res,
+            "model_args_dict": {**model_kwargs, "model_file": model_res},
+        }
 
         save_path = os.path.join(self.local_exp_path, "model_config.json")
 
-        with open(save_path, "w+") as fp:
+        with open(save_path, "w") as fp:
             json.dump(self.model_config, fp)
 
-
-
-    def log_docker_metadata(self, docker_image_url, docker_secret_name, image_pull_policy):
+    def log_docker_metadata(self, docker_image, docker_secret_name, image_pull_policy):
+        """
+        Logs the docker image metadata for use during evaluation.
+        :param docker_image: a valid docker image tag
+        :param docker_secret_name: the env var that stores the docker pull secret in cluster
+        :param image_pull_policy: the pull policy for the image
+        """
         docker_meta = {
             "docker_metadata": {
-                "docker_image_url": docker_image_url,
+                "docker_image_url": docker_image,
                 "docker_secret_name": docker_secret_name,
-                "image_pull_policy": image_pull_policy
-                
+                "image_pull_policy": image_pull_policy,
             }
         }
         self.docker_metadata = docker_meta
         save_path = os.path.join(self.local_exp_path, "docker_config.json")
-        with open(save_path, "w+") as fp:
+        with open(save_path, "w") as fp:
             json.dump(self.docker_metadata, fp)
 
-
     def log_k8s_metadata(self, k8s_meta_dict):
-        k8s_meta = {
-            "k8s_metadata": k8s_meta_dict
-            }
+        """
+        Logs the metadata regarding the newly spawned k8s container. You can customize this as you see fit or just use the config that we use.
+        :param k8s_meta_dict: dict containing all the data regarding the instantiation of a new kubernetes pod
+        """
+        k8s_meta = {"k8s_metadata": k8s_meta_dict}
         self.k8s_metadata = k8s_meta
         save_path = os.path.join(self.local_exp_path, "k8s_config.json")
-        with open(save_path, "w+") as fp:
+        with open(save_path, "w") as fp:
             json.dump(self.k8s_metadata, fp)
 
-
     def log_attacks(self, attacks=None):
-        '''
+        """
         Creates the attacks json either by copying a json or by a dictionary.
 
         :param attacks: Either a dictionary or the path to a JSON.
         :return:
-        '''
+        """
         if attacks is None:
             self.attacks = False
         elif type(attacks) == str:
             self.attacks = True
             shutil.copyfile(attacks, os.path.join(self.local_exp_path, "attacks.json"))
         elif type(attacks) == dict:
             save_path = os.path.join(self.local_exp_path, "attacks.json")
             self.attacks = True
-            with open(save_path, "w+") as fp:
+            with open(save_path, "w") as fp:
                 json.dump(attacks, fp)
 
     def log_checks(self, checks):
         if type(checks) == str:
             if checks.split(".")[-1] == "json":
                 self._set_checks_from_path(checks)
             else:
@@ -209,125 +292,133 @@
         elif type(checks) == dict:
             self.checks_list.append(checks)
         elif type(checks) == list:
             for i in checks:
                 self.checks_list.append(i)
 
     def reset(self):
-        '''
+        """
         Resets the internal values.
         :return:
-        '''
+        """
         self.base = {}
         self.attack_list = []
         self.checks_list = []
         self.test_data_conf = None
         self.train_data_conf = None
         self.custom_checks = None
         self.custom_eval = None
         self.custom_eval_kwargs = None
 
     def create_auth(self, project_name=None, dataset_name=None):
         auth = {}
         auth["api_endpoint"] = self.api_endpoint
         auth["auth_keys"] = self.auth_keys
-        if project_name==None:
+        auth["secrets"] = self.secrets
+        if project_name == None:
             auth["project_name"] = self.project_name
             auth["dataset_name"] = self.dataset_name
         else:
             auth["project_name"] = project_name
             auth["dataset_name"] = dataset_name
         return auth
 
-    def construct_base_config(self, audit=True, run_attacks_from_profile=True, task_type = None):
+    def construct_base_config(
+        self, audit=True, run_attacks_from_profile=True, task_type=None
+    ):
         base_conf = {}
         base_conf["test_run_name"] = self.experiment_name
         base_conf["task_type"] = task_type
         base_conf["audit"] = audit
         base_conf["run_attacks_from_model_profile"] = run_attacks_from_profile
         if self.test_data_conf is not None:
-            '''
+            """
             if data file path is local, upload to minio, return the path to the minio upload as well to replace in config
-            '''
-            base_conf["dataset"] = self.local_exp_path+"test_config.json"
+            """
+            base_conf["dataset"] = self.local_exp_path + "test_config.json"
         if self.train_data_conf is not None:
-            '''
+            """
             if data file path is local, upload to minio, return the path to the minio upload as well to replace in config
-            '''
-            base_conf["train_dataset"] = self.local_exp_path+"train_config.json"
-        base_conf["model"] = self.local_exp_path+"model_config.json"
+            """
+            base_conf["train_dataset"] = self.local_exp_path + "train_config.json"
+        base_conf["model"] = self.local_exp_path + "model_config.json"
         auth_dict = self.create_auth()
         save_path = os.path.join(self.local_exp_path, "auth.json")
-        with open(save_path, "w+") as fp:
+        with open(save_path, "w") as fp:
             json.dump(auth_dict, fp)
-        base_conf["auth_config"] = self.local_exp_path+"auth.json"
+        base_conf["auth_config"] = self.local_exp_path + "auth.json"
         base_save_path = os.path.join(self.local_exp_path, "base.json")
         base_conf["docker_metadata"] = self.docker_metadata["docker_metadata"]
         if self.k8s_metadata is not None:
-            base_conf["k8s_metadata"]  = self.k8s_metadata
+            base_conf["k8s_metadata"] = self.k8s_metadata
 
-        with open(base_save_path, "w+") as fp:
+        with open(base_save_path, "w") as fp:
             json.dump(base_conf, fp)
         print("configs constructed!")
 
     def upload_experiment(self, delete_after_upload=False):
         # change this to send with tsdk to auth config api endpoint
         self.handler.upload_folder_contents(self.local_exp_path, self.experiment_name)
 
     def set_auth(self, experiment):
-        #used to set the authentication after pulling
+        # used to set the authentication after pulling
         local_path = os.path.join(self.local, experiment)
         auth_path = os.path.join(local_path, "auth.json")
         with open(auth_path, "r") as fp:
             current_auth = json.load(fp)
             current_auth["auth_keys"] = self.auth_keys
-        with open(auth_path, "w+") as fp:
+        with open(auth_path, "w") as fp:
             json.dump(current_auth, fp)
 
-    
     def _set_attacks_from_path(self, path):
         attack_dict = json.load(path)
         self.attack_list = self.attack_list + attack_dict["attacks"]
 
     def _set_checks_from_path(self, path):
         checks_dict = json.load(path)
         self.checks_list = self.checks_list + checks_dict["integrity_checks"]
 
-
     def set_custom_eval(self, file_path, args_dict=None):
-        shutil.copyfile(file_path, os.path.join(self.local_exp_path, "custom_attacks.py"))
+        shutil.copyfile(
+            file_path, os.path.join(self.local_exp_path, "custom_attacks.py")
+        )
         self.custom_eval = "./custom_attacks.py"
         self.custom_eval_kwargs = args_dict
 
     def set_custom_checks(self, file_path):
-        shutil.copyfile(file_path, os.path.join(self.local_exp_path, "custom_checks.py"))
+        shutil.copyfile(
+            file_path, os.path.join(self.local_exp_path, "custom_checks.py")
+        )
         self.custom_checks = "./custom_checks.py"
 
-
     def set_integrity_checks(self):
-        #TODO
+        # TODO
         pass
 
-    def run_troj_evaluation(self, project, dataset, model, no_ssl = False):
+    def run_troj_evaluation(self, project, dataset, model, no_ssl=False):
         import os
-        from trojsdk.core import client_utils
+        from trojsdk.core.client_utils import submit_evaluation
+
         exp_name = "{}/{}/{}/".format(project, dataset, model)
         folder = os.path.join(self.local, exp_name)
         abs_path = os.path.abspath(folder)
         # config, docker_metadata, k8s_metadata = client_utils.config_from_dict(config_dict)
-        return client_utils.submit_evaluation(path_to_config=abs_path+"/base.json")
-
+        return submit_evaluation(path_to_config=abs_path + "/base.json", nossl=no_ssl)
 
+    def dump_auth(self):
+        return {
+            "api_endpoint": self.api_endpoint,
+            "project_name": self.project_name,
+            "dataset_name": self.dataset_name,
+            "auth_keys": self.auth_keys,
+            "secrets": self.secrets,
+        }
 
     def run_all_experiments_from_dataset(self, project, dataset):
         dset_name = "{}/{}/".format(project, dataset)
         experiments = self.handler.get_experiment_folders(dset_name)
-        for i,exp in enumerate(experiments):
-            print("running experiment {} of {}".format(i+1, len(experiments)))
-            exp_folder = '/'.join(exp)+'/'
-            #print(exp_folder)
+        for i, exp in enumerate(experiments):
+            print("running experiment {} of {}".format(i + 1, len(experiments)))
+            exp_folder = "/".join(exp) + "/"
+            # print(exp_folder)
             self.pull_experiment(exp_folder)
             self.run_troj_evaluation(exp[0], exp[1], exp[2])
-
-
-
-
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/core/troj_error.py` & `trojai-sdk-0.2.3.6/trojsdk/core/troj_error.py`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/auth_config.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/auth_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/gcloud_tests/gcloud_auth.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/gcloud_tests/gcloud_auth.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/label_map_num.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/label_map_num.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil/troj_config.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil/troj_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/nlp_phil_test.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/nlp_phil_test.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/nlp_test_main.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/nlp_test_main.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/s3_small_classification_pt_config.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/s3_small_classification_pt_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/tabular_SMOTETomek_logistic_base.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/tabular_SMOTETomek_logistic_base.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/tabular_medical_insurance_config.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/tabular_medical_insurance_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/all_pipe_transform_config.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/all_pipe_transform_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/tabular_test_main.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/tabular_test_main.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/tabular_test/troj_dev_auth.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/tabular_test/troj_dev_auth.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/examples/testing_config.json` & `trojai-sdk-0.2.3.6/trojsdk/examples/testing_config.json`

 * *Files identical despite different names*

### Comparing `trojai-sdk-0.2.3.4/trojsdk/setup.py` & `trojai-sdk-0.2.3.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+extras = {}
+
+extras["testing"] = [
+    "plotly",
+    "wandb"
+]
+
+
+
 setup(
-    name="trojsdk",
-    version="0.1",
+    name="trojai-sdk",
+    version="0.2.3.6",
     packages=find_packages(),
     author="TrojAI",
     author_email="stan.petley@troj.ai",
     description="TrojAI provides the troj Python convenience package to allow users to integrate TrojAI adversarial protections and robustness metrics seamlessly into their AI development pipelines.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://troj.ai",
@@ -17,9 +26,9 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=open("requirements.txt").readlines(),
     python_requires=">=3.6",
-    entry_points={"console_scripts": ["trojsdk = trojsdk.cmd:main"]},
+    entry_points={"console_scripts": ["tsdk = trojsdk.cmd:main"]},
 )
```

### Comparing `trojai-sdk-0.2.3.4/trojsdk/test_sdk.py` & `trojai-sdk-0.2.3.6/trojsdk/test_sdk.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from trojsdk.core import data_utils
 from trojsdk.core import client_utils
 from trojsdk.core.client_utils import TrojJobHandler
 
 
 def test_sdk_fail():
-
     troj_job_handler = TrojJobHandler()
     try:
-        troj_job_handler.check_job_status()
+        troj_job_handler.list_stress_test_jobs()
         assert False
     except:
         assert True
 
 
 def test_sdk_pass_tabular():
-
     troj_job_handler = client_utils.submit_evaluation(
-        path_to_config="./trojsdk/examples/tabular_medical_insurance_config.json", nossl=True
+        path_to_config="./trojsdk/examples/tabular_medical_insurance_config.json",
+        nossl=True,
     )
 
     import time
 
     time.sleep(2)
     try:
-        troj_job_handler.check_job_status()
-        print(troj_job_handler.status_response["data"])
+        resp = troj_job_handler.list_stress_test_jobs(pretty=False)
+        print(resp)
         assert True
     except Exception as e:
         print(e)
         assert False
```


# Comparing `tmp/resoto-plugin-aws-3.4.2.tar.gz` & `tmp/resoto-plugin-aws-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-3.4.2.tar", last modified: Wed May 10 12:22:37 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-3.5.0.tar", last modified: Fri May 26 18:24:37 2023, max compression
```

## Comparing `resoto-plugin-aws-3.4.2.tar` & `resoto-plugin-aws-3.5.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.724384 resoto-plugin-aws-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-10 12:22:37.724384 resoto-plugin-aws-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.716384 resoto-plugin-aws-3.4.2/resoto_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.716384 resoto-plugin-aws-3.4.2/resoto_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.720384 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    53709 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)   114504 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    77860 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26166 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (123)    31197 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39833 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)   234069 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.716384 resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-10 12:22:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-10 12:22:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 12:22:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:20:27.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 12:22:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 12:22:37.000000 resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 12:22:37.724384 resoto-plugin-aws-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.720384 resoto-plugin-aws-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.724384 resoto-plugin-aws-3.4.2/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-10 12:19:37.000000 resoto-plugin-aws-3.4.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.927827 resoto-plugin-aws-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-26 18:24:37.927827 resoto-plugin-aws-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.919828 resoto-plugin-aws-3.5.0/resoto_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.919828 resoto-plugin-aws-3.5.0/resoto_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.923828 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53709 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114499 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77860 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26166 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31197 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39833 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234069 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.919828 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:22:28.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 18:24:37.931827 resoto-plugin-aws-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.923828 resoto-plugin-aws-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.927827 resoto-plugin-aws-3.5.0/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/test_utils.py
```

### Comparing `resoto-plugin-aws-3.4.2/PKG-INFO` & `resoto-plugin-aws-3.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto AWS Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.4.2/README.md` & `resoto-plugin-aws-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/__init__.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/aws_client.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/collector.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/configuration.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/configuration.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/apigateway.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/apigateway.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/athena.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/autoscaling.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/base.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cloudformation.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudformation.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cloudfront.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cloudtrail.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cloudwatch.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/cognito.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cognito.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/config.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/dynamodb.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/ec2.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,21 +457,21 @@
                 if non_zero := metric.first_non_zero():
                     at, value = non_zero
                     if vol := lookup.get(query.ref_id):
                         if metric.label == "VolumeReadOps":
                             vol.atime = at
                         elif metric.label == "VolumeWriteOps":
                             vol.mtime = at
-                        lookup.pop(query.ref_id, None)
-            # all volumes in this list do not have value in cloudwatch
-            # fall back to either ctime or start time whatever is more recent.
+            # fall back to either ctime or start time whatever is more recent for all volumes cloudwatch did not return
             for v in lookup.values():
                 t = max(v.ctime or start, start)
-                v.atime = t
-                v.mtime = t
+                if v.atime is None:
+                    v.atime = t
+                if v.mtime is None:
+                    v.mtime = t
 
         for js in json:
             instance = builder.add_node(AwsEc2Volume.from_api(js), js)
             volumes.append(instance)
             if vt := builder.volume_type(instance.volume_type):
                 builder.add_edge(vt, EdgeType.default, node=instance)
         update_atime_mtime()
```

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/ecs.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/ecs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/efs.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/eks.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/eks.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/elasticache.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/elasticbeanstalk.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/elb.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/elbv2.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elbv2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/glacier.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/glacier.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/iam.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/iam.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/kinesis.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/kms.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/lambda_.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/lambda_.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/pricing.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/pricing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/rds.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/redshift.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/route53.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/route53.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/s3.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/sagemaker.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sagemaker.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/service_quotas.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/service_quotas.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/sns.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sns.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/resource/sqs.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws/utils.py` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/PKG-INFO` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto AWS Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.4.2/resoto_plugin_aws.egg-info/SOURCES.txt` & `resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/setup.py` & `resoto-plugin-aws-3.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-aws",
-    version="3.4.2",
+    version="3.5.0",
     description="Resoto AWS Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": ["aws = resoto_plugin_aws:AWSCollectorPlugin"],
```

### Comparing `resoto-plugin-aws-3.4.2/test/__init__.py` & `resoto-plugin-aws-3.5.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/aws_client_test.py` & `resoto-plugin-aws-3.5.0/test/aws_client_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/collector_test.py` & `resoto-plugin-aws-3.5.0/test/collector_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/configuration_test.py` & `resoto-plugin-aws-3.5.0/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/graphbuilder_test.py` & `resoto-plugin-aws-3.5.0/test/graphbuilder_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/__init__.py` & `resoto-plugin-aws-3.5.0/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/apigateway_test.py` & `resoto-plugin-aws-3.5.0/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/athena_test.py` & `resoto-plugin-aws-3.5.0/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/autoscaling_test.py` & `resoto-plugin-aws-3.5.0/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/base_test.py` & `resoto-plugin-aws-3.5.0/test/resources/base_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/cloudformation_test.py` & `resoto-plugin-aws-3.5.0/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/cloudfront_test.py` & `resoto-plugin-aws-3.5.0/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/cloudtrail_test.py` & `resoto-plugin-aws-3.5.0/test/resources/cloudtrail_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/cloudwatch_test.py` & `resoto-plugin-aws-3.5.0/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/cognito_test.py` & `resoto-plugin-aws-3.5.0/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/dynamodb_test.py` & `resoto-plugin-aws-3.5.0/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/ec2_test.py` & `resoto-plugin-aws-3.5.0/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/ecs_test.py` & `resoto-plugin-aws-3.5.0/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/eks_test.py` & `resoto-plugin-aws-3.5.0/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/elasticache_test.py` & `resoto-plugin-aws-3.5.0/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/elasticbeanstalk_test.py` & `resoto-plugin-aws-3.5.0/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/elb_test.py` & `resoto-plugin-aws-3.5.0/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/elbv2_test.py` & `resoto-plugin-aws-3.5.0/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/glacier_test.py` & `resoto-plugin-aws-3.5.0/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/iam_test.py` & `resoto-plugin-aws-3.5.0/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/kinesis_test.py` & `resoto-plugin-aws-3.5.0/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/kms_test.py` & `resoto-plugin-aws-3.5.0/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/lambda_test.py` & `resoto-plugin-aws-3.5.0/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/pricing_test.py` & `resoto-plugin-aws-3.5.0/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/rds_test.py` & `resoto-plugin-aws-3.5.0/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/redshift_test.py` & `resoto-plugin-aws-3.5.0/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/route53_test.py` & `resoto-plugin-aws-3.5.0/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/s3_test.py` & `resoto-plugin-aws-3.5.0/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/sagemaker_test.py` & `resoto-plugin-aws-3.5.0/test/resources/sagemaker_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/service_quotas_test.py` & `resoto-plugin-aws-3.5.0/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/sns_test.py` & `resoto-plugin-aws-3.5.0/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.4.2/test/resources/sqs_test.py` & `resoto-plugin-aws-3.5.0/test/resources/sqs_test.py`

 * *Files identical despite different names*


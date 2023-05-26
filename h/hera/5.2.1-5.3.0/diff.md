# Comparing `tmp/hera-5.2.1.tar.gz` & `tmp/hera-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera-5.2.1.tar", max compression
+gzip compressed data, was "hera-5.3.0.tar", max compression
```

## Comparing `hera-5.2.1.tar` & `hera-5.3.0.tar`

### file list

```diff
@@ -1,133 +1,134 @@
--rw-r--r--   0        0        0     1066 2023-05-25 15:41:22.997757 hera-5.2.1/LICENSE
--rw-r--r--   0        0        0    11980 2023-05-25 15:41:22.997757 hera-5.2.1/README.md
--rw-r--r--   0        0        0     3530 2023-05-25 15:41:37.981668 hera-5.2.1/pyproject.toml
--rw-r--r--   0        0        0      522 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/__init__.py
--rw-r--r--   0        0        0      300 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/_version.py
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3267 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.013757 hera-5.2.1/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    26811 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/events/service.py
--rw-r--r--   0        0        0      282 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12021 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/py.typed
--rw-r--r--   0        0        0      188 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      269 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     4927 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0      513 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4585 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     2912 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/_context.py
--rw-r--r--   0        0        0    27751 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0    32815 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/_unparse.py
--rw-r--r--   0        0        0       25 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/action.py
--rw-r--r--   0        0        0     1115 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/archive.py
--rw-r--r--   0        0        0     7697 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3464 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/container.py
--rw-r--r--   0        0        0     7280 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     3763 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     2877 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2241 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/data.py
--rw-r--r--   0        0        0     4855 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1329 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      208 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2346 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0       30 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/memoize.py
--rw-r--r--   0        0        0     4418 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/metrics.py
--rw-r--r--   0        0        0     6913 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.017757 hera-5.2.1/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      722 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4084 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1018 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     3146 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5262 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     1856 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0     3707 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    14836 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/script.py
--rw-r--r--   0        0        0    49251 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/service.py
--rw-r--r--   0        0        0     9148 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3332 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0    10501 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/task.py
--rw-r--r--   0        0        0       27 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     2007 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2610 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    18656 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    15738 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0      911 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     5509 2023-05-25 15:41:23.021757 hera-5.2.1/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0    13403 1970-01-01 00:00:00.000000 hera-5.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-26 16:26:41.880003 hera-5.3.0/LICENSE
+-rw-r--r--   0        0        0    11980 2023-05-26 16:26:41.880003 hera-5.3.0/README.md
+-rw-r--r--   0        0        0     3530 2023-05-26 16:26:57.651977 hera-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/__init__.py
+-rw-r--r--   0        0        0      300 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/_version.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3267 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    27607 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/service.py
+-rw-r--r--   0        0        0     2186 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/exceptions/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12021 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/py.typed
+-rw-r--r--   0        0        0      188 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      269 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     4927 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0      513 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4585 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     2912 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0    34769 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32815 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0       25 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/action.py
+-rw-r--r--   0        0        0     1115 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0     7697 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3464 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     7280 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     3779 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     2877 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2241 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     4855 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1329 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      208 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2346 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0       30 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/memoize.py
+-rw-r--r--   0        0        0     4418 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/metrics.py
+-rw-r--r--   0        0        0     6913 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      722 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4084 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1018 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     3146 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5262 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     1856 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0     3707 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    16549 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    55322 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     6738 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3332 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0     8071 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/task.py
+-rw-r--r--   0        0        0       27 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     2007 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2610 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    18656 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    18117 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0      911 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     7334 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0    13403 1970-01-01 00:00:00.000000 hera-5.3.0/PKG-INFO
```

### Comparing `hera-5.2.1/LICENSE` & `hera-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/README.md` & `hera-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/pyproject.toml` & `hera-5.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera"  # project-name
 # The version is automatically substituted by the CI
-version = "5.2.1"
+version = "5.3.0"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera-5.2.1/src/hera/__init__.py` & `hera-5.3.0/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/__init__.py` & `hera-5.3.0/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/eventsource.py` & `hera-5.3.0/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/eventsource.pyi` & `hera-5.3.0/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/grpc/gateway/runtime.py` & `hera-5.3.0/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera-5.3.0/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.3.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.3.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.3.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/k8s/api/core/v1.py` & `hera-5.3.0/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera-5.3.0/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera-5.3.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/sensor.py` & `hera-5.3.0/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/events/models/sensor.pyi` & `hera-5.3.0/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/expr/_node.py` & `hera-5.3.0/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/expr/_sprig.py` & `hera-5.3.0/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/shared/_global_config.py` & `hera-5.3.0/src/hera/shared/_global_config.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/shared/serialization.py` & `hera-5.3.0/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/__init__.py` & `hera-5.3.0/src/hera/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/_context.py` & `hera-5.3.0/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/_mixins.py` & `hera-5.3.0/src/hera/workflows/_mixins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import inspect
-from typing import Any, Callable, Dict, List, Optional, Set, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, TypeVar, Union, cast
 
 from pydantic import root_validator, validator
 
 from hera.shared import BaseMixin, global_config
 from hera.shared.serialization import serialize
 from hera.workflows._context import SubNodeMixin, _context
 from hera.workflows.artifact import Artifact
@@ -50,18 +50,24 @@
     Toleration,
     UserContainer as ModelUserContainer,
     Volume as ModelVolume,
     VolumeDevice,
     VolumeMount,
 )
 from hera.workflows.parameter import MISSING, Parameter
+from hera.workflows.protocol import Templatable
 from hera.workflows.resources import Resources
 from hera.workflows.user_container import UserContainer
 from hera.workflows.volume import Volume, _BaseVolume
 
+if TYPE_CHECKING:
+    from hera.workflows.steps import Step
+    from hera.workflows.task import Task
+
+
 InputsT = Optional[
     Union[
         ModelInputs,
         Union[Parameter, ModelParameter, Artifact, ModelArtifact, Dict[str, Any]],
         List[Union[Parameter, ModelParameter, Artifact, ModelArtifact, Dict[str, Any]]],
     ]
 ]
@@ -457,15 +463,15 @@
 
         if result.parameters is None and result.artifacts is None:
             return None
         return result
 
 
 class CallableTemplateMixin(ArgumentsMixin):
-    def __call__(self, *args, **kwargs) -> Optional[SubNodeMixin]:
+    def __call__(self, *args, **kwargs) -> Union[Step, Task]:
         if "name" not in kwargs:
             kwargs["name"] = self.name  # type: ignore
 
         # when the `source` is set via an `@script` decorator, it does not come in with the `kwargs` so we need to
         # set it here in order for the following logic to capture it
         if "source" not in kwargs and hasattr(self, "source"):
             kwargs["source"] = self.source  # type: ignore
@@ -661,24 +667,204 @@
     on_exit: Optional[str] = None
     template: Optional[Union[str, Template, TemplateMixin]] = None
     template_ref: Optional[TemplateRef] = None
     inline: Optional[Union[Template, TemplateMixin]] = None
     when: Optional[str] = None
     with_sequence: Optional[Sequence] = None
 
+    @property
+    def _subtype(self) -> str:
+        raise NotImplementedError
+
+    @property
+    def id(self) -> str:
+        """ID of this node."""
+        return f"{{{{{self._subtype}.{self.name}.id}}}}"
+
+    @property
+    def ip(self) -> str:
+        """IP of this node."""
+        return f"{{{{{self._subtype}.{self.name}.ip}}}}"
+
+    @property
+    def status(self) -> str:
+        """Status of this node."""
+        return f"{{{{{self._subtype}.{self.name}.status}}}}"
+
+    @property
+    def exit_code(self) -> str:
+        """ExitCode holds the exit code of a script template."""
+        return f"{{{{{self._subtype}.{self.name}.exitCode}}}}"
+
+    @property
+    def started_at(self) -> str:
+        """Time at which this node started."""
+        return f"{{{{{self._subtype}.{self.name}.startedAt}}}}"
+
+    @property
+    def finished_at(self) -> str:
+        """Time at which this node completed."""
+        return f"{{{{{self._subtype}.{self.name}.finishedAt}}}}"
+
+    @property
+    def result(self) -> str:
+        """Result holds the result (stdout) of a script template."""
+        return f"{{{{{self._subtype}.{self.name}.outputs.result}}}}"
+
     @root_validator(pre=False)
     def _check_values(cls, values):
         def one(xs: List):
             xs = list(map(bool, xs))
             return xs.count(True) == 1
 
         if not one([values.get("template"), values.get("template_ref"), values.get("inline")]):
             raise ValueError("exactly one of ['template', 'template_ref', 'inline'] must be present")
         return values
 
+    def _get_parameters_as(self, name: str, subtype: str) -> Parameter:
+        """Returns a `Parameter` that represents all the outputs of the specified subtype.
+
+        Parameters
+        ----------
+        name: str
+            The name of the parameter to search for.
+        subtype: str
+            The inheritor subtype field, used to construct the output artifact `from_` reference.
+
+        Returns
+        -------
+        Parameter
+            The parameter, named based on the given `name`, along with a value that references all outputs.
+        """
+        return Parameter(name=name, value=f"{{{{{subtype}.{self.name}.outputs.parameters}}}}")
+
+    def _get_parameter(self, name: str, subtype: str) -> Parameter:
+        """Attempts to find the specified parameter in the outputs for the specified subtype.
+
+        Notes
+        -----
+        This is specifically designed to be invoked by inheritors.
+
+        Parameters
+        ----------
+        name: str
+            The name of the parameter to search for.
+        subtype: str
+            The inheritor subtype field, used to construct the output artifact `from_` reference.
+
+        Returns
+        -------
+        Parameter
+            The parameter if found.
+
+        Raises
+        ------
+        ValueError
+            When no outputs can be constructed/no outputs are set.
+        KeyError
+            When the artifact is not found.
+        NotImplementedError
+            When something else other than an `Parameter` is found for the specified name.
+        """
+        if isinstance(self.template, str):
+            raise ValueError(f"Cannot get output parameters when the template was set via a name: {self.template}")
+
+        # here, we build the template early to verify that we can get the outputs
+        if isinstance(self.template, Templatable):
+            template = self.template._build_template()
+        else:
+            template = self.template
+
+        # at this point, we know that the template is a `Template` object
+        if template.outputs is None:  # type: ignore
+            raise ValueError(f"Cannot get output parameters when the template has no outputs: {template}")
+        if template.outputs.parameters is None:  # type: ignore
+            raise ValueError(f"Cannot get output parameters when the template has no output parameters: {template}")
+        parameters = template.outputs.parameters  # type: ignore
+
+        obj = next((output for output in parameters if output.name == name), None)
+        if obj is not None:
+            return Parameter(
+                name=obj.name,
+                value=f"{{{{{subtype}.{self.name}.outputs.parameters.{name}}}}}",
+            )
+        raise KeyError(f"No output parameter named `{name}` found")
+
+    def _get_artifact(self, name: str, subtype: str) -> Artifact:
+        """Attempts to find the specified artifact in the outputs for the specified subtype.
+
+        Notes
+        -----
+        This is specifically designed to be invoked by inheritors.
+
+        Parameters
+        ----------
+        name: str
+            The name of the artifact to search for.
+        subtype: str
+            The inheritor subtype field, used to construct the output artifact `from_` reference.
+
+        Returns
+        -------
+        Artifact
+            The artifact if found.
+
+        Raises
+        ------
+        ValueError
+            When no outputs can be constructed/no outputs are set.
+        KeyError
+            When the artifact is not found.
+        NotImplementedError
+            When something else other than an `Artifact` is found for the specified name.
+        """
+        if isinstance(self.template, str):
+            raise ValueError(f"Cannot get output parameters when the template was set via a name: {self.template}")
+
+        # here, we build the template early to verify that we can get the outputs
+        if isinstance(self.template, Templatable):
+            template = self.template._build_template()
+        else:
+            template = cast(Template, self.template)
+
+        # at this point, we know that the template is a `Template` object
+        if template.outputs is None:  # type: ignore
+            raise ValueError(f"Cannot get output artifacts when the template has no outputs: {template}")
+        elif template.outputs.artifacts is None:  # type: ignore
+            raise ValueError(f"Cannot get output artifacts when the template has no output artifacts: {template}")
+        artifacts = cast(List[ModelArtifact], template.outputs.artifacts)
+
+        obj = next((output for output in artifacts if output.name == name), None)
+        if obj is not None:
+            return Artifact(name=name, path=obj.path, from_=f"{{{{{subtype}.{self.name}.outputs.artifacts.{name}}}}}")
+        raise KeyError(f"No output artifact named `{name}` found")
+
+    def get_parameters_as(self, name: str) -> Parameter:
+        """Returns a `Parameter` that represents all the outputs of this subnode.
+
+        Parameters
+        ----------
+        name: str
+            The name of the parameter to search for.
+
+        Returns
+        -------
+        Parameter
+            The parameter, named based on the given `name`, along with a value that references all outputs.
+        """
+        return self._get_parameters_as(name=name, subtype=self._subtype)
+
+    def get_artifact(self, name: str) -> Artifact:
+        """Gets an artifact from the outputs of this subnode"""
+        return self._get_artifact(name=name, subtype=self._subtype)
+
+    def get_parameter(self, name: str) -> Parameter:
+        """Gets a parameter from the outputs of this subnode"""
+        return self._get_parameter(name=name, subtype=self._subtype)
+
 
 def _get_params_from_source(source: Callable) -> Optional[List[Parameter]]:
     source_signature: Dict[str, Optional[object]] = {}
     for p in inspect.signature(source).parameters.values():
         if p.default != inspect.Parameter.empty and p.kind == inspect.Parameter.POSITIONAL_OR_KEYWORD:
             source_signature[p.name] = p.default
         else:
```

### Comparing `hera-5.2.1/src/hera/workflows/_unparse.py` & `hera-5.3.0/src/hera/workflows/_unparse.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/archive.py` & `hera-5.3.0/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/artifact.py` & `hera-5.3.0/src/hera/workflows/artifact.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/container.py` & `hera-5.3.0/src/hera/workflows/container.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/container_set.py` & `hera-5.3.0/src/hera/workflows/container_set.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/cron_workflow.py` & `hera-5.3.0/src/hera/workflows/cron_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 timezone=self.timezone,
                 workflow_metadata=None,
                 workflow_spec=super().build().spec,
             ),
             status=self.cron_status,
         )
 
-    def create(self) -> TWorkflow:
+    def create(self) -> TWorkflow:  # type: ignore
         """Creates the CronWorkflow on the Argo cluster."""
         assert self.workflows_service, "workflow service not initialized"
         assert self.namespace, "workflow namespace not defined"
         return self.workflows_service.create_cron_workflow(
             CreateCronWorkflowRequest(cron_workflow=self.build()), namespace=self.namespace
         )
```

### Comparing `hera-5.2.1/src/hera/workflows/dag.py` & `hera-5.3.0/src/hera/workflows/dag.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/data.py` & `hera-5.3.0/src/hera/workflows/data.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/env.py` & `hera-5.3.0/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/env_from.py` & `hera-5.3.0/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/http_template.py` & `hera-5.3.0/src/hera/workflows/http_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/metrics.py` & `hera-5.3.0/src/hera/workflows/metrics.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/__init__.py` & `hera-5.3.0/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/eventsource.py` & `hera-5.3.0/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/eventsource.pyi` & `hera-5.3.0/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera-5.3.0/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera-5.3.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.3.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera-5.3.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/sensor.py` & `hera-5.3.0/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/models/sensor.pyi` & `hera-5.3.0/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/operator.py` & `hera-5.3.0/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/parameter.py` & `hera-5.3.0/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/protocol.py` & `hera-5.3.0/src/hera/workflows/protocol.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/resource.py` & `hera-5.3.0/src/hera/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/resources.py` & `hera-5.3.0/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/retry_strategy.py` & `hera-5.3.0/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/runner.py` & `hera-5.3.0/src/hera/workflows/runner.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/script.py` & `hera-5.3.0/src/hera/workflows/script.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,28 @@
 """
 
 import copy
 import inspect
 import textwrap
 from abc import abstractmethod
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Type, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+)
 
 from pydantic import root_validator, validator
+from typing_extensions import ParamSpec
 
 from hera.expr import g
 from hera.shared import BaseMixin, global_config
 from hera.workflows._context import _context
 from hera.workflows._mixins import (
     CallableTemplateMixin,
     ContainerMixin,
@@ -224,14 +235,50 @@
             source_signature[p.name] = MISSING
 
     if len(source_signature) == 0:
         return None
     return [Parameter(name=n, default=v) for n, v in source_signature.items()]
 
 
+FuncIns = ParamSpec("FuncIns")  # For input types of given func to script decorator
+FuncR = TypeVar("FuncR")  # For return type of given func to script decorator
+ScriptIns = ParamSpec("ScriptIns")  # For attribute types of Script
+
+
+def _take_annotation_from(
+    _: Callable[
+        ScriptIns,
+        Callable[[Callable[FuncIns, FuncR]], Union[Callable[FuncIns, FuncR], Callable[ScriptIns, Union[Task, Step]]]],
+    ]
+) -> Callable[
+    [Callable],
+    Callable[
+        ScriptIns,
+        Callable[[Callable[FuncIns, FuncR]], Union[Callable[FuncIns, FuncR], Callable[ScriptIns, Union[Task, Step]]]],
+    ],
+]:
+    def decorator(
+        real_function: Callable,
+    ) -> Callable[
+        ScriptIns,
+        Callable[[Callable[FuncIns, FuncR]], Union[Callable[FuncIns, FuncR], Callable[ScriptIns, Union[Task, Step]]]],
+    ]:
+        def new_function(
+            *args: ScriptIns.args, **kwargs: ScriptIns.kwargs
+        ) -> Callable[
+            [Callable[FuncIns, FuncR]], Union[Callable[FuncIns, FuncR], Callable[ScriptIns, Union[Task, Step]]]
+        ]:
+            return real_function(*args, **kwargs)
+
+        return new_function
+
+    return decorator
+
+
+@_take_annotation_from(Script)  # type: ignore
 def script(**script_kwargs):
     """A decorator that wraps a function into a Script object.
 
     Using this decorator users can define a function that will be executed as a script in a container. Once the
     `Script` is returned users can use it as they generally use a `Script` e.g. as a callable inside a DAG or Steps.
     Note that invoking the function will result in the template associated with the script to be added to the
     workflow context, so users do not have to worry about that.
@@ -243,34 +290,45 @@
 
     Returns
     -------
     Callable
         Function that wraps a given function into a `Script`.
     """
 
-    def script_wrapper(func: Callable) -> Callable:
+    def script_wrapper(
+        func: Callable[FuncIns, FuncR],
+    ) -> Union[Callable[FuncIns, FuncR], Callable[ScriptIns, Union[Task, Step]]]:
         """Wraps the given callable into a `Script` object that can be invoked.
 
         Parameters
         ----------
         func: Callable
             Function to wrap.
 
         Returns
         -------
         Callable
-            Another callable that represents the `Script` object `__call__` method.
+            Another callable that represents the `Script` object `__call__` method when in a Steps or DAG context,
+            otherwise return the callable function unchanged.
         """
         s = Script(name=func.__name__.replace("_", "-"), source=func, **script_kwargs)
 
+        @overload
+        def task_wrapper(*args: FuncIns.args, **kwargs: FuncIns.kwargs) -> FuncR:
+            ...
+
+        @overload
+        def task_wrapper(*args: ScriptIns.args, **kwargs: ScriptIns.kwargs) -> Union[Step, Task]:
+            ...
+
         @wraps(func)
-        def task_wrapper(*args, **kwargs) -> Union[Task, Step]:
+        def task_wrapper(*args, **kwargs):
             """Invokes a `Script` object's `__call__` method using the given `task_params`"""
             if _context.active:
-                return s.__call__(*args, **kwargs)  # type: ignore
+                return s.__call__(*args, **kwargs)
             return func(*args, **kwargs)
 
         # Set the wrapped function to the original function so that we can use it later
         task_wrapper.wrapped_function = func  # type: ignore
         return task_wrapper
 
     return script_wrapper
```

### Comparing `hera-5.2.1/src/hera/workflows/suspend.py` & `hera-5.3.0/src/hera/workflows/suspend.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/task.py` & `hera-5.3.0/src/hera/workflows/task.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     TemplateMixin,
 )
 from hera.workflows.models import (
     DAGTask as _ModelDAGTask,
     Template,
 )
 from hera.workflows.operator import Operator
-from hera.workflows.parameter import Parameter
 from hera.workflows.protocol import Templatable
 from hera.workflows.workflow_status import WorkflowStatus
 
 
 class TaskResult(Enum):
     """The enumeration of Task Results specified at
     https://argoproj.github.io/argo-workflows/enhanced-depends-logic/#depends
@@ -115,81 +114,16 @@
         tasks = [t for t in self.depends.split() if t not in all_operators]
 
         # remove dot suffixes
         task_names = [t.split(".")[0] for t in tasks]
         return task_names
 
     @property
-    def id(self) -> str:
-        return f"{{{{tasks.{self.name}.id}}}}"
-
-    @property
-    def ip(self) -> str:
-        return f"{{{{tasks.{self.name}.ip}}}}"
-
-    @property
-    def status(self) -> str:
-        return f"{{{{tasks.{self.name}.status}}}}"
-
-    @property
-    def exit_code(self) -> str:
-        return f"{{{{tasks.{self.name}.exitCode}}}}"
-
-    @property
-    def started_at(self) -> str:
-        return f"{{{{tasks.{self.name}.startedAt}}}}"
-
-    @property
-    def finished_at(self) -> str:
-        return f"{{{{tasks.{self.name}.finishedAt}}}}"
-
-    @property
-    def result(self) -> str:
-        return f"{{{{tasks.{self.name}.outputs.result}}}}"
-
-    def get_parameters_as(self, name: str) -> Parameter:
-        """Gets all the output parameters from this task"""
-        return Parameter(name=name, value=f"{{{{tasks.{self.name}.outputs.parameters}}}}")
-
-    def get_parameter(self, name: str) -> Parameter:
-        """Returns a Parameter from the task's outputs based on the name.
-
-        Parameters
-        ----------
-        name: str
-            The name of the parameter to extract as an output.
-
-        Returns
-        -------
-        Parameter
-            Parameter with the same name
-        """
-        if isinstance(self.template, str):
-            raise ValueError(f"Cannot get output parameters when the template was set via a name: {self.template}")
-
-        # here, we build the template early to verify that we can get the outputs
-        if isinstance(self.template, Templatable):
-            template = self.template._build_template()
-        else:
-            template = self.template
-
-        # at this point, we know that the template is a `Template` object
-        if template.outputs is None:  # type: ignore
-            raise ValueError(f"Cannot get output parameters when the template has no outputs: {template}")
-        if template.outputs.parameters is None:  # type: ignore
-            raise ValueError(f"Cannot get output parameters when the template has no output parameters: {template}")
-        parameters = template.outputs.parameters  # type: ignore
-
-        obj = next((output for output in parameters if output.name == name), None)
-        if obj is not None:
-            return Parameter(
-                name=obj.name,
-                value=f"{{{{tasks.{self.name}.outputs.parameters.{name}}}}}",
-            )
-        raise KeyError(f"No output parameter named `{name}` found")
+    def _subtype(self) -> str:
+        return "tasks"
 
     def next(self, other: Task, operator: Operator = Operator.and_, on: Optional[TaskResult] = None) -> Task:
         """Set self as a dependency of `other`."""
         assert issubclass(other.__class__, Task)
 
         condition = f".{on.value}" if on else ""
```

### Comparing `hera-5.2.1/src/hera/workflows/user_container.py` & `hera-5.3.0/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/validators.py` & `hera-5.3.0/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/volume.py` & `hera-5.3.0/src/hera/workflows/volume.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/workflow_status.py` & `hera-5.3.0/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera-5.2.1/src/hera/workflows/workflow_template.py` & `hera-5.3.0/src/hera/workflows/workflow_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """The workflow_template module provides the WorkflowTemplate class
 
 See https://argoproj.github.io/argo-workflows/workflow-templates/
 for more on WorkflowTemplates.
 """
 from pydantic import validator
 
+from hera.exceptions import NotFound
 from hera.workflows.models import (
     ObjectMeta,
     WorkflowSpec as _ModelWorkflowSpec,
     WorkflowTemplate as _ModelWorkflowTemplate,
     WorkflowTemplateCreateRequest,
     WorkflowTemplateLintRequest,
+    WorkflowTemplateUpdateRequest,
 )
 from hera.workflows.protocol import TWorkflow
 from hera.workflows.workflow import Workflow
 
 
 class WorkflowTemplate(Workflow):
     """WorkflowTemplates are definitions of Workflows that live in your cluster. This allows you
@@ -25,22 +27,54 @@
     # WorkflowTemplate fields match Workflow exactly except for `status`, which WorkflowTemplate
     # does not have - https://argoproj.github.io/argo-workflows/fields/#workflowtemplate
     @validator("status", pre=True, always=True)
     def _set_status(cls, v):
         if v is not None:
             raise ValueError("status is not a valid field on a WorkflowTemplate")
 
-    def create(self) -> TWorkflow:
+    def create(self) -> TWorkflow:  # type: ignore
         """Creates the WorkflowTemplate on the Argo cluster."""
         assert self.workflows_service, "workflow service not initialized"
         assert self.namespace, "workflow namespace not defined"
         return self.workflows_service.create_workflow_template(
             WorkflowTemplateCreateRequest(template=self.build()), namespace=self.namespace
         )
 
+    def get(self) -> TWorkflow:
+        """Attempts to get a workflow template based on the parameters of this template e.g. name + namespace"""
+        assert self.workflows_service, "workflow service not initialized"
+        assert self.namespace, "workflow namespace not defined"
+        assert self.name, "workflow name not defined"
+        return self.workflows_service.get_workflow_template(name=self.name, namespace=self.namespace)
+
+    def update(self) -> TWorkflow:
+        """
+        Attempts to perform a workflow template update based on the parameters of this template
+        e.g. name, namespace. Note that this creates the template if it does not exist. In addition, this performs
+        a get prior to updating to get the resource version to update in the first place. If you know the template
+        does not exist ahead of time, it is more efficient to use `create()` directly to avoid one round trip.
+        """
+        assert self.workflows_service, "workflow service not initialized"
+        assert self.namespace, "workflow namespace not defined"
+        assert self.name, "workflow name not defined"
+        # we always need to do a get prior to updating to get the resource version to update in the first place
+        # https://github.com/argoproj/argo-workflows/pull/5465#discussion_r597797052
+
+        template = self.build()
+        try:
+            curr = self.get()
+            template.metadata.resource_version = curr.metadata.resource_version
+        except NotFound:
+            return self.create()
+        return self.workflows_service.update_workflow_template(
+            self.name,
+            WorkflowTemplateUpdateRequest(template=template),
+            namespace=self.namespace,
+        )
+
     def lint(self) -> TWorkflow:
         """Lints the WorkflowTemplate using the Argo cluster."""
         assert self.workflows_service, "workflow service not initialized"
         assert self.namespace, "workflow namespace not defined"
         return self.workflows_service.lint_workflow_template(
             WorkflowTemplateLintRequest(template=self.build()), namespace=self.namespace
         )
```

### Comparing `hera-5.2.1/PKG-INFO` & `hera-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera
-Version: 5.2.1
+Version: 5.3.0
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
```


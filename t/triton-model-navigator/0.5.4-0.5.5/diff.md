# Comparing `tmp/triton_model_navigator-0.5.4-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.5.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,134 +1,135 @@
-Zip file size: 232590 bytes, number of entries: 132
--rw-r--r--  2.0 unx      881 b- defN 23-May-18 03:12 model_navigator/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-May-18 03:12 model_navigator/__version__.py
--rw-r--r--  2.0 unx     3668 b- defN 23-May-18 03:12 model_navigator/exceptions.py
--rw-r--r--  2.0 unx     9474 b- defN 23-May-18 03:12 model_navigator/execution_context.py
--rw-r--r--  2.0 unx     4790 b- defN 23-May-18 03:12 model_navigator/logger.py
--rw-r--r--  2.0 unx     1678 b- defN 23-May-18 03:12 model_navigator/api/__init__.py
--rw-r--r--  2.0 unx    23210 b- defN 23-May-18 03:12 model_navigator/api/config.py
--rw-r--r--  2.0 unx     6425 b- defN 23-May-18 03:12 model_navigator/api/jax.py
--rw-r--r--  2.0 unx     5423 b- defN 23-May-18 03:12 model_navigator/api/onnx.py
--rw-r--r--  2.0 unx    11860 b- defN 23-May-18 03:12 model_navigator/api/package.py
--rw-r--r--  2.0 unx     4906 b- defN 23-May-18 03:12 model_navigator/api/python.py
--rw-r--r--  2.0 unx     7748 b- defN 23-May-18 03:12 model_navigator/api/pytriton.py
--rw-r--r--  2.0 unx     6519 b- defN 23-May-18 03:12 model_navigator/api/tensorflow.py
--rw-r--r--  2.0 unx     6325 b- defN 23-May-18 03:12 model_navigator/api/torch.py
--rw-r--r--  2.0 unx     1553 b- defN 23-May-18 03:12 model_navigator/api/triton.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/commands/__init__.py
--rw-r--r--  2.0 unx     4938 b- defN 23-May-18 03:12 model_navigator/commands/base.py
--rw-r--r--  2.0 unx    10065 b- defN 23-May-18 03:12 model_navigator/commands/infer_metadata.py
--rw-r--r--  2.0 unx     3289 b- defN 23-May-18 03:12 model_navigator/commands/load.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/commands/convert/__init__.py
--rw-r--r--  2.0 unx     9863 b- defN 23-May-18 03:12 model_navigator/commands/convert/base.py
--rw-r--r--  2.0 unx     7838 b- defN 23-May-18 03:12 model_navigator/commands/convert/tf.py
--rw-r--r--  2.0 unx    10224 b- defN 23-May-18 03:12 model_navigator/commands/convert/torch.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/commands/convert/converters/__init__.py
--rw-r--r--  2.0 unx     3418 b- defN 23-May-18 03:12 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-r--r--  2.0 unx     3105 b- defN 23-May-18 03:12 model_navigator/commands/convert/converters/ts2onnx.py
--rw-r--r--  2.0 unx     4992 b- defN 23-May-18 03:12 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-r--r--  2.0 unx      680 b- defN 23-May-18 03:12 model_navigator/commands/convert/onnx/__init__.py
--rw-r--r--  2.0 unx     1727 b- defN 23-May-18 03:12 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-r--r--  2.0 unx    10454 b- defN 23-May-18 03:12 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-r--r--  2.0 unx     2235 b- defN 23-May-18 03:12 model_navigator/commands/convert/onnx/trt_load_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/commands/copy/__init__.py
--rw-r--r--  2.0 unx     1729 b- defN 23-May-18 03:12 model_navigator/commands/copy/onnx.py
--rw-r--r--  2.0 unx      678 b- defN 23-May-18 03:12 model_navigator/commands/correctness/__init__.py
--rw-r--r--  2.0 unx     5594 b- defN 23-May-18 03:12 model_navigator/commands/correctness/correctness.py
--rw-r--r--  2.0 unx     4550 b- defN 23-May-18 03:12 model_navigator/commands/correctness/correctness_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/commands/data_dump/__init__.py
--rw-r--r--  2.0 unx    11162 b- defN 23-May-18 03:12 model_navigator/commands/data_dump/samples.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/commands/export/__init__.py
--rw-r--r--  2.0 unx     3531 b- defN 23-May-18 03:12 model_navigator/commands/export/jax.py
--rw-r--r--  2.0 unx     5485 b- defN 23-May-18 03:12 model_navigator/commands/export/tf.py
--rw-r--r--  2.0 unx     8894 b- defN 23-May-18 03:12 model_navigator/commands/export/torch.py
--rw-r--r--  2.0 unx     1056 b- defN 23-May-18 03:12 model_navigator/commands/export/exporters/__init__.py
--rw-r--r--  2.0 unx     3945 b- defN 23-May-18 03:12 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-r--r--  2.0 unx     3171 b- defN 23-May-18 03:12 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-r--r--  2.0 unx     3122 b- defN 23-May-18 03:12 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-r--r--  2.0 unx     3077 b- defN 23-May-18 03:12 model_navigator/commands/export/exporters/torch2onnx.py
--rw-r--r--  2.0 unx     2603 b- defN 23-May-18 03:12 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-r--r--  2.0 unx      715 b- defN 23-May-18 03:12 model_navigator/commands/find_max_batch_size/__init__.py
--rw-r--r--  2.0 unx     6396 b- defN 23-May-18 03:12 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-r--r--  2.0 unx     2984 b- defN 23-May-18 03:12 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-r--r--  2.0 unx      688 b- defN 23-May-18 03:12 model_navigator/commands/performance/__init__.py
--rw-r--r--  2.0 unx    15770 b- defN 23-May-18 03:12 model_navigator/commands/performance/performance.py
--rw-r--r--  2.0 unx     3037 b- defN 23-May-18 03:12 model_navigator/commands/performance/performance_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/commands/verification/__init__.py
--rw-r--r--  2.0 unx     5441 b- defN 23-May-18 03:12 model_navigator/commands/verification/verify.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/configuration/__init__.py
--rw-r--r--  2.0 unx     2473 b- defN 23-May-18 03:12 model_navigator/configuration/common_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/configuration/model/__init__.py
--rw-r--r--  2.0 unx    14775 b- defN 23-May-18 03:12 model_navigator/configuration/model/model_config.py
--rw-r--r--  2.0 unx    13477 b- defN 23-May-18 03:12 model_navigator/configuration/model/model_config_builder.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/core/__init__.py
--rw-r--r--  2.0 unx     1326 b- defN 23-May-18 03:12 model_navigator/core/constants.py
--rw-r--r--  2.0 unx    20111 b- defN 23-May-18 03:12 model_navigator/core/package.py
--rw-r--r--  2.0 unx    20337 b- defN 23-May-18 03:12 model_navigator/core/status.py
--rw-r--r--  2.0 unx     8052 b- defN 23-May-18 03:12 model_navigator/core/tensor.py
--rw-r--r--  2.0 unx     2817 b- defN 23-May-18 03:12 model_navigator/frameworks/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-May-18 03:12 model_navigator/frameworks/jax/__init__.py
--rw-r--r--  2.0 unx     1554 b- defN 23-May-18 03:12 model_navigator/frameworks/jax/model.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/frameworks/onnx/__init__.py
--rw-r--r--  2.0 unx     1085 b- defN 23-May-18 03:12 model_navigator/frameworks/onnx/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/frameworks/tensorrt/__init__.py
--rw-r--r--  2.0 unx    26575 b- defN 23-May-18 03:12 model_navigator/frameworks/tensorrt/cuda.py
--rw-r--r--  2.0 unx     9836 b- defN 23-May-18 03:12 model_navigator/frameworks/tensorrt/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/frameworks/torch/__init__.py
--rw-r--r--  2.0 unx     1508 b- defN 23-May-18 03:12 model_navigator/frameworks/torch/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/pipelines/__init__.py
--rw-r--r--  2.0 unx     5685 b- defN 23-May-18 03:12 model_navigator/pipelines/pipeline.py
--rw-r--r--  2.0 unx     7333 b- defN 23-May-18 03:12 model_navigator/pipelines/pipeline_manager.py
--rw-r--r--  2.0 unx     9805 b- defN 23-May-18 03:12 model_navigator/pipelines/validation.py
--rw-r--r--  2.0 unx     1879 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/__init__.py
--rw-r--r--  2.0 unx     2036 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/correctness.py
--rw-r--r--  2.0 unx     5703 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-r--r--  2.0 unx     1647 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/jax.py
--rw-r--r--  2.0 unx     2483 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/onnx.py
--rw-r--r--  2.0 unx     2365 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/preprocessing.py
--rw-r--r--  2.0 unx     2685 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/profiling.py
--rw-r--r--  2.0 unx     2869 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/tensorflow.py
--rw-r--r--  2.0 unx     3261 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/torch.py
--rw-r--r--  2.0 unx     2042 b- defN 23-May-18 03:12 model_navigator/pipelines/builders/verify.py
--rw-r--r--  2.0 unx     1584 b- defN 23-May-18 03:12 model_navigator/runners/__init__.py
--rw-r--r--  2.0 unx    11369 b- defN 23-May-18 03:12 model_navigator/runners/base.py
--rw-r--r--  2.0 unx     2620 b- defN 23-May-18 03:12 model_navigator/runners/jax.py
--rw-r--r--  2.0 unx     7302 b- defN 23-May-18 03:12 model_navigator/runners/onnx.py
--rw-r--r--  2.0 unx     2267 b- defN 23-May-18 03:12 model_navigator/runners/python.py
--rw-r--r--  2.0 unx     2285 b- defN 23-May-18 03:12 model_navigator/runners/registry.py
--rw-r--r--  2.0 unx     7976 b- defN 23-May-18 03:12 model_navigator/runners/tensorflow.py
--rw-r--r--  2.0 unx    25301 b- defN 23-May-18 03:12 model_navigator/runners/tensorrt.py
--rw-r--r--  2.0 unx     7699 b- defN 23-May-18 03:12 model_navigator/runners/torch.py
--rw-r--r--  2.0 unx     3554 b- defN 23-May-18 03:12 model_navigator/runners/utils.py
--rw-r--r--  2.0 unx      937 b- defN 23-May-18 03:12 model_navigator/runtime_analyzer/__init__.py
--rw-r--r--  2.0 unx    11706 b- defN 23-May-18 03:12 model_navigator/runtime_analyzer/analyzer.py
--rw-r--r--  2.0 unx     2304 b- defN 23-May-18 03:12 model_navigator/runtime_analyzer/strategy.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/triton/__init__.py
--rw-r--r--  2.0 unx     3180 b- defN 23-May-18 03:12 model_navigator/triton/model_config.py
--rw-r--r--  2.0 unx     5218 b- defN 23-May-18 03:12 model_navigator/triton/model_config_builder.py
--rw-r--r--  2.0 unx    23090 b- defN 23-May-18 03:12 model_navigator/triton/model_config_generator.py
--rw-r--r--  2.0 unx    15193 b- defN 23-May-18 03:12 model_navigator/triton/model_repository.py
--rw-r--r--  2.0 unx     2081 b- defN 23-May-18 03:12 model_navigator/triton/utils.py
--rw-r--r--  2.0 unx      944 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/__init__.py
--rw-r--r--  2.0 unx     2872 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/base_model_config.py
--rw-r--r--  2.0 unx    22326 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/common.py
--rw-r--r--  2.0 unx     2229 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/internal.py
--rw-r--r--  2.0 unx     2685 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-r--r--  2.0 unx     1785 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/python_model_config.py
--rw-r--r--  2.0 unx     2239 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-r--r--  2.0 unx     3162 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-r--r--  2.0 unx     3040 b- defN 23-May-18 03:12 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-18 03:12 model_navigator/utils/__init__.py
--rw-r--r--  2.0 unx    14113 b- defN 23-May-18 03:12 model_navigator/utils/common.py
--rw-r--r--  2.0 unx     7996 b- defN 23-May-18 03:12 model_navigator/utils/dataloader.py
--rw-r--r--  2.0 unx     3902 b- defN 23-May-18 03:12 model_navigator/utils/devices.py
--rw-r--r--  2.0 unx     1308 b- defN 23-May-18 03:12 model_navigator/utils/enums.py
--rw-r--r--  2.0 unx     6163 b- defN 23-May-18 03:12 model_navigator/utils/environment.py
--rw-r--r--  2.0 unx     3528 b- defN 23-May-18 03:12 model_navigator/utils/format_helpers.py
--rw-r--r--  2.0 unx     2325 b- defN 23-May-18 03:12 model_navigator/utils/module.py
--rw-r--r--  2.0 unx     3233 b- defN 23-May-18 03:12 model_navigator/utils/package.py
--rw-r--r--  2.0 unx    10140 b- defN 23-May-18 07:14 triton_model_navigator-0.5.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    12074 b- defN 23-May-18 07:14 triton_model_navigator-0.5.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 07:14 triton_model_navigator-0.5.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-18 07:14 triton_model_navigator-0.5.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    13183 b- defN 23-May-18 07:14 triton_model_navigator-0.5.4.dist-info/RECORD
-132 files, 701006 bytes uncompressed, 211094 bytes compressed:  69.9%
+Zip file size: 234334 bytes, number of entries: 133
+-rw-r--r--  2.0 unx      881 b- defN 23-May-24 10:59 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-May-24 10:59 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     3668 b- defN 23-May-24 10:59 model_navigator/exceptions.py
+-rw-r--r--  2.0 unx     9474 b- defN 23-May-24 10:59 model_navigator/execution_context.py
+-rw-r--r--  2.0 unx     4790 b- defN 23-May-24 10:59 model_navigator/logger.py
+-rw-rw-rw-  2.0 unx     1716 b- defN 23-May-24 10:59 model_navigator/api/__init__.py
+-rw-rw-rw-  2.0 unx    24304 b- defN 23-May-24 10:59 model_navigator/api/config.py
+-rw-rw-rw-  2.0 unx     6425 b- defN 23-May-24 10:59 model_navigator/api/jax.py
+-rw-rw-rw-  2.0 unx     5423 b- defN 23-May-24 10:59 model_navigator/api/onnx.py
+-rw-rw-rw-  2.0 unx    11860 b- defN 23-May-24 10:59 model_navigator/api/package.py
+-rw-rw-rw-  2.0 unx     4906 b- defN 23-May-24 10:59 model_navigator/api/python.py
+-rw-rw-rw-  2.0 unx     7748 b- defN 23-May-24 10:59 model_navigator/api/pytriton.py
+-rw-rw-rw-  2.0 unx     6519 b- defN 23-May-24 10:59 model_navigator/api/tensorflow.py
+-rw-rw-rw-  2.0 unx     6325 b- defN 23-May-24 10:59 model_navigator/api/torch.py
+-rw-rw-rw-  2.0 unx     1553 b- defN 23-May-24 10:59 model_navigator/api/triton.py
+-rw-rw-rw-  2.0 unx     1811 b- defN 23-May-24 10:59 model_navigator/api/utilities.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/__init__.py
+-rw-rw-rw-  2.0 unx     4938 b- defN 23-May-24 10:59 model_navigator/commands/base.py
+-rw-rw-rw-  2.0 unx    10065 b- defN 23-May-24 10:59 model_navigator/commands/infer_metadata.py
+-rw-rw-rw-  2.0 unx     3289 b- defN 23-May-24 10:59 model_navigator/commands/load.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/convert/__init__.py
+-rw-rw-rw-  2.0 unx     9863 b- defN 23-May-24 10:59 model_navigator/commands/convert/base.py
+-rw-rw-rw-  2.0 unx     7838 b- defN 23-May-24 10:59 model_navigator/commands/convert/tf.py
+-rw-rw-rw-  2.0 unx    10224 b- defN 23-May-24 10:59 model_navigator/commands/convert/torch.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/convert/converters/__init__.py
+-rw-rw-rw-  2.0 unx     3418 b- defN 23-May-24 10:59 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-rw-rw-  2.0 unx     3105 b- defN 23-May-24 10:59 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-rw-rw-  2.0 unx     4992 b- defN 23-May-24 10:59 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-rw-rw-  2.0 unx      680 b- defN 23-May-24 10:59 model_navigator/commands/convert/onnx/__init__.py
+-rw-rw-rw-  2.0 unx     1727 b- defN 23-May-24 10:59 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-rw-rw-  2.0 unx    10818 b- defN 23-May-24 10:59 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-rw-rw-  2.0 unx     2235 b- defN 23-May-24 10:59 model_navigator/commands/convert/onnx/trt_load_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/copy/__init__.py
+-rw-rw-rw-  2.0 unx     1729 b- defN 23-May-24 10:59 model_navigator/commands/copy/onnx.py
+-rw-rw-rw-  2.0 unx      678 b- defN 23-May-24 10:59 model_navigator/commands/correctness/__init__.py
+-rw-rw-rw-  2.0 unx     5594 b- defN 23-May-24 10:59 model_navigator/commands/correctness/correctness.py
+-rw-rw-rw-  2.0 unx     4550 b- defN 23-May-24 10:59 model_navigator/commands/correctness/correctness_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/data_dump/__init__.py
+-rw-rw-rw-  2.0 unx    11162 b- defN 23-May-24 10:59 model_navigator/commands/data_dump/samples.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/export/__init__.py
+-rw-rw-rw-  2.0 unx     3531 b- defN 23-May-24 10:59 model_navigator/commands/export/jax.py
+-rw-rw-rw-  2.0 unx     5485 b- defN 23-May-24 10:59 model_navigator/commands/export/tf.py
+-rw-rw-rw-  2.0 unx     9043 b- defN 23-May-24 10:59 model_navigator/commands/export/torch.py
+-rw-rw-rw-  2.0 unx     1056 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/__init__.py
+-rw-rw-rw-  2.0 unx     3945 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-rw-rw-  2.0 unx     3171 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-rw-rw-  2.0 unx     3122 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-rw-rw-  2.0 unx     3077 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-rw-rw-  2.0 unx     2728 b- defN 23-May-24 10:59 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-rw-rw-  2.0 unx      715 b- defN 23-May-24 10:59 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-rw-rw-  2.0 unx     6396 b- defN 23-May-24 10:59 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-rw-rw-  2.0 unx     2984 b- defN 23-May-24 10:59 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-rw-rw-  2.0 unx      688 b- defN 23-May-24 10:59 model_navigator/commands/performance/__init__.py
+-rw-rw-rw-  2.0 unx    15770 b- defN 23-May-24 10:59 model_navigator/commands/performance/performance.py
+-rw-rw-rw-  2.0 unx     3037 b- defN 23-May-24 10:59 model_navigator/commands/performance/performance_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/commands/verification/__init__.py
+-rw-rw-rw-  2.0 unx     5441 b- defN 23-May-24 10:59 model_navigator/commands/verification/verify.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/configuration/__init__.py
+-rw-rw-rw-  2.0 unx     2473 b- defN 23-May-24 10:59 model_navigator/configuration/common_config.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/configuration/model/__init__.py
+-rw-rw-rw-  2.0 unx    15623 b- defN 23-May-24 10:59 model_navigator/configuration/model/model_config.py
+-rw-rw-rw-  2.0 unx    13677 b- defN 23-May-24 10:59 model_navigator/configuration/model/model_config_builder.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/core/__init__.py
+-rw-rw-rw-  2.0 unx     1326 b- defN 23-May-24 10:59 model_navigator/core/constants.py
+-rw-rw-rw-  2.0 unx    20111 b- defN 23-May-24 10:59 model_navigator/core/package.py
+-rw-rw-rw-  2.0 unx    20337 b- defN 23-May-24 10:59 model_navigator/core/status.py
+-rw-rw-rw-  2.0 unx     8052 b- defN 23-May-24 10:59 model_navigator/core/tensor.py
+-rw-rw-rw-  2.0 unx     2817 b- defN 23-May-24 10:59 model_navigator/frameworks/__init__.py
+-rw-rw-rw-  2.0 unx      669 b- defN 23-May-24 10:59 model_navigator/frameworks/jax/__init__.py
+-rw-rw-rw-  2.0 unx     1554 b- defN 23-May-24 10:59 model_navigator/frameworks/jax/model.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/frameworks/onnx/__init__.py
+-rw-rw-rw-  2.0 unx     1085 b- defN 23-May-24 10:59 model_navigator/frameworks/onnx/utils.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/frameworks/tensorrt/__init__.py
+-rw-rw-rw-  2.0 unx    26575 b- defN 23-May-24 10:59 model_navigator/frameworks/tensorrt/cuda.py
+-rw-rw-rw-  2.0 unx     9874 b- defN 23-May-24 10:59 model_navigator/frameworks/tensorrt/utils.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/frameworks/torch/__init__.py
+-rw-rw-rw-  2.0 unx     1508 b- defN 23-May-24 10:59 model_navigator/frameworks/torch/utils.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/pipelines/__init__.py
+-rw-rw-rw-  2.0 unx     5685 b- defN 23-May-24 10:59 model_navigator/pipelines/pipeline.py
+-rw-rw-rw-  2.0 unx     7333 b- defN 23-May-24 10:59 model_navigator/pipelines/pipeline_manager.py
+-rw-rw-rw-  2.0 unx     9805 b- defN 23-May-24 10:59 model_navigator/pipelines/validation.py
+-rw-rw-rw-  2.0 unx     1879 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/__init__.py
+-rw-rw-rw-  2.0 unx     2036 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/correctness.py
+-rw-rw-rw-  2.0 unx     5703 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-rw-rw-  2.0 unx     1647 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/jax.py
+-rw-rw-rw-  2.0 unx     2483 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/onnx.py
+-rw-rw-rw-  2.0 unx     2365 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/preprocessing.py
+-rw-rw-rw-  2.0 unx     2685 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/profiling.py
+-rw-rw-rw-  2.0 unx     2869 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/tensorflow.py
+-rw-rw-rw-  2.0 unx     3261 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/torch.py
+-rw-rw-rw-  2.0 unx     2042 b- defN 23-May-24 10:59 model_navigator/pipelines/builders/verify.py
+-rw-rw-rw-  2.0 unx     1584 b- defN 23-May-24 10:59 model_navigator/runners/__init__.py
+-rw-rw-rw-  2.0 unx    11369 b- defN 23-May-24 10:59 model_navigator/runners/base.py
+-rw-rw-rw-  2.0 unx     2620 b- defN 23-May-24 10:59 model_navigator/runners/jax.py
+-rw-rw-rw-  2.0 unx     7302 b- defN 23-May-24 10:59 model_navigator/runners/onnx.py
+-rw-rw-rw-  2.0 unx     2267 b- defN 23-May-24 10:59 model_navigator/runners/python.py
+-rw-rw-rw-  2.0 unx     2285 b- defN 23-May-24 10:59 model_navigator/runners/registry.py
+-rw-rw-rw-  2.0 unx     7976 b- defN 23-May-24 10:59 model_navigator/runners/tensorflow.py
+-rw-rw-rw-  2.0 unx    25301 b- defN 23-May-24 10:59 model_navigator/runners/tensorrt.py
+-rw-rw-rw-  2.0 unx     7699 b- defN 23-May-24 10:59 model_navigator/runners/torch.py
+-rw-rw-rw-  2.0 unx     3554 b- defN 23-May-24 10:59 model_navigator/runners/utils.py
+-rw-rw-rw-  2.0 unx      937 b- defN 23-May-24 10:59 model_navigator/runtime_analyzer/__init__.py
+-rw-rw-rw-  2.0 unx    11706 b- defN 23-May-24 10:59 model_navigator/runtime_analyzer/analyzer.py
+-rw-rw-rw-  2.0 unx     2304 b- defN 23-May-24 10:59 model_navigator/runtime_analyzer/strategy.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/triton/__init__.py
+-rw-rw-rw-  2.0 unx     3180 b- defN 23-May-24 10:59 model_navigator/triton/model_config.py
+-rw-rw-rw-  2.0 unx     5218 b- defN 23-May-24 10:59 model_navigator/triton/model_config_builder.py
+-rw-rw-rw-  2.0 unx    23090 b- defN 23-May-24 10:59 model_navigator/triton/model_config_generator.py
+-rw-rw-rw-  2.0 unx    15193 b- defN 23-May-24 10:59 model_navigator/triton/model_repository.py
+-rw-rw-rw-  2.0 unx     2081 b- defN 23-May-24 10:59 model_navigator/triton/utils.py
+-rw-rw-rw-  2.0 unx      944 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/__init__.py
+-rw-rw-rw-  2.0 unx     2872 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-rw-rw-  2.0 unx    22326 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/common.py
+-rw-rw-rw-  2.0 unx     2229 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/internal.py
+-rw-rw-rw-  2.0 unx     2685 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-rw-rw-  2.0 unx     1785 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-rw-rw-  2.0 unx     2239 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-rw-rw-  2.0 unx     3162 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-rw-rw-  2.0 unx     3040 b- defN 23-May-24 10:59 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-May-24 10:59 model_navigator/utils/__init__.py
+-rw-rw-rw-  2.0 unx    14113 b- defN 23-May-24 10:59 model_navigator/utils/common.py
+-rw-rw-rw-  2.0 unx     7996 b- defN 23-May-24 10:59 model_navigator/utils/dataloader.py
+-rw-rw-rw-  2.0 unx     3902 b- defN 23-May-24 10:59 model_navigator/utils/devices.py
+-rw-rw-rw-  2.0 unx     1308 b- defN 23-May-24 10:59 model_navigator/utils/enums.py
+-rw-rw-rw-  2.0 unx     6163 b- defN 23-May-24 10:59 model_navigator/utils/environment.py
+-rw-rw-rw-  2.0 unx     3528 b- defN 23-May-24 10:59 model_navigator/utils/format_helpers.py
+-rw-rw-rw-  2.0 unx     2325 b- defN 23-May-24 10:59 model_navigator/utils/module.py
+-rw-rw-rw-  2.0 unx     3233 b- defN 23-May-24 10:59 model_navigator/utils/package.py
+-rw-rw-rw-  2.0 unx    10140 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12074 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    13272 b- defN 23-May-24 11:56 triton_model_navigator-0.5.5.dist-info/RECORD
+133 files, 705762 bytes uncompressed, 212698 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -39,14 +39,17 @@
 
 Filename: model_navigator/api/torch.py
 Comment: 
 
 Filename: model_navigator/api/triton.py
 Comment: 
 
+Filename: model_navigator/api/utilities.py
+Comment: 
+
 Filename: model_navigator/commands/__init__.py
 Comment: 
 
 Filename: model_navigator/commands/base.py
 Comment: 
 
 Filename: model_navigator/commands/infer_metadata.py
@@ -375,23 +378,23 @@
 
 Filename: model_navigator/utils/module.py
 Comment: 
 
 Filename: model_navigator/utils/package.py
 Comment: 
 
-Filename: triton_model_navigator-0.5.4.dist-info/LICENSE
+Filename: triton_model_navigator-0.5.5.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.5.4.dist-info/METADATA
+Filename: triton_model_navigator-0.5.5.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.5.4.dist-info/WHEEL
+Filename: triton_model_navigator-0.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.5.4.dist-info/top_level.txt
+Filename: triton_model_navigator-0.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.5.4.dist-info/RECORD
+Filename: triton_model_navigator-0.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_navigator/__version__.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D100
-__version__ = "0.5.4"
+__version__ = "0.5.5"
```

## model_navigator/api/__init__.py

```diff
@@ -47,7 +47,8 @@
     from . import jax  # noqa: F401
 
 from . import onnx  # noqa: F401
 from . import package  # noqa: F401
 from . import python  # noqa: F401
 from . import pytriton  # noqa: F401
 from . import triton  # noqa: F401
+from . import utilities  # noqa: F401
```

## model_navigator/api/config.py

```diff
@@ -36,14 +36,15 @@
 
 from model_navigator.core.constants import (
     DEFAULT_MAX_WORKSPACE_SIZE,
     DEFAULT_MIN_SEGMENT_SIZE,
     DEFAULT_ONNX_OPSET,
     DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD,
 )
+from model_navigator.exceptions import ModelNavigatorConfigurationError
 from model_navigator.frameworks import Framework
 from model_navigator.logger import LOGGER
 from model_navigator.utils.common import DataObject
 
 Sample = Dict[str, numpy.ndarray]
 
 VerifyFunction = Callable[[Iterable[Sample], Iterable[Sample]], bool]
@@ -151,14 +152,24 @@
     """
 
     HIERARCHY = "hierarchy"
     SINGLE = "single"
     MIXED = "mixed"
 
 
+class TensorRTCompatibilityLevel(Enum):
+    """Compatibility level for TensorRT.
+
+    Args:
+        AMPERE_PLUS (str): Support AMPERE plus architecture
+    """
+
+    AMPERE_PLUS = "ampere_plus"
+
+
 @dataclass
 class ShapeTuple(DataObject):
     """Represents a set of shapes for a single binding in a profile.
 
     Each element of the tuple represents a shape for a single dimension of the binding.
 
     Args:
@@ -532,18 +543,20 @@
 
 @dataclass
 class TorchConfig(CustomConfigForFormat):
     """Torch custom config used for TorchScript export.
 
     Args:
         jit_type: Type of TorchScript export.
+        strict: Enable or Disable strict flag for tracer used in TorchScript export, default: True.
 
     """
 
     jit_type: Union[Union[str, JitType], Tuple[Union[str, JitType], ...]] = (JitType.SCRIPT, JitType.TRACE)
+    strict: bool = True
 
     def __post_init__(self) -> None:
         """Parse dataclass enums."""
         jit_type = (self.jit_type,) if not isinstance(self.jit_type, (list, tuple)) else self.jit_type
         self.jit_type = tuple(JitType(j) for j in jit_type)
 
     @property
@@ -559,14 +572,15 @@
     def name(cls) -> str:
         """Name of the config."""
         return "Torch"
 
     def defaults(self) -> None:
         """Update parameters to defaults."""
         self.jit_type = (JitType.SCRIPT, JitType.TRACE)
+        self.strict = True
 
 
 @dataclass
 class TorchTensorRTConfig(CustomConfigForFormat):
     """Torch custom config used for TensorRT TorchScript conversion.
 
     Args:
@@ -651,30 +665,38 @@
 class TensorRTConfig(CustomConfigForFormat):
     """TensorRT custom config used for TensorRT conversion.
 
     Args:
         precision: TensorRT precision.
         max_workspace_size: Max workspace size used by converter.
         trt_profile: TensorRT profile.
-
+        optimization_level: Optimization level for TensorRT conversion. Allowed values are fom 0 to 5. Where default is
+                            3 based on TensorRT API documentation.
     """
 
     precision: Union[
         Union[str, TensorRTPrecision], Tuple[Union[str, TensorRTPrecision], ...]
     ] = DEFAULT_TENSORRT_PRECISION
     precision_mode: Union[str, TensorRTPrecisionMode] = TensorRTPrecisionMode.HIERARCHY
     trt_profile: Optional[TensorRTProfile] = None
     max_workspace_size: Optional[int] = DEFAULT_MAX_WORKSPACE_SIZE
+    optimization_level: Optional[int] = None
+    compatibility_level: Optional[TensorRTCompatibilityLevel] = None
 
     def __post_init__(self) -> None:
         """Parse dataclass enums."""
         self.precision_mode = TensorRTPrecisionMode(self.precision_mode)
         precision = (self.precision,) if not isinstance(self.precision, (list, tuple)) else self.precision
         self.precision = tuple(TensorRTPrecision(p) for p in precision)
 
+        if self.optimization_level is not None and (self.optimization_level < 0 or self.optimization_level > 5):
+            raise ModelNavigatorConfigurationError(
+                f"TensorRT `optimization_level` must be between 0 and 5. Provided value: {self.optimization_level}."
+            )
+
     @property
     def format(self) -> Format:
         """Returns Format.TENSORRT.
 
         Returns:
             Format.TENSORRT
         """
@@ -687,14 +709,16 @@
 
     def defaults(self) -> None:
         """Update parameters to defaults."""
         self.precision = tuple(TensorRTPrecision(p) for p in DEFAULT_TENSORRT_PRECISION)
         self.precision_mode = DEFAULT_TENSORRT_PRECISION_MODE
         self.trt_profile = None
         self.max_workspace_size = DEFAULT_MAX_WORKSPACE_SIZE
+        self.optimization_level = None
+        self.compatibility_level = None
 
     @classmethod
     def from_dict(cls, config_dict: Dict[str, Any]) -> "TensorRTConfig":
         """Instantiate TensorRTConfig from  adictionary."""
         if config_dict.get("trt_profile") is not None and not isinstance(config_dict["trt_profile"], TensorRTProfile):
             config_dict["trt_profile"] = TensorRTProfile.from_dict(config_dict["trt_profile"])
         return cls(**config_dict)
```

## model_navigator/commands/convert/onnx/onnx2trt.py

```diff
@@ -16,15 +16,20 @@
 import pathlib
 import sys
 import tempfile
 from distutils.version import LooseVersion
 from pathlib import Path
 from typing import Optional
 
-from model_navigator.api.config import TensorRTPrecision, TensorRTPrecisionMode, TensorRTProfile
+from model_navigator.api.config import (
+    TensorRTCompatibilityLevel,
+    TensorRTPrecision,
+    TensorRTPrecisionMode,
+    TensorRTProfile,
+)
 from model_navigator.commands.base import CommandOutput, CommandStatus
 from model_navigator.commands.convert.base import Convert2TensorRTWithMaxBatchSizeSearch
 from model_navigator.core.tensor import TensorMetadata
 from model_navigator.execution_context import ExecutionContext
 from model_navigator.frameworks.tensorrt import utils as tensorrt_utils
 from model_navigator.logger import LOGGER
 from model_navigator.runners.tensorrt import TensorRTRunner
@@ -46,34 +51,38 @@
         precision_mode: TensorRTPrecisionMode,
         dataloader_trt_profile: TensorRTProfile,
         max_workspace_size: Optional[int] = None,
         batch_dim: Optional[int] = None,
         dataloader_max_batch_size: Optional[int] = None,
         device_max_batch_size: Optional[int] = None,
         trt_profile: Optional[TensorRTProfile] = None,
+        optimization_level: Optional[int] = None,
+        compatibility_level: Optional[TensorRTCompatibilityLevel] = None,
         verbose: bool = False,
     ) -> CommandOutput:
         """Run the ConvertONNX2TRT Command.
 
         Args:
-            workspace (Path): Model Navigator working directory.
-            path (Path): ONNX checkpoint path, relative to workspace.
-            parent_path (Path): Path of ONNX parent model, relative to workspace.
-            input_metadata (TensorMetadata): Model input metadata.
-            output_metadata (TensorMetadata): Model output metadata.
-            precision (TensorRTPrecision): TensoRT precision.
-            precision_mode (TensorRTPrecisionMode): TensorRT precision mode.
-            dataloader_trt_profile (TensorRTProfile): Dataloader TensorRT profile.
-            max_workspace_size (Optional[int], optional): Maximum TensoRT workspace size, in bytes. Defaults to None.
-            batch_dim (Optional[int], optional): Dimension of the batching, None if model does not support batching.
+            workspace: Model Navigator working directory.
+            path: ONNX checkpoint path, relative to workspace.
+            parent_path: Path of ONNX parent model, relative to workspace.
+            input_metadata: Model input metadata.
+            output_metadata: Model output metadata.
+            precision: TensorRT precision.
+            precision_mode: TensorRT precision mode.
+            dataloader_trt_profile: Dataloader TensorRT profile.
+            max_workspace_size: Maximum TensorRT workspace size, in bytes. Defaults to None.
+            batch_dim: Dimension of the batching, None if model does not support batching.
                 Defaults to None.
             dataloader_max_batch_size (Optional[int], optional): Maximum batch size in the dataloader. Defaults to None.
-            device_max_batch_size (Optional[int], optional): Maximum batch size that fits on the device.
+            device_max_batch_size: Maximum batch size that fits on the device.
                 Defaults to None.
-            trt_profile (Optional[TensorRTProfile], optional): User specified TensorRT profile. Defaults to None.
+            trt_profile: User specified TensorRT profile. Defaults to None.
+            optimization_level: Optimization level for TensorRT engine
+            compatibility_level: Hardware compatibility level for generated engine
             verbose: enable verbose logging for command
 
         Returns:
             CommandOutput: Status and results of the command.
         """
         LOGGER.info("ONNX to TRT conversion started")
         if not devices.get_available_gpus():
@@ -104,14 +113,20 @@
             verbose=verbose,
         )
 
         convert_cmd = ["polygraphy", "convert", input_model_path.relative_to(workspace).as_posix()]
         convert_cmd.extend(["--convert-to", "trt"])
         convert_cmd.extend(["-o", converted_model_path.relative_to(workspace).as_posix()])
 
+        if optimization_level is not None:
+            convert_cmd.extend(["--builder-optimization-level", optimization_level])
+
+        if compatibility_level is not None:
+            convert_cmd.extend(["--hardware-compatibility-level", compatibility_level.value])
+
         if precision_mode == TensorRTPrecisionMode.HIERARCHY:
             trt_precision_flags = {
                 TensorRTPrecision.FP32: ["--tf32"],
                 TensorRTPrecision.FP16: ["--tf32", "--fp16"],
                 TensorRTPrecision.INT8: ["--tf32", "--fp16", "--int8"],
             }[precision]
         elif precision_mode == TensorRTPrecisionMode.SINGLE:
```

## model_navigator/commands/export/torch.py

```diff
@@ -46,25 +46,27 @@
     def _run(
         self,
         workspace: Path,
         path: Path,
         target_device: DeviceKind,
         jit_type: JitType,
         verbose: bool,
+        strict: bool,
         model: Optional[Any] = None,
         batch_dim: Optional[int] = None,
     ) -> CommandOutput:
         """Execute command.
 
         Args:
             workspace: Workspace where the files are stored.
-            path: Path inside the workspace where exported model is stored
-            verbose: Enable verbose logging
-            model: The model that has to be exported
-            batch_dim: Location of batch position in shapes
+            path: Path inside the workspace where exported model is stored.
+            verbose: Enable verbose logging.
+            strict: Enable or Disable strict flag for tracer used in TorchScript export.
+            model: The model that has to be exported.
+            batch_dim: Location of batch position in shapes.
 
         Returns:
             CommandOutput object with status
         """
         LOGGER.info("TorchScrip export started")
 
         exported_model_path = workspace / path
@@ -94,14 +96,15 @@
         ) as context:
 
             kwargs = {
                 "exported_model_path": exported_model_path.relative_to(workspace).as_posix(),
                 "target_jit_type": jit_type.value,
                 "batch_dim": batch_dim,
                 "target_device": target_device.value,
+                "strict": strict,
                 "navigator_workspace": workspace.as_posix(),
             }
 
             args = parse_kwargs_to_cmd(kwargs)
 
             context.execute_local_runtime_script(
                 exporters.torch2torchscript.__file__, exporters.torch2torchscript.export, args
```

## model_navigator/commands/export/exporters/torch2torchscript.py

```diff
@@ -33,23 +33,25 @@
 
 
 def export(
     exported_model_path: str,
     target_jit_type: str,
     batch_dim: Optional[int],
     target_device: str,
+    strict: bool,
     navigator_workspace: Optional[str] = None,
 ):
     """Export Torch model to ONNX model.
 
     Args:
         exported_model_path (str): Output ONNX model path.
         target_jit_type (str): TorchScript jit type. Could be "trace" or "script".
         batch_dim (Optional[int]): Batch dimension.
         target_device (str): Device to load TorchScript model on.
+        strict (bool): Enable or Disable strict flag for tracer used in TorchScript export.
         navigator_workspace (Optional[str], optional): Model Navigator workspace path.
             When None use current workdir. Defaults to None.
     """
     model = get_model()
     target_jit_type = JitType(target_jit_type)
 
     if not navigator_workspace:
@@ -58,15 +60,15 @@
 
     profiling_sample = load_samples("profiling_sample", navigator_workspace, batch_dim)[0]
 
     if target_jit_type == JitType.SCRIPT:
         script_module = torch.jit.script(model)
     else:
         dummy_input = tuple(torch.from_numpy(val).to(target_device) for val in profiling_sample.values())
-        script_module = torch.jit.trace(model, dummy_input)
+        script_module = torch.jit.trace(model, dummy_input, strict=strict)
 
     exported_model_path = pathlib.Path(exported_model_path)
     if not exported_model_path.is_absolute():
         exported_model_path = navigator_workspace / exported_model_path
 
     torch.jit.save(script_module, exported_model_path.as_posix())
```

## model_navigator/configuration/model/model_config.py

```diff
@@ -8,21 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""This module contains classes represnting model configurations."""
+"""This module contains classes representing model configurations."""
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
-from model_navigator.api.config import Format, JitType, TensorRTPrecision, TensorRTPrecisionMode, TensorRTProfile
+from model_navigator.api.config import (
+    Format,
+    JitType,
+    TensorRTCompatibilityLevel,
+    TensorRTPrecision,
+    TensorRTPrecisionMode,
+    TensorRTProfile,
+)
 from model_navigator.utils.common import DataObject
 from model_navigator.utils.format_helpers import FORMAT2SUFFIX, is_source_format
 
 
 class ModelConfig(ABC, DataObject):
     """Abstrac model configuration class."""
 
@@ -269,31 +276,37 @@
 
 class TorchScriptConfig(_SerializedModelConfig, format=Format.TORCHSCRIPT):
     """TorchScript model configuration class."""
 
     def __init__(
         self,
         jit_type: JitType,
+        strict: bool,
         parent: Optional[ModelConfig] = None,
     ) -> None:
         """Initializes TorchScript model configuration class.
 
         Args:
             jit_type: TorchScript export method
+            strict: Enable or Disable strict flag for tracer used in TorchScript export
             parent: Parent model configuration
         """
         super().__init__(parent=parent)
         self.jit_type = jit_type
+        self.strict = strict
 
     def _get_path_params_as_array_of_strings(self) -> List[str]:
         return [self.jit_type.value] if self.jit_type else []
 
     @classmethod
     def _from_dict(cls, data_dict: Dict):
-        return cls(jit_type=cls._parse_string(JitType, data_dict.get("jit_type")))
+        return cls(
+            jit_type=cls._parse_string(JitType, data_dict.get("jit_type")),
+            strict=cls._parse_string(bool, data_dict.get("strict")),
+        )
 
 
 class ONNXConfig(_SerializedModelConfig, format=Format.ONNX):
     """ONNX model configuration class."""
 
     def __init__(
         self,
@@ -325,44 +338,52 @@
 
     def __init__(
         self,
         precision: TensorRTPrecision,
         precision_mode: TensorRTPrecisionMode,
         max_workspace_size: int,
         trt_profile: Optional[TensorRTProfile],
+        optimization_level: Optional[int],
+        compatibility_level: Optional[TensorRTCompatibilityLevel],
         parent: Optional[ModelConfig] = None,
     ) -> None:
         """Initializes TensorRT (plan) model configuration class.
 
         Args:
             parent: Parent model configuration
             precision: TensorRT model precision
             precision_mode: Mode how the precision flags are combined
             max_workspace_size: The maximum GPU memory the model can use temporarily during execution
             trt_profile: TensorRT profile
+            optimization_level: Level of TensorRT engine optimization
+            compatibility_level: Hardware compatibility level
         """
         super().__init__(parent=parent)
         self.precision = precision
         self.precision_mode = precision_mode
         self.max_workspace_size = max_workspace_size
         self.trt_profile = trt_profile
+        self.optimization_level = optimization_level
+        self.compatibility_level = compatibility_level
 
     def _get_path_params_as_array_of_strings(self) -> List[str]:
         return [self.precision.value] if self.precision else []
 
     @classmethod
     def _from_dict(cls, data_dict: Dict):
         trt_profile = data_dict.get("trt_profile")
         if trt_profile is not None:
             trt_profile = TensorRTProfile.from_dict(trt_profile)
         return cls(
             precision=cls._parse_string(TensorRTPrecision, data_dict.get("precision")),
             precision_mode=cls._parse_string(TensorRTPrecisionMode, data_dict.get("precision_mode")),
             max_workspace_size=cls._parse_string(int, data_dict.get("max_workspace_size")),
             trt_profile=trt_profile,
+            optimization_level=cls._parse_string(int, data_dict.get("optimization_level")),
+            compatibility_level=cls._parse_string(TensorRTCompatibilityLevel, data_dict.get("compatibility_level")),
         )
 
 
 class TensorFlowTensorRTConfig(_SerializedModelConfig, format=Format.TF_TRT):
     """TensorFlow TensorRT model configuration class."""
 
     def __init__(
```

## model_navigator/configuration/model/model_config_builder.py

```diff
@@ -162,15 +162,17 @@
 
         Args:
             custom_configs: Format configurations provided by the user
             model_configs: Dictionary mappint model formats to lists of model configs
         """
         torch_config = _get_custom_config(custom_configs=custom_configs, custom_config_cls=config_api.TorchConfig)
         for jit_type in torch_config.jit_type:
-            model_configs[Format.TORCHSCRIPT].append(model_config.TorchScriptConfig(jit_type=jit_type))
+            model_configs[Format.TORCHSCRIPT].append(
+                model_config.TorchScriptConfig(jit_type=jit_type, strict=torch_config.strict)
+            )
 
     @staticmethod
     def get_torch_trt_config(
         custom_configs: Sequence[config_api.CustomConfigForFormat],
         model_configs: Dict[Format, List[model_config.ModelConfig]],
     ):
         """Append TorchTensorRT model configurations to model_configs dictionary.
@@ -296,9 +298,11 @@
             model_configs[Format.TENSORRT].append(
                 model_config.TensorRTConfig(
                     parent=model_configuration,
                     precision=precision,
                     precision_mode=trt_config.precision_mode,
                     max_workspace_size=trt_config.max_workspace_size,
                     trt_profile=trt_config.trt_profile,
+                    optimization_level=trt_config.optimization_level,
+                    compatibility_level=trt_config.compatibility_level,
                 )
             )
```

## model_navigator/frameworks/tensorrt/utils.py

```diff
@@ -96,15 +96,16 @@
         opt_shapes[batch_dim] = _opt_batch_size(max_batch_size)
 
         new_profile[input_name] = ShapeTuple(trt_profile[input_name].min, tuple(opt_shapes), tuple(max_shapes))
     return new_profile
 
 
 def _opt_batch_size(max_batch_size):
-    opt_batch_size = 2 ** int(math.ceil(math.log2(max_batch_size) * OPT_MAX_SHAPE_RATIO))
+    magnitude = math.floor(math.log2(max_batch_size))
+    opt_batch_size = 2 ** int(math.ceil(magnitude * OPT_MAX_SHAPE_RATIO))
 
     return opt_batch_size
 
 
 def _should_use_v3_api():
     return LooseVersion(trt.__version__) > LooseVersion("8.5.0.9")
```

## Comparing `triton_model_navigator-0.5.4.dist-info/LICENSE` & `triton_model_navigator-0.5.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.5.4.dist-info/METADATA` & `triton_model_navigator-0.5.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.5.4
+Version: 0.5.5
 Summary: Triton Model Navigator provides tools supporting to create Deep Learning production ready inference models
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `triton_model_navigator-0.5.4.dist-info/RECORD` & `triton_model_navigator-0.5.5.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 model_navigator/__init__.py,sha256=YQ8MA8xQgnLgxeQ_oK_E7W8Tpxavwj0SKvbiq4r-JJE,881
-model_navigator/__version__.py,sha256=xPqlSzfRyqv8WWBwF3tFO_eYXdxwofY630AEnR1q4sQ,649
+model_navigator/__version__.py,sha256=OER3JOWyTyl2EWNM_d6KFSiH4Mg0S8OMrlQamc54JuA,649
 model_navigator/exceptions.py,sha256=6wR9REQeNkmHOklMPQ46SrGC61EJVH4jz0n2BC4e7ek,3668
 model_navigator/execution_context.py,sha256=eYV2YJU4V8X-v-dWTI6Oi5zJl3RdtK41XWtPxPRxNvU,9474
 model_navigator/logger.py,sha256=946izjz2i81kuehttGIkJ2_NhpNVCgTt6y9fL-s19-U,4790
-model_navigator/api/__init__.py,sha256=1BVyA9lvyJrVJb8dZWqDCpLP_9ZHdwpI6KUCtCS_SZY,1678
-model_navigator/api/config.py,sha256=JACeU-rAsB5XZWxbNrlD-rxL87dh14eZFYJEvIwqC6E,23210
+model_navigator/api/__init__.py,sha256=ZCychLWYCVP_Q5BWXK7-8FzldMSyFTiGgcT6c_kOnJc,1716
+model_navigator/api/config.py,sha256=MkYyt3XiD37d5ptOOJOvb9HwW-sYKCZetKgCDJfT7lk,24304
 model_navigator/api/jax.py,sha256=eLDXpJsYNhVkquv6bJaO20aXO7aBqWmCGrDd1cvkzDc,6425
 model_navigator/api/onnx.py,sha256=RI9d_-H7_3Q7hkDNSGvQ89jbbbAxS1kLv-8YKlR5Kx0,5423
 model_navigator/api/package.py,sha256=8fi6d_O3z3PqiNa6SrwdvqzVctpLj2DGP5LhcLvlkn0,11860
 model_navigator/api/python.py,sha256=6OaBA1SLP_0YWnqdLf5J8C4DdN2oFjh5SjQq5I6u-_I,4906
 model_navigator/api/pytriton.py,sha256=Wz31ISb3skDmJnOzlBzmwGdr_90febOsPIzqie6K_Dc,7748
 model_navigator/api/tensorflow.py,sha256=hG7e9-NxjRz602wmgKl-JNidslbbanOQPuJO1bjgHgo,6519
 model_navigator/api/torch.py,sha256=IY_FLbh4ntAwqRR1Ji213r2XVOsd6GnjSeyAD2MmIgA,6325
 model_navigator/api/triton.py,sha256=hdrU_WJn5DFzhJ5slcdJqzRcC7n69vhmP0RKa1B3QYQ,1553
+model_navigator/api/utilities.py,sha256=iDAsvY2lFZ1ri54OSmThTVokJ31vCnHoylBHiKkYUNg,1811
 model_navigator/commands/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/base.py,sha256=O75ENxJH4GtjYHru56h5XSLrR_iqnsbaQE7YHbtOnLk,4938
 model_navigator/commands/infer_metadata.py,sha256=uFDHHnadjjOFTjNVSPigBXcZYTD3h9jtPPj8-EtndWc,10065
 model_navigator/commands/load.py,sha256=7v1YqLbG0VZOf981XW-2Y6ad828d4Ynq2HNmj7_a8ys,3289
 model_navigator/commands/convert/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/convert/base.py,sha256=YlFjgaik1oqZr9m8FujYQ-gunFoHXA8dgLScgXTG__E,9863
 model_navigator/commands/convert/tf.py,sha256=tQw4DTmAqzDO0pr7ZPMjzTInmd11qmsNIKW6JsWasNM,7838
 model_navigator/commands/convert/torch.py,sha256=s7l6jNhoG4zoej3EOVbw04MGJ67HIw1XFa58OV_a4Js,10224
 model_navigator/commands/convert/converters/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/convert/converters/sm2tftrt.py,sha256=AcNyKV60yCUrzJ5B501H5SHKjtkr7kaNXNIewnOFJzk,3418
 model_navigator/commands/convert/converters/ts2onnx.py,sha256=ezjlPeHHbhx2LB4HDoLkVlmaZa1dreVMQMk2PL5UMos,3105
 model_navigator/commands/convert/converters/ts2torchtrt.py,sha256=a_mpR0j4y5ClaY6Ik_oIKEAlh45zD-ycCLHigsy1C7M,4992
 model_navigator/commands/convert/onnx/__init__.py,sha256=LwvvDj4oH7rwmUJXVEyRxIOWZnUxix6n_DmkAJzEJBY,680
 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py,sha256=KQR-qrVWVVBGVr5pqcKink2dcDNCk1Lszvl8x6TwqjU,1727
-model_navigator/commands/convert/onnx/onnx2trt.py,sha256=Zo28u93a3_ZmCNi9JVnZvD91Y-SsqfhxYMIjpPe8QVc,10454
+model_navigator/commands/convert/onnx/onnx2trt.py,sha256=FI-EKl4IP5wz_UTquhNz2xZFoe2BT3EQO_JbW3Klq8g,10818
 model_navigator/commands/convert/onnx/trt_load_script.py,sha256=D2fTNNIBELAsBSmy3ij9oxMyRDxi0RNFV29zAlPYFz8,2235
 model_navigator/commands/copy/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/copy/onnx.py,sha256=Z2dtowzXW1qVJq2L4bNNLLRRTbyeiJT7MoIxi4y42fk,1729
 model_navigator/commands/correctness/__init__.py,sha256=Xm-ikcHX6zpdmukjkSgL4JnPt2FIImoxXUPsL-334FM,678
 model_navigator/commands/correctness/correctness.py,sha256=qPBKlBE_wuJTtIJ2tt8zXWjFestp-nDvIn3Zh5T5xsc,5594
 model_navigator/commands/correctness/correctness_script.py,sha256=USxoVaa0flsEjNy-vYxjDTkF5Z-lVSY6Jl6Zv9sqNOA,4550
 model_navigator/commands/data_dump/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/data_dump/samples.py,sha256=9oJ8WEQLz5tGr1RvskjvXganpnL1p3E0BDcTF9lrI5I,11162
 model_navigator/commands/export/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/export/jax.py,sha256=A9MBAKbu99UNqbHxAp87sKkwZnQgLn9ZY1kD40XLYEc,3531
 model_navigator/commands/export/tf.py,sha256=JSQ4JrMf2duzhxoimae0g3tJtJaD7RXHsuyMUHkC-b0,5485
-model_navigator/commands/export/torch.py,sha256=3OxVUNKs49vxf0-ifMGZDjeXpdFGwdkA3mGv2v5Vku8,8894
+model_navigator/commands/export/torch.py,sha256=gueN1U39frfBMxeWL5Ivi7OaB87gH5HVcUQDg0E8p-Q,9043
 model_navigator/commands/export/exporters/__init__.py,sha256=ZkOuCGTEqfxCY1PilU3DJV4IMMuMpTEEm2KsCmmcoMQ,1056
 model_navigator/commands/export/exporters/jax2savedmodel.py,sha256=LSr8I4mRHpwYZNDCs3IfUAyk3n89951bjA1JM_rnQks,3945
 model_navigator/commands/export/exporters/keras2savedmodel.py,sha256=oG4BqcklEmTtpwd3tlyKhNBub41VrQBqiiTfRKZaU6Q,3171
 model_navigator/commands/export/exporters/savedmodel2savedmodel.py,sha256=sdE76nSyXD8i_OfePhOEFBiMQFSOsVRiFf8bu26SoaE,3122
 model_navigator/commands/export/exporters/torch2onnx.py,sha256=sTj6uVxFfr-avTjSWC9RXayQhyPkyvjY1YWJhXFrQxc,3077
-model_navigator/commands/export/exporters/torch2torchscript.py,sha256=6UvzjqvfY6GfcPIN8tScmfK2nvCsw6h_pd-MBUwIUHk,2603
+model_navigator/commands/export/exporters/torch2torchscript.py,sha256=UdBcw1TVoaj85Tg6ww-MhkGkHB15ZfbJf6x9szJ3PXE,2728
 model_navigator/commands/find_max_batch_size/__init__.py,sha256=-j67tQs-RhZGWwXSqmRZ7OqR7NOdNRjg4RhBgvOhBhg,715
 model_navigator/commands/find_max_batch_size/find_max_batch_size.py,sha256=_iOAw1NPGPwzaeMu8yy-xBdougxFNSDlVu3RrsBw9ng,6396
 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py,sha256=WWbNxCUm8D4KoUl0VIka4E8roqGU8NI3IHVYr6dgHhg,2984
 model_navigator/commands/performance/__init__.py,sha256=ypw9fRZEp0MA0z1qAxb4-7t9LuUtyRASNP5WHBoMAlw,688
 model_navigator/commands/performance/performance.py,sha256=Kq5-gYrxhXpzNhCeVVSw_EL8I8zQaaPpfAwi7qjGknU,15770
 model_navigator/commands/performance/performance_script.py,sha256=oIUR9gDtknCq6RQ-B9NFQFLwtiRIPjPlqw8VxFkV5Q8,3037
 model_navigator/commands/verification/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/verification/verify.py,sha256=WPZlbUgaQFprBPVhbCYWfk3m1k65f8RMJVtvBYocNt8,5441
 model_navigator/configuration/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/configuration/common_config.py,sha256=MgweUSANUGWnVSlvPvYH1VHxXYspkQ5YLQrZifKlb0g,2473
 model_navigator/configuration/model/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/configuration/model/model_config.py,sha256=_CS3i4OGmHmWyGAywrgV6T6y0I_9Cd-2NhWT_7U8CN8,14775
-model_navigator/configuration/model/model_config_builder.py,sha256=qi6TY7UNB4bLyDJDOwxd0tLNj-oHcGOgVrQebupUa2c,13477
+model_navigator/configuration/model/model_config.py,sha256=LHeJ9oWqigacrWLf0_bc0PIC4EoJMduaec3C8-QgF2I,15623
+model_navigator/configuration/model/model_config_builder.py,sha256=ZkCiMQDzJz8s53bp6lCBENlIr_p_65ET8UPEtj8j7Cs,13677
 model_navigator/core/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/core/constants.py,sha256=lzbcvfiiXrGjUfkGv1qTjsgSSKpUmyxvs2rBLOGeWLM,1326
 model_navigator/core/package.py,sha256=sOJ1pi4ygF2Xl4yodEKYf4r-BS8yupJiiMshQQsCkl0,20111
 model_navigator/core/status.py,sha256=BPRoUsETy-YC4bD3B5u4WUUCNK6YDalkpFagvW6Dn7I,20337
 model_navigator/core/tensor.py,sha256=21C_4LlFnakdc2Ix1QVRcvL917QoFcsi5f-xgN94O3k,8052
 model_navigator/frameworks/__init__.py,sha256=4ACuhCJjgzDo3zub8dNU_FYLiioG8n8iFFiO3LftbFg,2817
 model_navigator/frameworks/jax/__init__.py,sha256=DBjOUuVsMRMwOEPVPFVKQxPQTkYYcRLHvT0jjh907b4,669
 model_navigator/frameworks/jax/model.py,sha256=WROviV0IDfQKkfneaX88wZm7f3WhrB4DwB3-bl4_Qio,1554
 model_navigator/frameworks/onnx/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/frameworks/onnx/utils.py,sha256=L3IDVu0r-_BHSdf4htXwsmMVPoInk9Qset6SA66LusI,1085
 model_navigator/frameworks/tensorrt/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/frameworks/tensorrt/cuda.py,sha256=dT5HPExUqQnsR3npcpgCuc0iCnAUTSfjkLK-2eNkiw4,26575
-model_navigator/frameworks/tensorrt/utils.py,sha256=2msVkXizTMi4sn2EdIht_JGdLWW2FsZH8w-yG2j0lkw,9836
+model_navigator/frameworks/tensorrt/utils.py,sha256=sPmc1OF84WRzYLi7MFgjpKJkx8Rv4-Xx-fbMFRfGggs,9874
 model_navigator/frameworks/torch/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/frameworks/torch/utils.py,sha256=czQ3umUl1UtYydDApapftpEOBZsWCAdVyPD5wF9Gjq8,1508
 model_navigator/pipelines/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/pipelines/pipeline.py,sha256=l5ZGqSbdLwKanojJJGdQfDnABgJB_c-NGPnYJoQkB14,5685
 model_navigator/pipelines/pipeline_manager.py,sha256=4iBxa5-cT-Dch4Y1NNsPtK32-ypYPfFpkrKVwFsyKRA,7333
 model_navigator/pipelines/validation.py,sha256=5N8KOjMCOI_TH3JYKMQgyWH24l5OXvZrMAsSoI8n1-s,9805
 model_navigator/pipelines/builders/__init__.py,sha256=itg2I3yJgd25bTF1ewdEla6R5xjYO-8IwtOOYf0NQAg,1879
@@ -121,12 +122,12 @@
 model_navigator/utils/dataloader.py,sha256=_fxjq2vP4DNFxOEZA_HPX_8caQcbSwgP55gdey9rq-M,7996
 model_navigator/utils/devices.py,sha256=pGjRBByJqFjG6dyJ0H2E6GJA7hIgF6rgeINLNdS27kU,3902
 model_navigator/utils/enums.py,sha256=T-G5VV5CqimxpctOqPaCvVoAwx-pp10Eeo0rKlWoVGU,1308
 model_navigator/utils/environment.py,sha256=MnpdF5eCx2DJpHtaq8fUSky0hdT03qTJrGnJDhCnFhM,6163
 model_navigator/utils/format_helpers.py,sha256=VAbRMfBw-eZljk_yDcV6Q1ojkl8ah1OnqZR6DshXNqU,3528
 model_navigator/utils/module.py,sha256=fkokQmxhWgShqrhsXDPa-g-jBA0XaUQvuVuM74WPOIM,2325
 model_navigator/utils/package.py,sha256=wp1xOwrKuB_rtVfe61y2AznmA-up320RtHNNV2UExe4,3233
-triton_model_navigator-0.5.4.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.5.4.dist-info/METADATA,sha256=JznkmKwEXb1nm_-5LMI3Abw4ePpqQ-YyH8SZiKOFozk,12074
-triton_model_navigator-0.5.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-triton_model_navigator-0.5.4.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.5.4.dist-info/RECORD,,
+triton_model_navigator-0.5.5.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.5.5.dist-info/METADATA,sha256=-q2kbOGb5fXNXyHKmRT0vEHy3ihlW97_-UUMeApvLys,12074
+triton_model_navigator-0.5.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+triton_model_navigator-0.5.5.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.5.5.dist-info/RECORD,,
```


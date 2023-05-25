# Comparing `tmp/nvidia-dali-tf-plugin-cuda110-1.25.0.tar.gz` & `tmp/nvidia-dali-tf-plugin-cuda110-1.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-cuda110-1.25.0.tar", last modified: Tue Apr 11 13:03:36 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-cuda110-1.26.0.tar", last modified: Fri May 12 16:29:46 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0.tar` & `nvidia-dali-tf-plugin-cuda110-1.26.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.279297 nvidia-dali-tf-plugin-cuda110-1.25.0/
--rw-r--r--   0 root         (0) root         (0)      160 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2735 2023-04-11 13:03:36.279297 nvidia-dali-tf-plugin-cuda110-1.25.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    43001 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/dali_dataset_op.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.263297 nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin/
--rw-r--r--   0 root         (0) root         (0)     5169 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin/dali_dataset.h
--rw-r--r--   0 root         (0) root         (0)     7079 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin/dali_helper.h
--rw-r--r--   0 root         (0) root         (0)    17344 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin_install_tool.py
--rw-r--r--   0 root         (0) root         (0)     6207 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin_utils.py
--rw-r--r--   0 root         (0) root         (0)    17543 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/daliop.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.259297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.263297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/
--rw-r--r--   0 root         (0) root         (0)    27259 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/c_api.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.271297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/
--rw-r--r--   0 root         (0) root         (0)     5686 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/access_order.h
--rw-r--r--   0 root         (0) root         (0)    10320 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/any.h
--rw-r--r--   0 root         (0) root         (0)     1461 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/api_helper.h
--rw-r--r--   0 root         (0) root         (0)     2207 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/backend_tags.h
--rw-r--r--   0 root         (0) root         (0)     7777 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/bitmask.h
--rw-r--r--   0 root         (0) root         (0)     7937 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/boundary.h
--rw-r--r--   0 root         (0) root         (0)     3297 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/byte_io.h
--rw-r--r--   0 root         (0) root         (0)     1281 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/call_at_exit.h
--rw-r--r--   0 root         (0) root         (0)     5354 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/common.h
--rw-r--r--   0 root         (0) root         (0)    17542 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/convert.h
--rw-r--r--   0 root         (0) root         (0)     2428 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/copy_vector_helper.h
--rw-r--r--   0 root         (0) root         (0)     5249 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_error.h
--rw-r--r--   0 root         (0) root         (0)     1895 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_event.h
--rw-r--r--   0 root         (0) root         (0)     3154 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_event_pool.h
--rw-r--r--   0 root         (0) root         (0)     2460 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_rt_utils.h
--rw-r--r--   0 root         (0) root         (0)     2059 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_stream.h
--rw-r--r--   0 root         (0) root         (0)     7050 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_stream_pool.h
--rw-r--r--   0 root         (0) root         (0)     2179 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_utils.h
--rw-r--r--   0 root         (0) root         (0)     5012 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dev_array.h
--rw-r--r--   0 root         (0) root         (0)     5315 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dev_buffer.h
--rw-r--r--   0 root         (0) root         (0)     6438 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dev_string.h
--rw-r--r--   0 root         (0) root         (0)     1381 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/device_guard.h
--rw-r--r--   0 root         (0) root         (0)      815 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dynlink_cuda.h
--rw-r--r--   0 root         (0) root         (0)     5034 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dynlink_cufile.h
--rw-r--r--   0 root         (0) root         (0)     6146 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/endian_util.h
--rw-r--r--   0 root         (0) root         (0)    10891 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/error_handling.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.271297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/exec/
--rw-r--r--   0 root         (0) root         (0)     2115 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/exec/engine.h
--rw-r--r--   0 root         (0) root         (0)     4648 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/expand_dims.h
--rw-r--r--   0 root         (0) root         (0)     6831 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/fast_div.h
--rw-r--r--   0 root         (0) root         (0)    14461 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/float16.h
--rw-r--r--   0 root         (0) root         (0)      977 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/force_inline.h
--rw-r--r--   0 root         (0) root         (0)     3478 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/format.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.271297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/
--rw-r--r--   0 root         (0) root         (0)     5018 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/box.h
--rw-r--r--   0 root         (0) root         (0)     1706 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/geom_utils.h
--rw-r--r--   0 root         (0) root         (0)    17992 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/mat.h
--rw-r--r--   0 root         (0) root         (0)     4521 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/transform.h
--rw-r--r--   0 root         (0) root         (0)    21114 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/vec.h
--rw-r--r--   0 root         (0) root         (0)     1160 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/host_dev.h
--rw-r--r--   0 root         (0) root         (0)     2267 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/int_literals.h
--rw-r--r--   0 root         (0) root         (0)     5889 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/math_util.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.275297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/
--rw-r--r--   0 root         (0) root         (0)    22047 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/async_pool.h
--rw-r--r--   0 root         (0) root         (0)     5291 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/composite_resource.h
--rw-r--r--   0 root         (0) root         (0)     9018 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/cu_vm.h
--rw-r--r--   0 root         (0) root         (0)    27092 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/cuda_vm_resource.h
--rw-r--r--   0 root         (0) root         (0)     5267 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/default_resources.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.275297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/
--rw-r--r--   0 root         (0) root         (0)     3850 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/align.h
--rw-r--r--   0 root         (0) root         (0)     6541 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/aux_alloc.h
--rw-r--r--   0 root         (0) root         (0)     1426 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/aux_collections.h
--rw-r--r--   0 root         (0) root         (0)    25585 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/free_list.h
--rw-r--r--   0 root         (0) root         (0)     2332 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/util.h
--rw-r--r--   0 root         (0) root         (0)     2934 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/fixed_order_resource.h
--rw-r--r--   0 root         (0) root         (0)     6580 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/malloc_resource.h
--rw-r--r--   0 root         (0) root         (0)    22782 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/memory.h
--rw-r--r--   0 root         (0) root         (0)     2057 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/memory_kind.h
--rw-r--r--   0 root         (0) root         (0)     2278 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/memory_resource.h
--rw-r--r--   0 root         (0) root         (0)     9348 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/monotonic_resource.h
--rw-r--r--   0 root         (0) root         (0)    11682 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/pool_resource.h
--rw-r--r--   0 root         (0) root         (0)     1084 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/pool_resource_base.h
--rw-r--r--   0 root         (0) root         (0)      998 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/with_upstream.h
--rw-r--r--   0 root         (0) root         (0)     3169 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/nvtx.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.275297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/os/
--rw-r--r--   0 root         (0) root         (0)     5420 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/os/shared_mem.h
--rw-r--r--   0 root         (0) root         (0)     4677 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/partition.h
--rw-r--r--   0 root         (0) root         (0)    10461 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/per_stream_pool.h
--rw-r--r--   0 root         (0) root         (0)     3288 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/permute.h
--rw-r--r--   0 root         (0) root         (0)     2337 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/python_util.h
--rw-r--r--   0 root         (0) root         (0)     3283 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/random.h
--rw-r--r--   0 root         (0) root         (0)    19482 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/small_vector.h
--rw-r--r--   0 root         (0) root         (0)     9394 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/span.h
--rw-r--r--   0 root         (0) root         (0)     1902 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/spinlock.h
--rw-r--r--   0 root         (0) root         (0)     5372 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/static_map.h
--rw-r--r--   0 root         (0) root         (0)     6547 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/static_switch.h
--rw-r--r--   0 root         (0) root         (0)     5872 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/stream.h
--rw-r--r--   0 root         (0) root         (0)    18748 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tensor_layout.h
--rw-r--r--   0 root         (0) root         (0)    54963 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tensor_shape.h
--rw-r--r--   0 root         (0) root         (0)     1617 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tensor_shape_print.h
--rw-r--r--   0 root         (0) root         (0)    33471 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tensor_view.h
--rw-r--r--   0 root         (0) root         (0)     2403 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/traits.h
--rw-r--r--   0 root         (0) root         (0)     8062 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tuple_helpers.h
--rw-r--r--   0 root         (0) root         (0)     5479 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/unique_handle.h
--rw-r--r--   0 root         (0) root         (0)    13684 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/util.h
--rw-r--r--   0 root         (0) root         (0)     1655 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/version_util.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.275297 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/
--rw-r--r--   0 root         (0) root         (0)     5734 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/decode_results.h
--rw-r--r--   0 root         (0) root         (0)     8884 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_decoder.h
--rw-r--r--   0 root         (0) root         (0)     8845 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_decoder_interfaces.h
--rw-r--r--   0 root         (0) root         (0)     4098 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_format.h
--rw-r--r--   0 root         (0) root         (0)     1542 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_orientation.h
--rw-r--r--   0 root         (0) root         (0)     5546 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_source.h
--rw-r--r--   0 root         (0) root         (0)     1992 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/operators.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.259297 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.275297 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/
--rw-r--r--   0 root         (0) root         (0)   256667 2023-03-29 07:29:37.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/Acknowledgements.txt
--rw-r--r--   0 root         (0) root         (0)      621 2023-03-29 07:29:37.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/COPYRIGHT
--rw-r--r--   0 root         (0) root         (0)    10142 2023-03-29 07:29:37.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      690 2023-04-11 13:03:35.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/dali_tf_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.279297 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2735 2023-04-11 13:03:36.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3985 2023-04-11 13:03:36.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:03:36.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:03:36.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 13:03:36.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-11 13:03:36.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.279297 nvidia-dali-tf-plugin-cuda110-1.25.0/prebuilt/
--rw-r--r--   0 root         (0) root         (0)   206632 2023-04-11 13:03:30.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/prebuilt/libdali_tf_2_11.so
--rw-r--r--   0 root         (0) root         (0)   206896 2023-04-11 13:03:30.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/prebuilt/libdali_tf_2_12.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:03:36.279297 nvidia-dali-tf-plugin-cuda110-1.25.0/prebuilt/stub/
--rw-r--r--   0 root         (0) root         (0)    13800 2023-04-11 13:03:30.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/prebuilt/stub/libdali.so
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:03:36.279297 nvidia-dali-tf-plugin-cuda110-1.25.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4409 2023-04-11 13:03:35.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-03-29 07:29:38.000000 nvidia-dali-tf-plugin-cuda110-1.25.0/stubgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.100265 nvidia-dali-tf-plugin-cuda110-1.26.0/
+-rw-r--r--   0 root         (0) root         (0)      160 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-05-12 16:29:46.100265 nvidia-dali-tf-plugin-cuda110-1.26.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    43001 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_dataset_op.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.088265 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/
+-rw-r--r--   0 root         (0) root         (0)     5169 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/dali_dataset.h
+-rw-r--r--   0 root         (0) root         (0)     7079 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/dali_helper.h
+-rw-r--r--   0 root         (0) root         (0)    17344 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin_install_tool.py
+-rw-r--r--   0 root         (0) root         (0)     6207 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17543 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/daliop.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.088265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.088265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/
+-rw-r--r--   0 root         (0) root         (0)    27259 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/c_api.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.092265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/
+-rw-r--r--   0 root         (0) root         (0)     5686 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/access_order.h
+-rw-r--r--   0 root         (0) root         (0)    10320 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/any.h
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/api_helper.h
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/backend_tags.h
+-rw-r--r--   0 root         (0) root         (0)     7777 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/bitmask.h
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/boundary.h
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/byte_io.h
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/call_at_exit.h
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/common.h
+-rw-r--r--   0 root         (0) root         (0)    17542 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/convert.h
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/copy_vector_helper.h
+-rw-r--r--   0 root         (0) root         (0)     5249 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_error.h
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_event.h
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_event_pool.h
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_rt_utils.h
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_stream.h
+-rw-r--r--   0 root         (0) root         (0)     7050 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_stream_pool.h
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_utils.h
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_array.h
+-rw-r--r--   0 root         (0) root         (0)     5315 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     6438 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_string.h
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/device_guard.h
+-rw-r--r--   0 root         (0) root         (0)      815 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dynlink_cuda.h
+-rw-r--r--   0 root         (0) root         (0)     5034 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dynlink_cufile.h
+-rw-r--r--   0 root         (0) root         (0)     6146 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/endian_util.h
+-rw-r--r--   0 root         (0) root         (0)    10891 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/error_handling.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.092265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/exec/
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/exec/engine.h
+-rw-r--r--   0 root         (0) root         (0)     4648 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/expand_dims.h
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/fast_div.h
+-rw-r--r--   0 root         (0) root         (0)    14461 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/float16.h
+-rw-r--r--   0 root         (0) root         (0)      977 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/force_inline.h
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/format.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.092265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/box.h
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/geom_utils.h
+-rw-r--r--   0 root         (0) root         (0)    17992 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/mat.h
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/transform.h
+-rw-r--r--   0 root         (0) root         (0)    21114 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/vec.h
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/host_dev.h
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/int_literals.h
+-rw-r--r--   0 root         (0) root         (0)     5889 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/math_util.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/
+-rw-r--r--   0 root         (0) root         (0)    22047 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/async_pool.h
+-rw-r--r--   0 root         (0) root         (0)     5291 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/composite_resource.h
+-rw-r--r--   0 root         (0) root         (0)     9018 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/cu_vm.h
+-rw-r--r--   0 root         (0) root         (0)    27092 2023-05-09 19:27:36.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/cuda_vm_resource.h
+-rw-r--r--   0 root         (0) root         (0)     5267 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/default_resources.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/align.h
+-rw-r--r--   0 root         (0) root         (0)     6541 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/aux_alloc.h
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/aux_collections.h
+-rw-r--r--   0 root         (0) root         (0)    25585 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/free_list.h
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/util.h
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/fixed_order_resource.h
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/malloc_resource.h
+-rw-r--r--   0 root         (0) root         (0)    22782 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory.h
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory_kind.h
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory_resource.h
+-rw-r--r--   0 root         (0) root         (0)     9348 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/monotonic_resource.h
+-rw-r--r--   0 root         (0) root         (0)    11682 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/pool_resource.h
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/pool_resource_base.h
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/with_upstream.h
+-rw-r--r--   0 root         (0) root         (0)     3169 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/nvtx.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/os/
+-rw-r--r--   0 root         (0) root         (0)     5420 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/os/shared_mem.h
+-rw-r--r--   0 root         (0) root         (0)     4677 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/partition.h
+-rw-r--r--   0 root         (0) root         (0)    10461 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/per_stream_pool.h
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/permute.h
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/python_util.h
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/random.h
+-rw-r--r--   0 root         (0) root         (0)    19482 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/small_vector.h
+-rw-r--r--   0 root         (0) root         (0)     9394 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/span.h
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/spinlock.h
+-rw-r--r--   0 root         (0) root         (0)     5372 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/static_map.h
+-rw-r--r--   0 root         (0) root         (0)     6547 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/static_switch.h
+-rw-r--r--   0 root         (0) root         (0)     5872 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/stream.h
+-rw-r--r--   0 root         (0) root         (0)    18748 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_layout.h
+-rw-r--r--   0 root         (0) root         (0)    54963 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_shape.h
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_shape_print.h
+-rw-r--r--   0 root         (0) root         (0)    33471 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_view.h
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/traits.h
+-rw-r--r--   0 root         (0) root         (0)     8062 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tuple_helpers.h
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/unique_handle.h
+-rw-r--r--   0 root         (0) root         (0)    13956 2023-04-27 19:33:13.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/util.h
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/version_util.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/decode_results.h
+-rw-r--r--   0 root         (0) root         (0)     8884 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_decoder.h
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_decoder_interfaces.h
+-rw-r--r--   0 root         (0) root         (0)     4098 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_format.h
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_orientation.h
+-rw-r--r--   0 root         (0) root         (0)     5546 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_source.h
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/operators.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.088265 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/
+-rw-r--r--   0 root         (0) root         (0)   256667 2023-04-24 07:02:14.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/Acknowledgements.txt
+-rw-r--r--   0 root         (0) root         (0)      621 2023-04-24 07:02:14.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/COPYRIGHT
+-rw-r--r--   0 root         (0) root         (0)    10142 2023-04-24 07:02:14.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      690 2023-05-12 16:29:45.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-04-24 07:02:48.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/dali_tf_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3985 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-12 16:29:46.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.096265 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/
+-rw-r--r--   0 root         (0) root         (0)   206632 2023-05-12 16:29:42.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/libdali_tf_2_11.so
+-rw-r--r--   0 root         (0) root         (0)   206896 2023-05-12 16:29:42.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/libdali_tf_2_12.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:29:46.100265 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/stub/
+-rw-r--r--   0 root         (0) root         (0)    13800 2023-05-12 16:29:42.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/stub/libdali.so
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 16:29:46.100265 nvidia-dali-tf-plugin-cuda110-1.26.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4409 2023-05-12 16:29:45.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-04-24 07:05:38.000000 nvidia-dali-tf-plugin-cuda110-1.26.0/stubgen.py
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/PKG-INFO` & `nvidia-dali-tf-plugin-cuda110-1.26.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-cuda110
-Version: 1.25.0
-Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 8a17f3caa31ab99c1a13f36eb8208beb410eba52
+Version: 1.26.0
+Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: cdc39704b8f824f342e0e0c9163ba12518434987
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Description: TensorFlow plugin for NVIDIA DALI
         =================================
         
         The TensorFlow plugin enables usage of DALI with TensorFlow.
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/dali_dataset_op.cc` & `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_dataset_op.cc`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin/dali_dataset.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/dali_dataset.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin/dali_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin/dali_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin_install_tool.py` & `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin_install_tool.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/dali_tf_plugin_utils.py` & `nvidia-dali-tf-plugin-cuda110-1.26.0/dali_tf_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/daliop.cc` & `nvidia-dali-tf-plugin-cuda110-1.26.0/daliop.cc`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/c_api.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/c_api.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/access_order.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/access_order.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/any.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/any.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/api_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/api_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/backend_tags.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/backend_tags.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/bitmask.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/bitmask.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/boundary.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/boundary.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/byte_io.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/byte_io.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/call_at_exit.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/call_at_exit.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/common.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/common.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/convert.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/convert.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/copy_vector_helper.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/copy_vector_helper.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_error.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_error.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_event.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_event.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_event_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_event_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_rt_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_rt_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_stream.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_stream.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_stream_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_stream_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/cuda_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dev_array.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_array.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dev_buffer.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_buffer.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dev_string.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dev_string.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/device_guard.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/device_guard.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dynlink_cuda.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dynlink_cuda.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/dynlink_cufile.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/dynlink_cufile.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/endian_util.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/endian_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/error_handling.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/error_handling.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/exec/engine.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/exec/engine.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/expand_dims.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/expand_dims.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/fast_div.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/fast_div.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/float16.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/float16.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/force_inline.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/force_inline.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/format.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/format.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/box.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/box.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/geom_utils.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/geom_utils.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/mat.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/mat.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/transform.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/transform.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/geom/vec.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/geom/vec.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/host_dev.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/host_dev.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/int_literals.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/int_literals.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/math_util.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/math_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/async_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/async_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/composite_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/composite_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/cu_vm.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/cu_vm.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/cuda_vm_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/cuda_vm_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/default_resources.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/default_resources.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/align.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/align.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/aux_alloc.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/aux_alloc.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/aux_collections.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/aux_collections.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/free_list.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/free_list.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/detail/util.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/detail/util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/fixed_order_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/fixed_order_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/malloc_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/malloc_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/memory.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/memory_kind.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory_kind.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/memory_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/memory_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/monotonic_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/monotonic_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/pool_resource.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/pool_resource.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/pool_resource_base.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/pool_resource_base.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/mm/with_upstream.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/mm/with_upstream.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/nvtx.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/nvtx.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/os/shared_mem.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/os/shared_mem.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/partition.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/partition.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/per_stream_pool.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/per_stream_pool.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/permute.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/permute.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/python_util.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/python_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/random.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/random.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/small_vector.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/small_vector.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/span.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/span.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/spinlock.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/spinlock.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/static_map.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/static_map.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/static_switch.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/static_switch.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/stream.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/stream.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tensor_layout.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_layout.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tensor_shape.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_shape.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tensor_shape_print.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_shape_print.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tensor_view.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tensor_view.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/traits.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/traits.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/tuple_helpers.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/tuple_helpers.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/unique_handle.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/unique_handle.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/util.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/util.h`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,25 @@
 
 template <typename Value, typename Alignment>
 DALI_HOST_DEV
 constexpr Value align_up(Value v, Alignment a) {
   return v + ((a - 1) & -v);
 }
 
+template <typename Value, typename Alignment>
+DALI_HOST_DEV
+constexpr Value alignment_offset(Value v, Alignment a) {
+  return v & (a - 1);
+}
+
+template <typename Value, typename Alignment>
+DALI_HOST_DEV
+constexpr Value align_down(Value v, Alignment a) {
+  return v & -a;
+}
 
 DALI_HOST_DEV
 constexpr int32_t div_ceil(int32_t total, uint32_t grain) {
   return (total + grain - 1) / grain;
 }
 
 DALI_HOST_DEV
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/core/version_util.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/core/version_util.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/decode_results.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/decode_results.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_decoder.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_decoder.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_decoder_interfaces.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_decoder_interfaces.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_format.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_format.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_orientation.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_orientation.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/imgcodec/image_source.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/imgcodec/image_source.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/include/dali/operators.h` & `nvidia-dali-tf-plugin-cuda110-1.26.0/include/dali/operators.h`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/Acknowledgements.txt` & `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/Acknowledgements.txt`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/COPYRIGHT` & `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/LICENSE` & `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/LICENSE`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/__init__.py` & `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.25.0'
-__git_sha__ = '8a17f3caa31ab99c1a13f36eb8208beb410eba52'
+__version__ = '1.26.0'
+__git_sha__ = 'cdc39704b8f824f342e0e0c9163ba12518434987'
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia/dali_tf_plugin/dali_tf_plugin.py` & `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia/dali_tf_plugin/dali_tf_plugin.py`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-cuda110
-Version: 1.25.0
-Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 8a17f3caa31ab99c1a13f36eb8208beb410eba52
+Version: 1.26.0
+Summary: NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: cdc39704b8f824f342e0e0c9163ba12518434987
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Description: TensorFlow plugin for NVIDIA DALI
         =================================
         
         The TensorFlow plugin enables usage of DALI with TensorFlow.
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt` & `nvidia-dali-tf-plugin-cuda110-1.26.0/nvidia_dali_tf_plugin_cuda110.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/prebuilt/libdali_tf_2_11.so` & `nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/libdali_tf_2_11.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/prebuilt/libdali_tf_2_12.so` & `nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/libdali_tf_2_12.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/prebuilt/stub/libdali.so` & `nvidia-dali-tf-plugin-cuda110-1.26.0/prebuilt/stub/libdali.so`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/setup.py` & `nvidia-dali-tf-plugin-cuda110-1.26.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         # It doesn't matter what we write here, because we are overriding the
         # build_ext step altogether.
         # By filling this ext_modules we are signaling that this package needs
         # to be built for different platforms
         self.ext_modules = [Extension('nvidia.dali_tf_plugin', [])]
 
 setup(name='nvidia-dali-tf-plugin-cuda110',
-      description='NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: 8a17f3caa31ab99c1a13f36eb8208beb410eba52',
+      description='NVIDIA DALI  TensorFlow plugin for CUDA 11.0. Git SHA: cdc39704b8f824f342e0e0c9163ba12518434987',
       long_description='''TensorFlow plugin for NVIDIA DALI
 =================================
 
 The TensorFlow plugin enables usage of DALI with TensorFlow.
 
 The NVIDIA Data Loading Library (DALI) is a library for data loading and
 pre-processing to accelerate deep learning applications. It provides a
@@ -70,30 +70,30 @@
     :alt: DALI Diagram
 
 .. |release-doc| replace:: latest DALI Documentation
 .. _release-doc: https://docs.nvidia.com/deeplearning/dali/user-guide/docs/index.html
 ''',
       long_description_content_type="text/x-rst",
       url='https://github.com/NVIDIA/dali',
-      version='1.25.0',
+      version='1.26.0',
       author='NVIDIA Corporation',
       license='Apache License 2.0',
       packages=find_namespace_packages(include=['nvidia.*']),
       include_package_data=True,
       zip_safe=False,
       python_requires='>=3.6, <3.11',
       classifiers=[
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           ],
       install_requires = [
-          'nvidia-dali-cuda110==1.25.0'
+          'nvidia-dali-cuda110==1.26.0'
           ],
 
       cmdclass={
           'build_ext': CustomBuildExt,
       },
       distclass=CustomDistribution
      )
```

### Comparing `nvidia-dali-tf-plugin-cuda110-1.25.0/stubgen.py` & `nvidia-dali-tf-plugin-cuda110-1.26.0/stubgen.py`

 * *Files identical despite different names*


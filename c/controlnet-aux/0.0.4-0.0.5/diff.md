# Comparing `tmp/controlnet_aux-0.0.4.tar.gz` & `tmp/controlnet_aux-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlnet_aux-0.0.4.tar", last modified: Mon May 22 20:32:50 2023, max compression
+gzip compressed data, was "controlnet_aux-0.0.5.tar", last modified: Fri May 26 09:48:40 2023, max compression
```

## Comparing `controlnet_aux-0.0.4.tar` & `controlnet_aux-0.0.5.tar`

### file list

```diff
@@ -1,180 +1,181 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11357 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/LICENSE.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3250 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2320 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/README.md
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8756 2023-05-22 20:31:03.000000 controlnet_aux-0.0.4/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.557665 controlnet_aux-0.0.4/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      515 2023-05-22 20:31:09.000000 controlnet_aux-0.0.4/src/controlnet_aux/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/canny/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      547 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/canny/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/hed/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7994 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/hed/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/lineart/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5293 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/lineart/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/lineart_anime/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7718 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/lineart_anime/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/mediapipe_face/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      645 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/mediapipe_face/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6870 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2992 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/api.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/blocks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/dpt_depth.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/midas_net.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/midas_net_custom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2314 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    24134 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2662 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      597 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/NNET.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:17.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2980 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/baseline.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:28.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10480 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/decoder.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:38.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2428 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5993 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       89 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3000 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3113 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9187 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4760 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2690 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2294 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4549 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3350 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12093 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    26514 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    59925 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2833 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15009 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      707 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       22 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2730 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5821 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2932 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      843 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4905 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1737 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6632 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1060 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5703 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/submodules.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:29.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7570 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/losses.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6725 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5563 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10883 2023-04-14 09:59:01.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/body.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15314 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/face.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6530 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/hand.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7934 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/pidi/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2978 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/pidi/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    21794 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/pidi/model.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2502 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15148 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2941 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/build_sam.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      385 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1479 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/common.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14420 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6615 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8594 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7226 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/sam.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8397 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/transformer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11664 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/predictor.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      197 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12712 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/amg.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5812 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/onnx.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3972 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/transforms.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/shuffle/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3468 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/shuffle/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3890 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2192 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15248 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    13757 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6909 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3436 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1045 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      333 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      931 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1576 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7284 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6899 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12792 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6099 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8552 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2390 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/builder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7362 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1153 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8693 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4838 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6733 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4163 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3438 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/model_io.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1270 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1587 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      556 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12630 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1276 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1968 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16363 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      624 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16310 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/config.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/easydict/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3426 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3250 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8351 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      120 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11357 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/LICENSE.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3287 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2336 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/README.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8777 2023-05-26 09:47:39.000000 controlnet_aux-0.0.5/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.937408 controlnet_aux-0.0.5/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      515 2023-05-26 09:47:55.000000 controlnet_aux-0.0.5/src/controlnet_aux/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/canny/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      547 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/canny/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/hed/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7994 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/hed/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/lineart/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5293 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/lineart/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/lineart_anime/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7718 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/lineart_anime/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      645 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7118 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2992 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/api.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/blocks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/dpt_depth.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/midas_net.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2314 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    24134 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2662 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      597 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/NNET.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:17.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2980 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/baseline.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:28.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10480 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/decoder.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:38.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2428 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5993 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       89 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3000 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3113 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9187 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4760 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2690 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2294 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4549 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3350 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12093 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    26514 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    59925 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2833 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15009 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      707 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       22 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2730 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5821 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2932 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      843 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4905 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1737 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6632 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1060 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5703 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/submodules.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:29.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7570 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/losses.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6725 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6199 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10837 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/body.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15271 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/face.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6484 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/hand.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7934 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/pidi/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2978 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/pidi/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    21794 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/pidi/model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4430 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/processor.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2502 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15148 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2941 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/build_sam.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      385 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1479 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/common.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14420 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6615 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8594 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7226 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/sam.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8397 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11664 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/predictor.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      197 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12712 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/amg.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5812 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/onnx.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3972 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/transforms.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/shuffle/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3468 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/shuffle/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3890 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2192 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15248 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    13757 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6909 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3436 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1045 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      333 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      931 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1576 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7284 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6899 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12792 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6099 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8552 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2390 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/builder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7362 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1153 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8693 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4838 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6733 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4163 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3438 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/model_io.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1270 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1587 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      556 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12630 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1276 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1968 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    16363 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      624 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    16310 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/config.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/easydict/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3426 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3287 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8383 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      120 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/top_level.txt
```

### Comparing `controlnet_aux-0.0.4/LICENSE.txt` & `controlnet_aux-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/PKG-INFO` & `controlnet_aux-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: controlnet_aux
-Version: 0.0.4
-Summary: Human Pose
+Version: 0.0.5
+Summary: Auxillary models for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
 All credit & copyright goes to https://github.com/lllyasviel .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.3
+pip install controlnet-aux==0.0.4
 ```
 
 ## Usage
 
 ```python
 from PIL import Image
 import requests
@@ -57,15 +57,15 @@
 mlsd = MLSDdetector.from_pretrained("lllyasviel/Annotators")
 open_pose = OpenposeDetector.from_pretrained("lllyasviel/Annotators")
 pidi = PidiNetDetector.from_pretrained("lllyasviel/Annotators")
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
 zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
-sam = SamDetector("./weight_path")
+sam = SamDetector.from_pretrained("./weight_path")
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
 face_detector = MediapipeFaceDetector()
```

### Comparing `controlnet_aux-0.0.4/README.md` & `controlnet_aux-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
 All credit & copyright goes to https://github.com/lllyasviel .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.3
+pip install controlnet-aux==0.0.4
 ```
 
 ## Usage
 
 ```python
 from PIL import Image
 import requests
@@ -32,15 +32,15 @@
 mlsd = MLSDdetector.from_pretrained("lllyasviel/Annotators")
 open_pose = OpenposeDetector.from_pretrained("lllyasviel/Annotators")
 pidi = PidiNetDetector.from_pretrained("lllyasviel/Annotators")
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
 zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
-sam = SamDetector("./weight_path")
+sam = SamDetector.from_pretrained("./weight_path")
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
 face_detector = MediapipeFaceDetector()
```

### Comparing `controlnet_aux-0.0.4/setup.py` & `controlnet_aux-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,16 +177,16 @@
     deps["torchvision"],
     deps["timm"],
     deps["scikit-image"],
 ]
 
 setup(
     name="controlnet_aux",
-    version="0.0.4",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
-    description="Human Pose",
+    version="0.0.5",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    description="Auxillary models for controlnet",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
     url="https://github.com/patrickvonplaten/controlnet_aux",
```

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 from .hed import HEDdetector
 from .midas import MidasDetector
 from .mlsd import MLSDdetector
 from .open_pose import OpenposeDetector
 from .pidi import PidiNetDetector
 from .normalbae import NormalBaeDetector
```

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/canny/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/canny/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/hed/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/lineart/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/lineart/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/lineart_anime/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/lineart_anime/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/mediapipe_face/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py` & `controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 from typing import Mapping
+import warnings
 
 try:
     import mediapipe as mp
 except ImportError:
-    raise ImportError("The module 'mediapipe' is not installed. Please install it using the command: pip install 'mediapipe'")
+    warnings.warn(
+        "The module 'mediapipe' is not installed. The package will have limited functionality. Please install it using the command: pip install 'mediapipe'"
+    )
 
-import numpy
+    mp = None
 
+import numpy
 
-mp_drawing = mp.solutions.drawing_utils
-mp_drawing_styles = mp.solutions.drawing_styles
-mp_face_detection = mp.solutions.face_detection  # Only for counting faces.
-mp_face_mesh = mp.solutions.face_mesh
-mp_face_connections = mp.solutions.face_mesh_connections.FACEMESH_TESSELATION
-mp_hand_connections = mp.solutions.hands_connections.HAND_CONNECTIONS
-mp_body_connections = mp.solutions.pose_connections.POSE_CONNECTIONS
-
-DrawingSpec = mp.solutions.drawing_styles.DrawingSpec
-PoseLandmark = mp.solutions.drawing_styles.PoseLandmark
-
-min_face_size_pixels: int = 64
-f_thick = 2
-f_rad = 1
-right_iris_draw = DrawingSpec(color=(10, 200, 250), thickness=f_thick, circle_radius=f_rad)
-right_eye_draw = DrawingSpec(color=(10, 200, 180), thickness=f_thick, circle_radius=f_rad)
-right_eyebrow_draw = DrawingSpec(color=(10, 220, 180), thickness=f_thick, circle_radius=f_rad)
-left_iris_draw = DrawingSpec(color=(250, 200, 10), thickness=f_thick, circle_radius=f_rad)
-left_eye_draw = DrawingSpec(color=(180, 200, 10), thickness=f_thick, circle_radius=f_rad)
-left_eyebrow_draw = DrawingSpec(color=(180, 220, 10), thickness=f_thick, circle_radius=f_rad)
-mouth_draw = DrawingSpec(color=(10, 180, 10), thickness=f_thick, circle_radius=f_rad)
-head_draw = DrawingSpec(color=(10, 200, 10), thickness=f_thick, circle_radius=f_rad)
-
-# mp_face_mesh.FACEMESH_CONTOURS has all the items we care about.
-face_connection_spec = {}
-for edge in mp_face_mesh.FACEMESH_FACE_OVAL:
-    face_connection_spec[edge] = head_draw
-for edge in mp_face_mesh.FACEMESH_LEFT_EYE:
-    face_connection_spec[edge] = left_eye_draw
-for edge in mp_face_mesh.FACEMESH_LEFT_EYEBROW:
-    face_connection_spec[edge] = left_eyebrow_draw
-# for edge in mp_face_mesh.FACEMESH_LEFT_IRIS:
-#    face_connection_spec[edge] = left_iris_draw
-for edge in mp_face_mesh.FACEMESH_RIGHT_EYE:
-    face_connection_spec[edge] = right_eye_draw
-for edge in mp_face_mesh.FACEMESH_RIGHT_EYEBROW:
-    face_connection_spec[edge] = right_eyebrow_draw
-# for edge in mp_face_mesh.FACEMESH_RIGHT_IRIS:
-#    face_connection_spec[edge] = right_iris_draw
-for edge in mp_face_mesh.FACEMESH_LIPS:
-    face_connection_spec[edge] = mouth_draw
-iris_landmark_spec = {468: right_iris_draw, 473: left_iris_draw}
+if mp:
+    mp_drawing = mp.solutions.drawing_utils
+    mp_drawing_styles = mp.solutions.drawing_styles
+    mp_face_detection = mp.solutions.face_detection  # Only for counting faces.
+    mp_face_mesh = mp.solutions.face_mesh
+    mp_face_connections = mp.solutions.face_mesh_connections.FACEMESH_TESSELATION
+    mp_hand_connections = mp.solutions.hands_connections.HAND_CONNECTIONS
+    mp_body_connections = mp.solutions.pose_connections.POSE_CONNECTIONS
+
+    DrawingSpec = mp.solutions.drawing_styles.DrawingSpec
+    PoseLandmark = mp.solutions.drawing_styles.PoseLandmark
+
+    min_face_size_pixels: int = 64
+    f_thick = 2
+    f_rad = 1
+    right_iris_draw = DrawingSpec(color=(10, 200, 250), thickness=f_thick, circle_radius=f_rad)
+    right_eye_draw = DrawingSpec(color=(10, 200, 180), thickness=f_thick, circle_radius=f_rad)
+    right_eyebrow_draw = DrawingSpec(color=(10, 220, 180), thickness=f_thick, circle_radius=f_rad)
+    left_iris_draw = DrawingSpec(color=(250, 200, 10), thickness=f_thick, circle_radius=f_rad)
+    left_eye_draw = DrawingSpec(color=(180, 200, 10), thickness=f_thick, circle_radius=f_rad)
+    left_eyebrow_draw = DrawingSpec(color=(180, 220, 10), thickness=f_thick, circle_radius=f_rad)
+    mouth_draw = DrawingSpec(color=(10, 180, 10), thickness=f_thick, circle_radius=f_rad)
+    head_draw = DrawingSpec(color=(10, 200, 10), thickness=f_thick, circle_radius=f_rad)
+
+    # mp_face_mesh.FACEMESH_CONTOURS has all the items we care about.
+    face_connection_spec = {}
+    for edge in mp_face_mesh.FACEMESH_FACE_OVAL:
+        face_connection_spec[edge] = head_draw
+    for edge in mp_face_mesh.FACEMESH_LEFT_EYE:
+        face_connection_spec[edge] = left_eye_draw
+    for edge in mp_face_mesh.FACEMESH_LEFT_EYEBROW:
+        face_connection_spec[edge] = left_eyebrow_draw
+    # for edge in mp_face_mesh.FACEMESH_LEFT_IRIS:
+    #    face_connection_spec[edge] = left_iris_draw
+    for edge in mp_face_mesh.FACEMESH_RIGHT_EYE:
+        face_connection_spec[edge] = right_eye_draw
+    for edge in mp_face_mesh.FACEMESH_RIGHT_EYEBROW:
+        face_connection_spec[edge] = right_eyebrow_draw
+    # for edge in mp_face_mesh.FACEMESH_RIGHT_IRIS:
+    #    face_connection_spec[edge] = right_iris_draw
+    for edge in mp_face_mesh.FACEMESH_LIPS:
+        face_connection_spec[edge] = mouth_draw
+    iris_landmark_spec = {468: right_iris_draw, 473: left_iris_draw}
 
 
 def draw_pupils(image, landmark_list, drawing_spec, halfwidth: int = 2):
     """We have a custom function to draw the pupils because the mp.draw_landmarks method requires a parameter for all
     landmarks.  Until our PR is merged into mediapipe, we need this separate method."""
     if len(image.shape) != 3:
         raise ValueError("Input image must be H,W,C.")
```

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/api.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/blocks.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/dpt_depth.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/midas_net.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/midas_net_custom.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/transforms.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/vit.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/midas/utils.py` & `controlnet_aux-0.0.5/src/controlnet_aux/midas/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/mlsd/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/mlsd/utils.py` & `controlnet_aux-0.0.5/src/controlnet_aux/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/NNET.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/NNET.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/baseline.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/baseline.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/decoder.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/encoder.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/submodules.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/submodules.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/losses.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/losses.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/utils.py` & `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
+import warnings
 
 import torch
 import cv2
 import numpy as np
 from PIL import Image
 from .util import HWC3, resize_image, draw_bodypose, draw_handpose, draw_facepose
 from .body import Body
@@ -41,15 +42,15 @@
 class OpenposeDetector:
     def __init__(self, body_estimation, hand_estimation=None, face_estimation=None):
         self.body_estimation = body_estimation
         self.hand_estimation = hand_estimation
         self.face_estimation = face_estimation
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, hand_filename=None, face_filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, device=None, filename=None, hand_filename=None, face_filename=None, cache_dir=None):
 
         if pretrained_model_or_path == "lllyasviel/ControlNet":
             filename = filename or "annotator/ckpts/body_pose_model.pth"
             hand_filename = hand_filename or "annotator/ckpts/hand_pose_model.pth"
             face_filename = face_filename or "facenet.pth"
 
             face_pretrained_model_or_path = "lllyasviel/Annotators"
@@ -65,42 +66,56 @@
             hand_model_path = os.path.join(pretrained_model_or_path, hand_filename)
             face_model_path = os.path.join(face_pretrained_model_or_path, face_filename)
         else:
             body_model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
             hand_model_path = hf_hub_download(pretrained_model_or_path, hand_filename, cache_dir=cache_dir)
             face_model_path = hf_hub_download(face_pretrained_model_or_path, face_filename, cache_dir=cache_dir)
 
-        body_estimation = Body(body_model_path)
-        hand_estimation = Hand(hand_model_path)
-        face_estimation = Face(face_model_path)
+        if device is None:
+            if torch.cuda.is_available():
+                device = 'cuda'
+            elif torch.backends.mps.is_available():
+                device = 'mps'
+            else:
+                device = 'cpu'
+
+        body_estimation = Body(body_model_path, device)
+        hand_estimation = Hand(hand_model_path, device)
+        face_estimation = Face(face_model_path, device)
 
         return cls(body_estimation, hand_estimation, face_estimation)
 
-    def __call__(self, input_image, detect_resolution=512, image_resolution=512, hand_and_face=False, return_pil=True):
-        # hand = False
+
+    def __call__(self, input_image, detect_resolution=512, image_resolution=512, include_body=True, include_hand=False, include_face=False, hand_and_face=False, return_pil=True):
+        if hand_and_face:
+            warnings.warn("hand_and_face is deprecated. Use include_hand and include_face instead.", DeprecationWarning)
+            include_hand = True
+            include_face = True
+
         if not isinstance(input_image, np.ndarray):
             input_image = np.array(input_image, dtype=np.uint8)
 
         input_image = HWC3(input_image)
         input_image = resize_image(input_image, detect_resolution)
         input_image = input_image[:, :, ::-1].copy()
         H, W, C = input_image.shape
         with torch.no_grad():
             candidate, subset = self.body_estimation(input_image)
             hands = []
             faces = []
-            if hand_and_face:
+            if include_hand:
                 # Hand
                 hands_list = handDetect(candidate, subset, input_image)
                 for x, y, w, is_left in hands_list:
                     peaks = self.hand_estimation(input_image[y:y+w, x:x+w, :]).astype(np.float32)
                     if peaks.ndim == 2 and peaks.shape[1] == 2:
                         peaks[:, 0] = np.where(peaks[:, 0] < 1e-6, -1, peaks[:, 0] + x) / float(W)
                         peaks[:, 1] = np.where(peaks[:, 1] < 1e-6, -1, peaks[:, 1] + y) / float(H)
                         hands.append(peaks.tolist())
+            if include_face:
                 # Face
                 faces_list = faceDetect(candidate, subset, input_image)
                 for x, y, w in faces_list:
                     heatmaps = self.face_estimation(input_image[y:y+w, x:x+w, :])
                     peaks = self.face_estimation.compute_peaks_from_heatmaps(heatmaps).astype(np.float32)
                     if peaks.ndim == 2 and peaks.shape[1] == 2:
                         peaks[:, 0] = np.where(peaks[:, 0] < 1e-6, -1, peaks[:, 0] + x) / float(W)
@@ -111,15 +126,15 @@
                 candidate = candidate[:, :2]
                 candidate[:, 0] /= float(W)
                 candidate[:, 1] /= float(H)
 
             bodies = dict(candidate=candidate.tolist(), subset=subset.tolist())
             pose = dict(bodies=bodies, hands=hands, faces=faces)
 
-            canvas = draw_pose(pose, H, W)
+            canvas = draw_pose(pose, H, W, draw_body=include_body, draw_hand=include_hand, draw_face=include_face)
 
         detected_map = HWC3(canvas)
         img = resize_image(input_image, image_resolution)
         H, W, C = img.shape
 
         detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_NEAREST)
```

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/body.py` & `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/body.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from scipy.ndimage.filters import gaussian_filter
 import torch
 
 from . import util
 from .model import bodypose_model
 
 class Body(object):
-    def __init__(self, model_path):
+    def __init__(self, model_path, device):
+        self.device = device
         self.model = bodypose_model()
-        if torch.cuda.is_available():
-            self.model = self.model.cuda()
         model_dict = util.transfer(self.model, torch.load(model_path))
         self.model.load_state_dict(model_dict)
+        self.model.to(self.device)
         self.model.eval()
 
     def __call__(self, oriImg):
         # scale_search = [0.5, 1.0, 1.5, 2.0]
         scale_search = [0.5]
         boxsize = 368
         stride = 8
@@ -33,16 +33,15 @@
             scale = multiplier[m]
             imageToTest = cv2.resize(oriImg, (0, 0), fx=scale, fy=scale, interpolation=cv2.INTER_CUBIC)
             imageToTest_padded, pad = util.padRightDownCorner(imageToTest, stride, padValue)
             im = np.transpose(np.float32(imageToTest_padded[:, :, :, np.newaxis]), (3, 2, 0, 1)) / 256 - 0.5
             im = np.ascontiguousarray(im)
 
             data = torch.from_numpy(im).float()
-            if torch.cuda.is_available():
-                data = data.cuda()
+            data = data.to(self.device)
             # data = data.permute([2, 0, 1]).unsqueeze(0).float()
             with torch.no_grad():
                 Mconv7_stage6_L1, Mconv7_stage6_L2 = self.model(data)
             Mconv7_stage6_L1 = Mconv7_stage6_L1.cpu().numpy()
             Mconv7_stage6_L2 = Mconv7_stage6_L2.cpu().numpy()
 
             # extract outputs, resize, and remove padding
```

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/face.py` & `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/face.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,35 +310,33 @@
     Args:
         inference_size: set the size of the inference image size, suggested:
             368, 736, 1312, default 736
         gaussian_sigma: blur the heatmaps, default 2.5
         heatmap_peak_thresh: return landmark if over threshold, default 0.1
 
     """
-    def __init__(self, face_model_path,
+    def __init__(self, face_model_path, device,
                  inference_size=None,
                  gaussian_sigma=None,
                  heatmap_peak_thresh=None):
+        self.device = device
         self.inference_size = inference_size or params["inference_img_size"]
         self.sigma = gaussian_sigma or params['gaussian_sigma']
         self.threshold = heatmap_peak_thresh or params["heatmap_peak_thresh"]
         self.model = FaceNet()
         self.model.load_state_dict(torch.load(face_model_path))
-        if torch.cuda.is_available():
-            self.model = self.model.cuda()
+        self.model.to(self.device)
         self.model.eval()
 
     def __call__(self, face_img):
         H, W, C = face_img.shape
 
         w_size = 384
         x_data = torch.from_numpy(util.smart_resize(face_img, (w_size, w_size))).permute([2, 0, 1]) / 256.0 - 0.5
-
-        if torch.cuda.is_available():
-            x_data = x_data.cuda()
+        x_data = x_data.to(self.device)
 
         with torch.no_grad():
             hs = self.model(x_data[None, ...])
             heatmaps = F.interpolate(
                 hs[-1],
                 (H, W),
                 mode='bilinear', align_corners=True).cpu().numpy()[0]
```

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/hand.py` & `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/hand.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import torch
 from skimage.measure import label
 
 from .model import handpose_model
 from . import util
 
 class Hand(object):
-    def __init__(self, model_path):
+    def __init__(self, model_path, device):
+        self.device = device
         self.model = handpose_model()
-        if torch.cuda.is_available():
-            self.model = self.model.cuda()
         model_dict = util.transfer(self.model, torch.load(model_path))
         self.model.load_state_dict(model_dict)
+        self.model.to(self.device)
         self.model.eval()
 
     def __call__(self, oriImg):
         scale_search = [0.5, 1.0, 1.5, 2.0]
         # scale_search = [0.5]
         boxsize = 368
         stride = 8
@@ -34,16 +34,15 @@
             scale = multiplier[m]
             imageToTest = cv2.resize(oriImg, (0, 0), fx=scale, fy=scale, interpolation=cv2.INTER_CUBIC)
             imageToTest_padded, pad = util.padRightDownCorner(imageToTest, stride, padValue)
             im = np.transpose(np.float32(imageToTest_padded[:, :, :, np.newaxis]), (3, 2, 0, 1)) / 256 - 0.5
             im = np.ascontiguousarray(im)
 
             data = torch.from_numpy(im).float()
-            if torch.cuda.is_available():
-                data = data.cuda()
+            data = data.to(self.device)
             # data = data.permute([2, 0, 1]).unsqueeze(0).float()
             with torch.no_grad():
                 output = self.model(data).cpu().numpy()
                 # output = self.model(data).numpy()q
 
             # extract outputs, resize, and remove padding
             heatmap = np.transpose(np.squeeze(output), (1, 2, 0))  # output 1 is heatmaps
```

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/model.py` & `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/util.py` & `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/pidi/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/pidi/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/pidi/model.py` & `controlnet_aux-0.0.5/src/controlnet_aux/pidi/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/automatic_mask_generator.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/build_sam.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/common.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/image_encoder.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/mask_decoder.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/sam.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/transformer.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/predictor.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/amg.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/onnx.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/transforms.py` & `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/shuffle/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/util.py` & `controlnet_aux-0.0.5/src/controlnet_aux/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/builder.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/depth_model.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/depth_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/model_io.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/model_io.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/config.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py` & `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux.egg-info/PKG-INFO` & `controlnet_aux-0.0.5/src/controlnet_aux.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: controlnet-aux
-Version: 0.0.4
-Summary: Human Pose
+Version: 0.0.5
+Summary: Auxillary models for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
 All credit & copyright goes to https://github.com/lllyasviel .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.3
+pip install controlnet-aux==0.0.4
 ```
 
 ## Usage
 
 ```python
 from PIL import Image
 import requests
@@ -57,15 +57,15 @@
 mlsd = MLSDdetector.from_pretrained("lllyasviel/Annotators")
 open_pose = OpenposeDetector.from_pretrained("lllyasviel/Annotators")
 pidi = PidiNetDetector.from_pretrained("lllyasviel/Annotators")
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
 zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
-sam = SamDetector("./weight_path")
+sam = SamDetector.from_pretrained("./weight_path")
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
 face_detector = MediapipeFaceDetector()
```

### Comparing `controlnet_aux-0.0.4/src/controlnet_aux.egg-info/SOURCES.txt` & `controlnet_aux-0.0.5/src/controlnet_aux.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 README.md
 setup.py
 src/controlnet_aux/__init__.py
+src/controlnet_aux/processor.py
 src/controlnet_aux/util.py
 src/controlnet_aux.egg-info/PKG-INFO
 src/controlnet_aux.egg-info/SOURCES.txt
 src/controlnet_aux.egg-info/dependency_links.txt
 src/controlnet_aux.egg-info/requires.txt
 src/controlnet_aux.egg-info/top_level.txt
 src/controlnet_aux/canny/__init__.py
```


# Comparing `tmp/innerverz-0.0.14.tar.gz` & `tmp/innerverz-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.14.tar", last modified: Fri May 26 06:32:58 2023, max compression
+gzip compressed data, was "innerverz-0.0.15.tar", last modified: Fri May 26 07:20:56 2023, max compression
```

## Comparing `innerverz-0.0.14.tar` & `innerverz-0.0.15.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1073 2023-05-26 05:00:26.000000 innerverz-0.0.14/LICENSE.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-26 06:32:58.400369 innerverz-0.0.14/PKG-INFO
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       10 2023-05-26 05:00:26.000000 innerverz-0.0.14/README.md
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      383 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/__init__.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/data_process/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/data_process/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3459 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/data_process/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/deblurrer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deblurrer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2171 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deblurrer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3609 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deblurrer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      867 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deblurrer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/deca/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       23 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    16976 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/deca/models/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12616 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/models/FLAME.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/models/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2464 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/models/decoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/models/detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1427 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/models/encoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/models/face_detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    13786 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/models/lbs.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8386 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/models/resnet.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1126 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/deca/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5036 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/utils/cfg.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/deca/utils/rasterizer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/utils/rasterizer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      706 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/utils/rasterizer/setup.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    22281 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/utils/renderer.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12710 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/utils/rotation_converter.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5574 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/utils/tensor_cropper.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    26962 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deca/utils/util.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/deep3dmm/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deep3dmm/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3414 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deep3dmm/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    25860 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deep3dmm/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      651 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/deep3dmm/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/face_alignment/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      125 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6646 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/graphic_utils.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5089 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/landmark.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9365 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12774 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/retina_face.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      656 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/face_alignment/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       24 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3354 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/utils/face_align.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4933 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_alignment/utils/transform.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/face_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5238 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8503 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2047 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/face_enhancer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_enhancer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3745 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_enhancer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4079 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_enhancer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      792 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_enhancer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/face_parser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_parser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2682 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_parser/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    11822 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_parser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      713 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/face_parser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/head_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5409 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8742 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1997 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/head_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/id_extractor/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       29 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/id_extractor/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2217 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/id_extractor/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5192 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/id_extractor/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      717 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/id_extractor/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/relighter/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/relighter/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2912 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/relighter/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4546 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/relighter/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3078 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/relighter/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/upsampler/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/upsampler/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2250 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/upsampler/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    36818 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/upsampler/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      854 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/upsampler/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      109 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1438 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/utils/download.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1009 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/utils/input.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    15902 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/utils/utils.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/video_faceparser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       34 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6039 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/video_faceparser/model/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       79 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/model/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4009 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      217 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.400369 innerverz-0.0.14/innerverz/video_faceparser/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       94 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3079 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/utils/corr.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8847 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/utils/extractor.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3984 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/utils/update.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6502 2023-05-26 05:00:27.000000 innerverz-0.0.14/innerverz/video_faceparser/utils/util.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 06:32:58.396369 innerverz-0.0.14/innerverz.egg-info/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-26 06:32:58.000000 innerverz-0.0.14/innerverz.egg-info/PKG-INFO
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3484 2023-05-26 06:32:58.000000 innerverz-0.0.14/innerverz.egg-info/SOURCES.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        1 2023-05-26 06:32:58.000000 innerverz-0.0.14/innerverz.egg-info/dependency_links.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       50 2023-05-26 06:32:58.000000 innerverz-0.0.14/innerverz.egg-info/requires.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       10 2023-05-26 06:32:58.000000 innerverz-0.0.14/innerverz.egg-info/top_level.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       89 2023-05-26 05:00:26.000000 innerverz-0.0.14/pyproject.toml
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       38 2023-05-26 06:32:58.400369 innerverz-0.0.14/setup.cfg
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      770 2023-05-26 06:32:49.000000 innerverz-0.0.14/setup.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1073 2023-05-26 05:00:26.000000 innerverz-0.0.15/LICENSE.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-26 07:20:56.964547 innerverz-0.0.15/PKG-INFO
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       10 2023-05-26 05:00:26.000000 innerverz-0.0.15/README.md
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1417 2023-05-26 07:19:35.000000 innerverz-0.0.15/innerverz/__init__.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/data_process/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 07:19:35.000000 innerverz-0.0.15/innerverz/data_process/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3459 2023-05-26 07:19:35.000000 innerverz-0.0.15/innerverz/data_process/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/deblurrer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:35.000000 innerverz-0.0.15/innerverz/deblurrer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2171 2023-05-26 07:19:35.000000 innerverz-0.0.15/innerverz/deblurrer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3609 2023-05-26 07:19:35.000000 innerverz-0.0.15/innerverz/deblurrer/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      867 2023-05-26 07:19:35.000000 innerverz-0.0.15/innerverz/deblurrer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/deca/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       23 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    16976 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/deca/models/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12616 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/models/FLAME.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/models/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2464 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/models/decoders.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/models/detectors.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1427 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/models/encoders.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/models/face_detectors.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    13786 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/models/lbs.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8386 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/models/resnet.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1126 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/deca/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5036 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/utils/cfg.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/deca/utils/rasterizer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/utils/rasterizer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      706 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/utils/rasterizer/setup.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    22281 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/utils/renderer.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12710 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/utils/rotation_converter.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5574 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/utils/tensor_cropper.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    26962 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deca/utils/util.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/deep3dmm/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deep3dmm/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3414 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deep3dmm/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    25860 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deep3dmm/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      651 2023-05-26 07:19:36.000000 innerverz-0.0.15/innerverz/deep3dmm/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/face_alignment/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      125 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6646 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/graphic_utils.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5089 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/landmark.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9365 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12774 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/retina_face.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      656 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz/face_alignment/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       24 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3354 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/utils/face_align.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4933 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_alignment/utils/transform.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/face_color_transfer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5238 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8503 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/nets.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2047 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_color_transfer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/face_enhancer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_enhancer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3745 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_enhancer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4079 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_enhancer/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      792 2023-05-26 07:19:37.000000 innerverz-0.0.15/innerverz/face_enhancer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/face_parser/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/face_parser/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2682 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/face_parser/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    11822 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/face_parser/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      713 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/face_parser/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/head_color_transfer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5409 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8742 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/nets.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1997 2023-05-26 07:19:38.000000 innerverz-0.0.15/innerverz/head_color_transfer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/id_extractor/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       29 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/id_extractor/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2253 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/id_extractor/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5192 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/id_extractor/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      717 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/id_extractor/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/relighter/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/relighter/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2912 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/relighter/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4546 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/relighter/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3078 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/relighter/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/upsampler/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/upsampler/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2250 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/upsampler/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    36818 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/upsampler/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      854 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/upsampler/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      109 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1438 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/utils/download.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1009 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/utils/input.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    15902 2023-05-26 07:19:39.000000 innerverz-0.0.15/innerverz/utils/utils.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/video_faceparser/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       34 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6039 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/video_faceparser/model/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       79 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/model/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4009 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      217 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.964547 innerverz-0.0.15/innerverz/video_faceparser/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       94 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3079 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/utils/corr.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8847 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/utils/extractor.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3984 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/utils/update.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6502 2023-05-26 07:19:40.000000 innerverz-0.0.15/innerverz/video_faceparser/utils/util.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:20:56.960548 innerverz-0.0.15/innerverz.egg-info/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-26 07:20:56.000000 innerverz-0.0.15/innerverz.egg-info/PKG-INFO
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3484 2023-05-26 07:20:56.000000 innerverz-0.0.15/innerverz.egg-info/SOURCES.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        1 2023-05-26 07:20:56.000000 innerverz-0.0.15/innerverz.egg-info/dependency_links.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       50 2023-05-26 07:20:56.000000 innerverz-0.0.15/innerverz.egg-info/requires.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       10 2023-05-26 07:20:56.000000 innerverz-0.0.15/innerverz.egg-info/top_level.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       89 2023-05-26 05:00:26.000000 innerverz-0.0.15/pyproject.toml
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       38 2023-05-26 07:20:56.964547 innerverz-0.0.15/setup.cfg
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      770 2023-05-26 07:20:48.000000 innerverz-0.0.15/setup.py
```

### Comparing `innerverz-0.0.14/LICENSE.txt` & `innerverz-0.0.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/data_process/main.py` & `innerverz-0.0.15/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deblurrer/main.py` & `innerverz-0.0.15/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deblurrer/nets.py` & `innerverz-0.0.15/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deblurrer/test.py` & `innerverz-0.0.15/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/main.py` & `innerverz-0.0.15/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/models/FLAME.py` & `innerverz-0.0.15/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/models/decoders.py` & `innerverz-0.0.15/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/models/detectors.py` & `innerverz-0.0.15/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/models/encoders.py` & `innerverz-0.0.15/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/models/face_detectors.py` & `innerverz-0.0.15/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/models/lbs.py` & `innerverz-0.0.15/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/models/resnet.py` & `innerverz-0.0.15/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/test.py` & `innerverz-0.0.15/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/utils/cfg.py` & `innerverz-0.0.15/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.0.15/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/utils/renderer.py` & `innerverz-0.0.15/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.0.15/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.0.15/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deca/utils/util.py` & `innerverz-0.0.15/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deep3dmm/main.py` & `innerverz-0.0.15/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deep3dmm/nets.py` & `innerverz-0.0.15/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/deep3dmm/test.py` & `innerverz-0.0.15/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.0.15/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_alignment/landmark.py` & `innerverz-0.0.15/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_alignment/main.py` & `innerverz-0.0.15/innerverz/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_alignment/retina_face.py` & `innerverz-0.0.15/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_alignment/test.py` & `innerverz-0.0.15/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.0.15/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_alignment/utils/transform.py` & `innerverz-0.0.15/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_color_transfer/main.py` & `innerverz-0.0.15/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_color_transfer/nets.py` & `innerverz-0.0.15/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.15/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_color_transfer/test.py` & `innerverz-0.0.15/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_enhancer/main.py` & `innerverz-0.0.15/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_enhancer/nets.py` & `innerverz-0.0.15/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_enhancer/test.py` & `innerverz-0.0.15/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_parser/main.py` & `innerverz-0.0.15/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_parser/nets.py` & `innerverz-0.0.15/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/face_parser/test.py` & `innerverz-0.0.15/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/head_color_transfer/main.py` & `innerverz-0.0.15/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/head_color_transfer/nets.py` & `innerverz-0.0.15/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.15/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/head_color_transfer/test.py` & `innerverz-0.0.15/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/id_extractor/main.py` & `innerverz-0.0.15/innerverz/id_extractor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 import warnings; warnings.filterwarnings('ignore')
 
 from .nets import Backbone
 from ..utils import check_ckpt_exist, get_url_id
 
 class IdExtractor(nn.Module):
-    """
-    Methods
-    --------
-    forward(tesnor_img : tensor) -> id_vector : tensor
-    
-    data_preprocess(img_path : str) -> tensor_img : tensor
-    
-    compare_similarity(id_vector_1 : tensor, id_vector_2 : tensor) -> score : float
-    """
     def __init__(self, x=32, y=32, w=192, h=192 , folder_name='id_extractor', ckpt_name='currface.pth', force=False, device='cuda' ):
+        """
+        Methods
+        --------
+        forward(tesnor_img : tensor) -> id_vector : tensor
+        
+        data_preprocess(img_path : str) -> tensor_img : tensor
+        
+        compare_similarity(id_vector_1 : tensor, id_vector_2 : tensor) -> score : float
+        """
         super(IdExtractor, self).__init__()
         self.device = device
         self.id_extractor = Backbone().to(self.device).eval()
         url_id = get_url_id('~/.invz_pack/', folder_name, ckpt_name)
         root = os.path.join('~/.invz_pack/', folder_name)
         ckpt_path = check_ckpt_exist(root, ckpt_name = ckpt_name, url_id = url_id, force = force)
         ckpt = torch.load(ckpt_path, map_location=self.device)
```

### Comparing `innerverz-0.0.14/innerverz/id_extractor/nets.py` & `innerverz-0.0.15/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/id_extractor/test.py` & `innerverz-0.0.15/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/relighter/main.py` & `innerverz-0.0.15/innerverz/relighter/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,36 +10,14 @@
 from .nets import MyGenerator
 
 from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
 from ..utils import check_ckpt_exist, get_url_id
 
 class ReLighter(nn.Module):
     def __init__(self, folder_name='relighter', ckpt_name = 'G_129k.pt', force=False, device = 'cuda'):
-        super(ReLighter, self).__init__()
-        self.device = device
-        
-        self.img_size = 512
-        self.generator = MyGenerator().to(self.device)
-
-        url_id = get_url_id('~/.invz_pack/', folder_name, ckpt_name)
-        root = os.path.join('~/.invz_pack/', folder_name)
-        ckpt_path = check_ckpt_exist(root, ckpt_name = ckpt_name, url_id = url_id, force = force)
-        
-        ckpt = torch.load(os.path.join(ckpt_path), map_location=self.device)
-        self.generator.load_state_dict(ckpt['model'])
-        for param in self.generator.parameters():
-            param.requires_grad = False
-        self.generator.eval()
-        del ckpt
-
-    def relight(self,):
-        return
-
-    # source light -> target light
-    def forward(self, masked_gray_face, relight_detail_shape, code_dict, id_param, output_size=None):
         """
         Input
         --------
         - masked_gray_face
             - dtype : tensor
             - shape : (b, 1, 512, 512)
             - min max (-1 1)
@@ -59,14 +37,36 @@
         Output
         --------
         - result
             - dtype : tensor
             - shape : (b, 1 , 512, 512)
             - min max : (-1 1)
         """
+        super(ReLighter, self).__init__()
+        self.device = device
+        
+        self.img_size = 512
+        self.generator = MyGenerator().to(self.device)
+
+        url_id = get_url_id('~/.invz_pack/', folder_name, ckpt_name)
+        root = os.path.join('~/.invz_pack/', folder_name)
+        ckpt_path = check_ckpt_exist(root, ckpt_name = ckpt_name, url_id = url_id, force = force)
+        
+        ckpt = torch.load(os.path.join(ckpt_path), map_location=self.device)
+        self.generator.load_state_dict(ckpt['model'])
+        for param in self.generator.parameters():
+            param.requires_grad = False
+        self.generator.eval()
+        del ckpt
+
+    def relight(self,):
+        return
+
+    # source light -> target light
+    def forward(self, masked_gray_face, relight_detail_shape, code_dict, id_param, output_size=None):
         _, _, origin_h, origin_w = masked_gray_face.shape
         
         masked_gray_face = F.interpolate(masked_gray_face, (self.img_size, self.img_size), mode='bilinear')
         relight_detail_shape = F.interpolate(relight_detail_shape, (self.img_size, self.img_size), mode='bilinear')
         
         params = torch.cat((code_dict['light'].view(1, -1), code_dict['cam'].view(1, -1), code_dict['pose'].view(1, -1), code_dict['detail'].view(1, -1), id_param), dim=-1)
         res = self.generator(masked_gray_face, relight_detail_shape, params)
```

### Comparing `innerverz-0.0.14/innerverz/relighter/nets.py` & `innerverz-0.0.15/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/relighter/test.py` & `innerverz-0.0.15/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/upsampler/main.py` & `innerverz-0.0.15/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/upsampler/nets.py` & `innerverz-0.0.15/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/upsampler/test.py` & `innerverz-0.0.15/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/utils/download.py` & `innerverz-0.0.15/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/utils/input.py` & `innerverz-0.0.15/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/utils/utils.py` & `innerverz-0.0.15/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/video_faceparser/main.py` & `innerverz-0.0.15/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/video_faceparser/nets.py` & `innerverz-0.0.15/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.0.15/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.0.15/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/video_faceparser/utils/update.py` & `innerverz-0.0.15/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz/video_faceparser/utils/util.py` & `innerverz-0.0.15/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/innerverz.egg-info/SOURCES.txt` & `innerverz-0.0.15/innerverz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.14/setup.py` & `innerverz-0.0.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.14",
+    version="0.0.15",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```


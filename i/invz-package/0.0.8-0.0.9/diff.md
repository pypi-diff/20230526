# Comparing `tmp/invz_package-0.0.8.tar.gz` & `tmp/invz_package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invz_package-0.0.8.tar", last modified: Mon Feb  6 07:37:03 2023, max compression
+gzip compressed data, was "invz_package-0.0.9.tar", last modified: Fri May 26 01:13:36 2023, max compression
```

## Comparing `invz_package-0.0.8.tar` & `invz_package-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,230 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.322880 invz_package-0.0.8/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-01-27 06:12:58.000000 invz_package-0.0.8/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      208 2023-02-06 07:37:03.322696 invz_package-0.0.8/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-01-27 06:13:11.000000 invz_package-0.0.8/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.318098 invz_package-0.0.8/invz_pack/
--rw-r--r--   0 jjy        (501) staff       (20)       62 2023-02-06 04:13:00.000000 invz_package-0.0.8/invz_pack/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.318826 invz_package-0.0.8/invz_pack/face_aligner/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-02-06 04:35:19.000000 invz_package-0.0.8/invz_pack/face_aligner/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1742 2023-02-06 05:53:42.000000 invz_package-0.0.8/invz_pack/face_aligner/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     9875 2023-02-06 04:35:19.000000 invz_package-0.0.8/invz_pack/face_aligner/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.319507 invz_package-0.0.8/invz_pack/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       59 2023-02-06 07:36:02.000000 invz_package-0.0.8/invz_pack/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2252 2023-02-06 07:30:02.000000 invz_package-0.0.8/invz_pack/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8472 2023-02-06 06:01:06.000000 invz_package-0.0.8/invz_pack/face_parser/model.py
--rw-r--r--   0 jjy        (501) staff       (20)     3648 2023-02-06 06:51:08.000000 invz_package-0.0.8/invz_pack/face_parser/resnet.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.319991 invz_package-0.0.8/invz_pack/face_parser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-02-06 06:41:53.000000 invz_package-0.0.8/invz_pack/face_parser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      837 2023-02-06 07:24:32.000000 invz_package-0.0.8/invz_pack/face_parser/utils/mask_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     1509 2023-02-06 07:02:57.000000 invz_package-0.0.8/invz_pack/face_parser/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.320556 invz_package-0.0.8/invz_pack/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-01-28 00:58:54.000000 invz_package-0.0.8/invz_pack/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2219 2023-02-06 06:00:02.000000 invz_package-0.0.8/invz_pack/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-01-27 05:21:47.000000 invz_package-0.0.8/invz_pack/id_extractor/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.320986 invz_package-0.0.8/invz_pack/lmk_detector/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-02-06 04:37:37.000000 invz_package-0.0.8/invz_pack/lmk_detector/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1467 2023-02-06 05:48:27.000000 invz_package-0.0.8/invz_pack/lmk_detector/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.321548 invz_package-0.0.8/invz_pack/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       76 2023-02-06 03:02:55.000000 invz_package-0.0.8/invz_pack/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      819 2023-01-28 01:03:40.000000 invz_package-0.0.8/invz_pack/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1009 2023-02-06 03:04:22.000000 invz_package-0.0.8/invz_pack/utils/input.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-02-06 07:37:03.322463 invz_package-0.0.8/invz_package.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      208 2023-02-06 07:37:03.000000 invz_package-0.0.8/invz_package.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)      834 2023-02-06 07:37:03.000000 invz_package-0.0.8/invz_package.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-02-06 07:37:03.000000 invz_package-0.0.8/invz_package.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       36 2023-02-06 07:37:03.000000 invz_package-0.0.8/invz_package.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-02-06 07:37:03.000000 invz_package-0.0.8/invz_package.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-01-27 04:47:26.000000 invz_package-0.0.8/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-02-06 07:37:03.322944 invz_package-0.0.8/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      758 2023-02-06 07:36:35.000000 invz_package-0.0.8/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.720734 invz_package-0.0.9/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 invz_package-0.0.9/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      208 2023-05-26 01:13:36.720820 invz_package-0.0.9/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 invz_package-0.0.9/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.688645 invz_package-0.0.9/innerverz_package/
+-rw-r--r--   0 jjy        (501) staff       (20)      383 2023-05-25 23:54:06.000000 invz_package-0.0.9/innerverz_package/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.704038 invz_package-0.0.9/innerverz_package/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-05-25 04:27:01.000000 invz_package-0.0.9/innerverz_package/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3352 2023-05-25 06:23:38.000000 invz_package-0.0.9/innerverz_package/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.704602 invz_package-0.0.9/innerverz_package/deblurrer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/deblurrer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2985 2023-05-24 02:40:28.000000 invz_package-0.0.9/innerverz_package/deblurrer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3609 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/deblurrer/nets.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     1072 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.705061 invz_package-0.0.9/innerverz_package/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    16976 2023-05-25 06:56:05.000000 invz_package-0.0.9/innerverz_package/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.707394 invz_package-0.0.9/innerverz_package/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-05-24 06:09:07.000000 invz_package-0.0.9/innerverz_package/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:50.000000 invz_package-0.0.9/innerverz_package/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)      407 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.708870 invz_package-0.0.9/innerverz_package/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 invz_package-0.0.9/innerverz_package/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-05-24 05:33:36.000000 invz_package-0.0.9/innerverz_package/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.709266 invz_package-0.0.9/innerverz_package/deca/utils/rasterizer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 invz_package-0.0.9/innerverz_package/deca/utils/rasterizer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)      706 2023-05-24 04:57:52.000000 invz_package-0.0.9/innerverz_package/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-05-24 04:57:52.000000 invz_package-0.0.9/innerverz_package/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-05-24 04:57:52.000000 invz_package-0.0.9/innerverz_package/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-05-24 04:57:51.000000 invz_package-0.0.9/innerverz_package/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.709765 invz_package-0.0.9/innerverz_package/deep3dmm/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/deep3dmm/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3711 2023-05-25 05:48:37.000000 invz_package-0.0.9/innerverz_package/deep3dmm/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)    25860 2023-05-25 02:02:16.000000 invz_package-0.0.9/innerverz_package/deep3dmm/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.710562 invz_package-0.0.9/innerverz_package/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-05-25 02:04:04.000000 invz_package-0.0.9/innerverz_package/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9365 2023-05-25 05:29:18.000000 invz_package-0.0.9/innerverz_package/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_alignment/retina_face.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.711017 invz_package-0.0.9/innerverz_package/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-05-25 02:04:18.000000 invz_package-0.0.9/innerverz_package/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.711494 invz_package-0.0.9/innerverz_package/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:44.000000 invz_package-0.0.9/innerverz_package/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4104 2023-05-25 06:00:12.000000 invz_package-0.0.9/innerverz_package/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-05-25 06:09:56.000000 invz_package-0.0.9/innerverz_package/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.712245 invz_package-0.0.9/innerverz_package/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/face_color_transfer/sub_nets/warp_net.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.712708 invz_package-0.0.9/innerverz_package/face_enhancer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       30 2023-05-24 05:06:22.000000 invz_package-0.0.9/innerverz_package/face_enhancer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3745 2023-05-25 05:57:15.000000 invz_package-0.0.9/innerverz_package/face_enhancer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     4079 2023-05-24 05:06:21.000000 invz_package-0.0.9/innerverz_package/face_enhancer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.713171 invz_package-0.0.9/innerverz_package/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-25 02:00:51.000000 invz_package-0.0.9/innerverz_package/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2654 2023-05-25 05:10:35.000000 invz_package-0.0.9/innerverz_package/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-05-25 02:00:38.000000 invz_package-0.0.9/innerverz_package/face_parser/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.713631 invz_package-0.0.9/innerverz_package/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:32.000000 invz_package-0.0.9/innerverz_package/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4275 2023-05-25 06:17:39.000000 invz_package-0.0.9/innerverz_package/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-05-25 06:24:09.000000 invz_package-0.0.9/innerverz_package/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.714477 invz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/head_color_transfer/sub_nets/warp_net.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.715287 invz_package-0.0.9/innerverz_package/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2217 2023-05-25 02:48:38.000000 invz_package-0.0.9/innerverz_package/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/id_extractor/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.715821 invz_package-0.0.9/innerverz_package/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-05-24 05:03:33.000000 invz_package-0.0.9/innerverz_package/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2196 2023-05-25 11:03:26.000000 invz_package-0.0.9/innerverz_package/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-05-25 04:23:49.000000 invz_package-0.0.9/innerverz_package/relighter/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.716286 invz_package-0.0.9/innerverz_package/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/upsampler/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     1977 2023-05-25 08:33:22.000000 invz_package-0.0.9/innerverz_package/upsampler/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)    36818 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/upsampler/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.716993 invz_package-0.0.9/innerverz_package/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-05-25 01:56:47.000000 invz_package-0.0.9/innerverz_package/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-05-24 07:27:58.000000 invz_package-0.0.9/innerverz_package/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1009 2023-05-23 07:04:26.000000 invz_package-0.0.9/innerverz_package/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15902 2023-05-25 06:06:11.000000 invz_package-0.0.9/innerverz_package/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.717505 invz_package-0.0.9/innerverz_package/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-05-25 11:12:49.000000 invz_package-0.0.9/innerverz_package/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5926 2023-05-25 11:09:24.000000 invz_package-0.0.9/innerverz_package/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.717660 invz_package-0.0.9/innerverz_package/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-05-24 07:24:49.000000 invz_package-0.0.9/innerverz_package/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4005 2023-05-25 11:12:19.000000 invz_package-0.0.9/innerverz_package/video_faceparser/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.718946 invz_package-0.0.9/innerverz_package/video_faceparser/util/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-05-25 05:03:53.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.719659 invz_package-0.0.9/innerverz_package/video_faceparser/util/_utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-25 04:42:56.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/_utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9108 2023-05-25 04:42:56.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/_utils/augmentor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4318 2023-05-25 04:42:56.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/_utils/flow_viz.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4024 2023-05-25 04:42:56.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/_utils/frame_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-05-25 05:01:36.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-05-25 04:43:21.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-05-25 04:43:21.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-05-25 04:58:45.000000 invz_package-0.0.9/innerverz_package/video_faceparser/util/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.688789 invz_package-0.0.9/innerverz_package copy/
+-rw-r--r--   0 jjy        (501) staff       (20)      332 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.689369 invz_package-0.0.9/innerverz_package copy/_deblurrer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/_deblurrer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2985 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/_deblurrer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3609 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/_deblurrer/nets.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     1072 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/_deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.689630 invz_package-0.0.9/innerverz_package copy/data_preprocess/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/data_preprocess/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2093 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/data_preprocess/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.690096 invz_package-0.0.9/innerverz_package copy/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    14845 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.691343 invz_package-0.0.9/innerverz_package copy/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)      407 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.692278 invz_package-0.0.9/innerverz_package copy/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.692578 invz_package-0.0.9/innerverz_package copy/deca/utils/rasterizer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/utils/rasterizer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)      706 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.693041 invz_package-0.0.9/innerverz_package copy/deep3dmm/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deep3dmm/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     4417 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deep3dmm/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)    25860 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/deep3dmm/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.693864 invz_package-0.0.9/innerverz_package copy/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9425 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_alignment/retina_face.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.694381 invz_package-0.0.9/innerverz_package copy/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.694842 invz_package-0.0.9/innerverz_package copy/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       48 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6548 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8289 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.696419 invz_package-0.0.9/innerverz_package copy/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/sub_nets/warp_net.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.696802 invz_package-0.0.9/innerverz_package copy/face_color_transfer/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       49 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3319 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_color_transfer/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.697564 invz_package-0.0.9/innerverz_package copy/face_enhancer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       30 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1568 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_enhancer/fe_test.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     4586 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_enhancer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     4079 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_enhancer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.698117 invz_package-0.0.9/innerverz_package copy/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2777 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/face_parser/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.699700 invz_package-0.0.9/innerverz_package copy/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       49 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6583 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8276 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.700530 invz_package-0.0.9/innerverz_package copy/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/sub_nets/warp_net.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.700847 invz_package-0.0.9/innerverz_package copy/head_color_transfer/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       20 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      788 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/head_color_transfer/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.701326 invz_package-0.0.9/innerverz_package copy/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3108 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/id_extractor/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.701766 invz_package-0.0.9/innerverz_package copy/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6291 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2705 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/relighter/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.702172 invz_package-0.0.9/innerverz_package copy/relighter/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/relighter/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5619 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/relighter/utils/blocks.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1858 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/relighter/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.702603 invz_package-0.0.9/innerverz_package copy/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/upsampler/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2231 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/upsampler/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)    36818 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/upsampler/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.703262 invz_package-0.0.9/innerverz_package copy/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1009 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    14233 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.703586 invz_package-0.0.9/innerverz_package copy/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5669 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.703751 invz_package-0.0.9/innerverz_package copy/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-05-25 02:42:00.000000 invz_package-0.0.9/innerverz_package copy/video_faceparser/model/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-26 01:13:36.720573 invz_package-0.0.9/invz_package.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      208 2023-05-26 01:13:36.000000 invz_package-0.0.9/invz_package.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     8174 2023-05-26 01:13:36.000000 invz_package-0.0.9/invz_package.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-05-26 01:13:36.000000 invz_package-0.0.9/invz_package.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       50 2023-05-26 01:13:36.000000 invz_package-0.0.9/invz_package.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       41 2023-05-26 01:13:36.000000 invz_package-0.0.9/invz_package.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 invz_package-0.0.9/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-05-26 01:13:36.721145 invz_package-0.0.9/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      784 2023-05-26 01:13:24.000000 invz_package-0.0.9/setup.py
```

### Comparing `invz_package-0.0.8/LICENSE.txt` & `invz_package-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `invz_package-0.0.8/invz_pack/face_parser/model.py` & `invz_package-0.0.9/innerverz_package/face_parser/nets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,105 @@
+#!/usr/bin/python
+# -*- encoding: utf-8 -*-
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from .resnet import Resnet18
+import torch.utils.model_zoo as modelzoo
 
+# from modules.bn import InPlaceABNSync as BatchNorm2d
+
+resnet18_url = 'https://download.pytorch.org/models/resnet18-5c106cde.pth'
+
+
+def conv3x3(in_planes, out_planes, stride=1):
+    """3x3 convolution with padding"""
+    return nn.Conv2d(in_planes, out_planes, kernel_size=3, stride=stride,
+                     padding=1, bias=False)
+
+
+class BasicBlock(nn.Module):
+    def __init__(self, in_chan, out_chan, stride=1):
+        super(BasicBlock, self).__init__()
+        self.conv1 = conv3x3(in_chan, out_chan, stride)
+        self.bn1 = nn.BatchNorm2d(out_chan)
+        self.conv2 = conv3x3(out_chan, out_chan)
+        self.bn2 = nn.BatchNorm2d(out_chan)
+        self.relu = nn.ReLU(inplace=True)
+        self.downsample = None
+        if in_chan != out_chan or stride != 1:
+            self.downsample = nn.Sequential(
+                nn.Conv2d(in_chan, out_chan,
+                          kernel_size=1, stride=stride, bias=False),
+                nn.BatchNorm2d(out_chan),
+                )
+
+    def forward(self, x):
+        residual = self.conv1(x)
+        residual = F.relu(self.bn1(residual))
+        residual = self.conv2(residual)
+        residual = self.bn2(residual)
+
+        shortcut = x
+        if self.downsample is not None:
+            shortcut = self.downsample(x)
+
+        out = shortcut + residual
+        out = self.relu(out)
+        return out
+
+
+def create_layer_basic(in_chan, out_chan, bnum, stride=1):
+    layers = [BasicBlock(in_chan, out_chan, stride=stride)]
+    for i in range(bnum-1):
+        layers.append(BasicBlock(out_chan, out_chan, stride=1))
+    return nn.Sequential(*layers)
+
+
+class Resnet18(nn.Module):
+    def __init__(self):
+        super(Resnet18, self).__init__()
+        self.conv1 = nn.Conv2d(3, 64, kernel_size=7, stride=2, padding=3,
+                               bias=False)
+        self.bn1 = nn.BatchNorm2d(64)
+        self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
+        self.layer1 = create_layer_basic(64, 64, bnum=2, stride=1)
+        self.layer2 = create_layer_basic(64, 128, bnum=2, stride=2)
+        self.layer3 = create_layer_basic(128, 256, bnum=2, stride=2)
+        self.layer4 = create_layer_basic(256, 512, bnum=2, stride=2)
+        self.init_weight()
+
+    def forward(self, x):
+        x = self.conv1(x)
+        x = F.relu(self.bn1(x))
+        x = self.maxpool(x)
+
+        x = self.layer1(x)
+        feat8 = self.layer2(x) # 1/8
+        feat16 = self.layer3(feat8) # 1/16
+        feat32 = self.layer4(feat16) # 1/32
+        return feat8, feat16, feat32
+
+    def init_weight(self):
+        state_dict = modelzoo.load_url(resnet18_url)
+        self_state_dict = self.state_dict()
+        for k, v in state_dict.items():
+            if 'fc' in k: continue
+            self_state_dict.update({k: v})
+        self.load_state_dict(self_state_dict)
+
+    def get_params(self):
+        wd_params, nowd_params = [], []
+        for name, module in self.named_modules():
+            if isinstance(module, (nn.Linear, nn.Conv2d)):
+                wd_params.append(module.weight)
+                if not module.bias is None:
+                    nowd_params.append(module.bias)
+            elif isinstance(module,  nn.BatchNorm2d):
+                nowd_params += list(module.parameters())
+        return wd_params, nowd_params
 
 
 class BiSeNetOutput(nn.Module):
     def __init__(self, in_chan, mid_chan, n_classes, *args, **kwargs):
         super(BiSeNetOutput, self).__init__()
         self.conv = ConvBNReLU(in_chan, mid_chan, ks=3, stride=1, padding=1)
         self.conv_out = nn.Conv2d(mid_chan, n_classes, kernel_size=1, bias=False)
```

### Comparing `invz_package-0.0.8/invz_pack/id_extractor/nets.py` & `invz_package-0.0.9/innerverz_package/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `invz_package-0.0.8/invz_pack/utils/input.py` & `invz_package-0.0.9/innerverz_package/utils/input.py`

 * *Files identical despite different names*

### Comparing `invz_package-0.0.8/setup.py` & `invz_package-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 
 requirements =[
     'Pillow',
     'numpy',
     'tqdm',
     'gdown',
     'insightface',
+    'opencv-python',
+    
 ]
 
 pypandoc_enabled = True
 try:
     import pypandoc
     print('pandoc enabled')
     long_description = pypandoc.convert_file('README.md', 'rst')
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="invz_package",
-    version="0.0.8",
+    version="0.0.9",
     author="Innerverz-by.JJY",
     author_email="pensee0.0a@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```


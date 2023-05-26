# Comparing `tmp/autogluon.multimodal-0.7.1b20230525.tar.gz` & `tmp/autogluon.multimodal-0.7.1b20230526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.7.1b20230525.tar", last modified: Thu May 25 09:04:22 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.7.1b20230526.tar", last modified: Fri May 26 09:04:17 2023, max compression
```

## Comparing `autogluon.multimodal-0.7.1b20230525.tar` & `autogluon.multimodal-0.7.1b20230526.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.077209 autogluon.multimodal-0.7.1b20230525/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-25 09:04:22.077209 autogluon.multimodal-0.7.1b20230525/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:04:22.077209 autogluon.multimodal-0.7.1b20230525/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.045209 autogluon.multimodal-0.7.1b20230525/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.045209 autogluon.multimodal-0.7.1b20230525/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.049209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.049209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.053209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.053209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.053209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.053209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.053209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.053209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.053209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.053209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.057209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.057209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26706 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.061209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    85367 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.065209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.065209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.065209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   122388 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.077209 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-25 09:03:38.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 09:04:21.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:22.049209 autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-25 09:04:21.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-05-25 09:04:22.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:04:21.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:04:21.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-25 09:04:21.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:04:21.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:04:21.000000 autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.848047 autogluon.multimodal-0.7.1b20230526/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-26 09:04:17.848047 autogluon.multimodal-0.7.1b20230526/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:04:17.848047 autogluon.multimodal-0.7.1b20230526/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.836047 autogluon.multimodal-0.7.1b20230526/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.836047 autogluon.multimodal-0.7.1b20230526/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.836047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.836047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.836047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.836047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.836047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.840047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.840047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.840047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.840047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.840047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.840047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.840047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.840047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84510 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.844047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.844047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.844047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120730 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.848047 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-26 09:03:32.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 09:04:17.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:17.836047 autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-26 09:04:17.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-05-26 09:04:17.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:04:17.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:04:17.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-26 09:04:17.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:04:17.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:04:17.000000 autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.7.1b20230525/PKG-INFO` & `autogluon.multimodal-0.7.1b20230526/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230525
+Version: 0.7.1b20230526
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230525/setup.py` & `autogluon.multimodal-0.7.1b20230526/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/infer_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from io import BytesIO
 from typing import Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 import PIL
 import pytesseract
 
+from autogluon.core.utils import infer_problem_type as infer_basic_problem_type
+
 from ..constants import (
     BINARY,
     CATEGORICAL,
     CLASSIFICATION,
     DOCUMENT_IMAGE,
     DOCUMENT_PDF,
     IDENTIFIER,
@@ -562,14 +564,23 @@
             column_types=column_types,
             allowable_column_types=allowable_column_types,
             fallback_column_type=fallback_column_type,
         )
     if problem_type == NER:
         column_types = infer_ner_column_type(column_types=column_types)
 
+    if problem_type and label_columns:
+        column_types = infer_label_column_type_by_problem_type(
+            column_types=column_types,
+            label_columns=label_columns,
+            problem_type=problem_type,
+            data=data,
+            valid_data=valid_data if is_training else None,
+        )
+
     return column_types
 
 
 def check_missing_values(
     data: pd.DataFrame,
     column_name: str,
     split: Optional[str] = "",
@@ -619,18 +630,17 @@
     if label_columns is None:
         return column_types
 
     if isinstance(label_columns, str):
         label_columns = [label_columns]
 
     for col_name in label_columns:
-        # Make sure the provided label columns are in the dataframe.
-        assert (
-            col_name in column_types
-        ), f"Column {col_name} is not in {column_types.keys()}. Make sure calling `infer_column_types()` first."
+        # For zero-shot inference, label column is unnecessary
+        if col_name not in column_types:
+            continue
         if data is not None:
             check_missing_values(data=data, column_name=col_name, split="training")
         if valid_data is not None:
             check_missing_values(data=valid_data, column_name=col_name, split="validation")
         if column_types[col_name] == NULL:
             raise ValueError(
                 f"Label column '{col_name}' contains only one label class. Make sure it has at least two label classes."
@@ -656,99 +666,103 @@
 ):
     for col_name in column_types.keys():
         if is_rois_column(data[col_name]):
             column_types[col_name] = ROIS
     return column_types
 
 
-def infer_problem_type_output_shape(
-    label_column: str,
-    column_types: Optional[Dict] = None,
-    data: Optional[pd.DataFrame] = None,
+def infer_problem_type(
+    y_train_data: Optional[pd.DataFrame] = None,
     provided_problem_type: Optional[str] = None,
-) -> Tuple[str, int]:
+) -> str:
+    """
+    Infer the basic (binary, multiclass, and regression) problem types if problem type is None or classification.
+    Only training data are used. Assume users provide valid validation data.
+
+    Parameters
+    ----------
+    y_train_data
+        The label column of training data.
+    provided_problem_type
+        Provided problem type
+
+    Returns
+    -------
+    Inferred problem type
+    """
+    if provided_problem_type in [None, CLASSIFICATION]:
+        problem_type = infer_basic_problem_type(y=y_train_data)
+        # trust users' prior knowledge
+        if provided_problem_type == CLASSIFICATION and problem_type == REGRESSION:
+            problem_type = MULTICLASS
+    else:
+        problem_type = provided_problem_type
+
+    return problem_type
+
+
+def infer_output_shape(
+    label_column: str,
+    problem_type: str,
+    data: pd.DataFrame,
+) -> int:
     """
-    Infer the problem type and output shape based on the label column type and training data.
+    Infer the output shape based on the label column type, training data, and problem type.
     Binary classification should have class number 2, while multi-class classification's class
     number should be larger than 2. For regression, the output is restricted to 1 scalar.
 
     Parameters
     ----------
-    column_types
-        Types of columns in a multimodal pd.DataFrame.
     label_column
         The label column in a multimodal pd.DataFrame.
     data
         The multimodal pd.DataFrame for training.
-    provided_problem_type
-        The provided problem type.
+    problem_type
+        Problem type which can be inferred or provided.
 
     Returns
     -------
     problem_type
         Type of problem.
     output_shape
         Shape of output.
     """
     if label_column is None:
-        return provided_problem_type, None
+        return None
 
-    if provided_problem_type is not None:
-        if provided_problem_type == MULTICLASS or provided_problem_type == BINARY:
-            class_num = len(data[label_column].unique())
-            err_msg = (
-                f"Provided problem type is '{provided_problem_type}' while the number of "
-                f"unique values in the label column is {class_num}."
-            )
-            if provided_problem_type == BINARY and class_num != 2:
+    if problem_type in [BINARY, MULTICLASS, REGRESSION, CLASSIFICATION]:
+        class_num = len(data[label_column].unique())
+        err_msg = (
+            f"Problem type is '{problem_type}' while the number of "
+            f"unique values in the label column is {class_num}."
+        )
+        if problem_type == BINARY:
+            if class_num != 2:
                 raise AssertionError(err_msg)
-            elif provided_problem_type == MULTICLASS and class_num <= 2:
+            return 2
+        elif problem_type == MULTICLASS:
+            if class_num <= 2:
                 raise AssertionError(err_msg)
-            return provided_problem_type, class_num
-        if provided_problem_type == BINARY:
-            return BINARY, 2
-        elif provided_problem_type == MULTICLASS:
-            class_num = len(data[label_column].value_counts())
-            return MULTICLASS, class_num
-        elif provided_problem_type == CLASSIFICATION:
-            class_num = len(data[label_column].value_counts())
-            if class_num == 2:
-                return BINARY, 2
-            else:
-                return MULTICLASS, class_num
-        elif provided_problem_type == REGRESSION:
-            return provided_problem_type, 1
-        elif provided_problem_type == NER:
-            return provided_problem_type, None
-        elif provided_problem_type == OBJECT_DETECTION:
-            return provided_problem_type, None
-        elif provided_problem_type == OPEN_VOCABULARY_OBJECT_DETECTION:
-            return provided_problem_type, None
+            return class_num
+        elif problem_type == REGRESSION:
+            if class_num < 1:
+                raise AssertionError(err_msg)
+            return 1
         else:
-            raise ValueError(
-                f"Problem type '{provided_problem_type}' doesn't have a valid output shape "
-                f"for training. The supported problem types are"
-                f" '{BINARY}', '{MULTICLASS}', '{REGRESSION}',"
-                f" '{CLASSIFICATION}', '{NER}',"
-                f" '{OBJECT_DETECTION}', '{OPEN_VOCABULARY_OBJECT_DETECTION}'"
-            )
+            return class_num
+    elif problem_type in [NER, OBJECT_DETECTION, OPEN_VOCABULARY_OBJECT_DETECTION]:
+        return None
     else:
-        if column_types[label_column] == CATEGORICAL:
-            class_num = len(data[label_column].unique())
-            if class_num == 2:
-                return BINARY, 2
-            else:
-                return MULTICLASS, class_num
-        elif column_types[label_column] == NUMERICAL:
-            return REGRESSION, 1
-        else:
-            raise ValueError(
-                f"The label column '{label_column}' has type"
-                f" '{column_types[label_column]}', which is not supported yet."
-            )
+        raise ValueError(
+            f"Problem type '{problem_type}' doesn't have a valid output shape "
+            f"for training. The supported problem types are"
+            f" '{BINARY}', '{MULTICLASS}', '{REGRESSION}',"
+            f" '{CLASSIFICATION}', '{NER}',"
+            f" '{OBJECT_DETECTION}', '{OPEN_VOCABULARY_OBJECT_DETECTION}'"
+        )
 
 
 def set_fallback_column_type(column_types: Dict, allowable_column_types: List[str], fallback_column_type: str) -> Dict:
     """
     Filter the auto-detected column types to make sure that all column types are allowable.
     Use the fallback type to replace those out of the allowable_column_types.
```

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,15 @@
     TEXT,
     UNIFORM_SOUP,
     Y_PRED,
     Y_PRED_PROB,
     Y_TRUE,
 )
 from .data.datamodule import BaseDataModule
-from .data.infer_types import (
-    infer_column_types,
-    infer_label_column_type_by_problem_type,
-    infer_problem_type_output_shape,
-)
+from .data.infer_types import infer_column_types, infer_output_shape, infer_problem_type
 from .data.preprocess_dataframe import MultiModalFeaturePreprocessor
 from .optimization.lit_matcher import MatcherLitModule
 from .optimization.utils import get_matcher_loss_func, get_matcher_miner_func, get_metric
 from .presets import matcher_presets
 from .utils import (
     AutoMMModelCheckpoint,
     CustomUnpickler,
@@ -390,63 +386,54 @@
             tuning_data=tuning_data,
             holdout_frac=holdout_frac,
             is_classification=self._problem_type in [BINARY, MULTICLASS, CLASSIFICATION],
             label_column=self._label_column,
             seed=seed,
         )
 
+        if self._label_column:
+            self._problem_type = infer_problem_type(
+                y_train_data=train_data[self._label_column],
+                provided_problem_type=self._problem_type,
+            )
+
         column_types = infer_column_types(
             data=train_data,
             valid_data=tuning_data,
             label_columns=self._label_column,
             provided_column_types=column_types,
-            id_mappings=id_mappings,
-        )
-        column_types = infer_label_column_type_by_problem_type(
-            column_types=column_types,
-            label_columns=self._label_column,
-            problem_type=self._problem_type,
-            data=train_data,
-            valid_data=tuning_data,
+            problem_type=self._problem_type,  # used to update the corresponding column type
         )
-        problem_type, output_shape = infer_problem_type_output_shape(
+
+        output_shape = infer_output_shape(
             label_column=self._label_column,
-            column_types=column_types,
             data=train_data,
-            provided_problem_type=self._problem_type,
+            problem_type=self._problem_type,
         )
 
         logger.debug(f"column_types: {column_types}")
         logger.debug(f"image columns: {[k for k, v in column_types.items() if v == 'image_path']}")
 
         if self._column_types is not None and self._column_types != column_types:
             warnings.warn(
                 f"Inferred column types {column_types} are inconsistent with "
                 f"the previous {self._column_types}. "
                 f"New columns will not be used in the current training."
             )
             # use previous column types to avoid inconsistency with previous numerical mlp and categorical mlp
             column_types = self._column_types
 
-        if self._problem_type is not None:
-            if self._problem_type == CLASSIFICATION:
-                # Set the problem type to be inferred problem type
-                self._problem_type = problem_type
-            assert self._problem_type == problem_type, (
-                f"Inferred problem type {problem_type} is different from " f"the previous {self._problem_type}"
-            )
-
         if self._output_shape is not None:
             assert self._output_shape == output_shape, (
                 f"Inferred output shape {output_shape} is different from " f"the previous {self._output_shape}"
             )
 
         if self._validation_metric_name is None or self._eval_metric_name is None:
             validation_metric_name, eval_metric_name = infer_metrics(
-                problem_type=problem_type,
+                problem_type=self._problem_type,
                 is_matching=self._pipeline in matcher_presets.list_keys(),
                 eval_metric_name=self._eval_metric_name,
             )
         else:
             validation_metric_name = self._validation_metric_name
             eval_metric_name = self._eval_metric_name
         minmax_mode = get_minmax_mode(validation_metric_name)
@@ -456,15 +443,14 @@
 
         if self._presets is not None:
             presets = self._presets
         else:
             self._presets = presets
 
         # set attributes for saving and prediction
-        self._problem_type = problem_type  # In case problem type isn't provided in __init__().
         self._eval_metric_name = eval_metric_name  # In case eval_metric isn't provided in __init__().
         self._validation_metric_name = validation_metric_name
         self._output_shape = output_shape
         self._column_types = column_types
 
         hyperparameters, hyperparameter_tune_kwargs = update_hyperparameters(
             problem_type=self._pipeline,
@@ -1106,25 +1092,20 @@
                 assert sorted(allowable_query_dtypes) == sorted(allowable_response_dtypes)
                 assert fallback_query_dtype == fallback_response_dtype
                 allowable_dtypes = allowable_query_dtypes
                 fallback_dtype = fallback_query_dtype
 
             column_types = infer_column_types(
                 data=data,
+                label_columns=self._label_column,
+                problem_type=self._problem_type,
                 allowable_column_types=allowable_dtypes,
                 fallback_column_type=fallback_dtype,
                 id_mappings=id_mappings,
             )
-            if self._label_column and self._label_column in data.columns:
-                column_types = infer_label_column_type_by_problem_type(
-                    column_types=column_types,
-                    label_columns=self._label_column,
-                    problem_type=self._problem_type,
-                    data=data,
-                )
         else:  # called .fit() or .load()
             column_types = self._column_types
 
         query_config = None
         query_model = None
         response_config = None
         response_model = None
```

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.core.utils import default_holdout_frac, generate_train_test_split_combined
 from autogluon.core.utils.loaders import load_pd
 from autogluon.multimodal.utils.log import get_fit_complete_message, get_fit_start_message
 
 from . import version as ag_version
 from .constants import (
-    AUTOMM,
     AUTOMM_TUTORIAL_MODE,
     BBOX,
     BEST,
     BEST_K_MODELS_FILE,
     BINARY,
+    CLASSIFICATION,
     COLUMN_FEATURES,
     DEEPSPEED_MIN_PL_VERSION,
     DEEPSPEED_MODULE,
     DEEPSPEED_OFFLOADING,
     DEEPSPEED_STRATEGY,
     DEPRECATED_ZERO_SHOT,
     DOCUMENT,
@@ -85,16 +85,16 @@
     Y_TRUE,
     ZERO_SHOT_IMAGE_CLASSIFICATION,
 )
 from .data.datamodule import BaseDataModule
 from .data.dataset_mmlab import MultiImageMixDataset
 from .data.infer_types import (
     infer_column_types,
-    infer_label_column_type_by_problem_type,
-    infer_problem_type_output_shape,
+    infer_output_shape,
+    infer_problem_type,
     infer_rois_column_type,
     is_image_column,
 )
 from .data.preprocess_dataframe import MultiModalFeaturePreprocessor
 from .matcher import MultiModalMatcher
 from .models.utils import get_model_postprocess_fn
 from .optimization.lit_distiller import DistillerLitModule
@@ -708,31 +708,37 @@
             old_save_path=self._save_path,
             proposed_save_path=save_path,
             raise_if_exist=True,
             warn_if_exist=False,
             fit_called=fit_called,
         )
 
-        self._problem_type = self._infer_problem_type(train_data=train_data, column_types=column_types)
-
         if tuning_data is None:
             train_data, tuning_data = self._split_train_tuning(
                 data=train_data, holdout_frac=holdout_frac, random_state=seed
             )
 
-        column_types = self._infer_column_types(
-            train_data=train_data, tuning_data=tuning_data, column_types=column_types
+        if self._label_column:
+            self._problem_type = infer_problem_type(
+                y_train_data=train_data[self._label_column],
+                provided_problem_type=self._problem_type,
+            )
+
+        column_types = infer_column_types(
+            data=train_data,
+            valid_data=tuning_data,
+            label_columns=self._label_column,
+            provided_column_types=column_types,
+            problem_type=self._problem_type,  # used to update the corresponding column type
         )
 
-        # FIXME: separate infer problem_type with output_shape, should be logically distinct
-        _, output_shape = infer_problem_type_output_shape(
+        output_shape = infer_output_shape(
             label_column=self._label_column,
-            column_types=column_types,
             data=train_data,
-            provided_problem_type=self._problem_type,
+            problem_type=self._problem_type,
         )
 
         # Determine data scarcity mode, i.e. a few-shot scenario
         scarcity_mode = infer_scarcity_mode_by_data_size(
             df_train=train_data, scarcity_threshold=50
         )  # Add as separate hyperparameter somewhere?
         if scarcity_mode == FEW_SHOT and (not presets or FEW_SHOT not in presets):  # TODO: check for data  type
@@ -838,50 +844,14 @@
         self._total_train_time = training_end - training_start
 
         # TODO(?) We should have a separate "_post_training_event()" for logging messages.
         logger.info(get_fit_complete_message(self._save_path))
 
         return self
 
-    # FIXME: Avoid having separate logic for inferring features and label column that is combined together
-    def _infer_column_types(
-        self, train_data: pd.DataFrame, tuning_data: pd.DataFrame = None, column_types: dict = None
-    ) -> dict:
-        column_types = infer_column_types(
-            data=train_data,
-            label_columns=self._label_column,
-            provided_column_types=column_types,
-            valid_data=tuning_data,
-            problem_type=self._problem_type,
-        )
-        column_types = infer_label_column_type_by_problem_type(
-            column_types=column_types,
-            label_columns=self._label_column,
-            problem_type=self._problem_type,
-            data=train_data,
-            valid_data=tuning_data,
-        )
-        return column_types
-
-    # FIXME: Align logic with Tabular,
-    #  don't combine output_shape and problem_type detection, make them separate
-    #  Use autogluon.core.utils.utils.infer_problem_type
-    def _infer_problem_type(self, train_data: pd.DataFrame, column_types: dict = None) -> str:
-        column_types_label = self._infer_column_types(
-            train_data=train_data[[self._label_column]], column_types=column_types
-        )
-
-        problem_type, _ = infer_problem_type_output_shape(
-            label_column=self._label_column,
-            column_types=column_types_label,
-            data=train_data,
-            provided_problem_type=self._problem_type,
-        )
-        return problem_type
-
     def _split_train_tuning(
         self, data: pd.DataFrame, holdout_frac: float = None, random_state: int = 0
     ) -> (pd.DataFrame, pd.DataFrame):
         """
         Splits `data` into `train_data` and `tuning_data`.
         If the problem_type is one of ['binary', 'multiclass']:
             The split will be done with stratification on the label column.
@@ -1820,24 +1790,19 @@
         requires_label: bool,
     ):
         if self._column_types is None:
             data = data_to_df(data=data)
             allowable_dtypes, fallback_dtype = infer_dtypes_by_model_names(model_config=self._config.model)
             column_types = infer_column_types(
                 data=data,
+                label_columns=self._label_column,
+                problem_type=self._problem_type,
                 allowable_column_types=allowable_dtypes,
                 fallback_column_type=fallback_dtype,
             )
-            if self._label_column and self._label_column in data.columns:
-                column_types = infer_label_column_type_by_problem_type(
-                    column_types=column_types,
-                    label_columns=self._label_column,
-                    problem_type=self._problem_type,
-                    data=data,
-                )
             if self._problem_type == OBJECT_DETECTION:
                 column_types = infer_rois_column_type(
                     column_types=column_types,
                     data=data,
                 )
         else:  # called .fit() or .load()
             column_names = list(self._column_types.keys())
```

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.7.1b20230526/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230525
+Version: 0.7.1b20230526
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230525/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.7.1b20230526/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
 transformers<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
 sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.7.1b20230525
-autogluon.features==0.7.1b20230525
-autogluon.common==0.7.1b20230525
+autogluon.core[raytune]==0.7.1b20230526
+autogluon.features==0.7.1b20230526
+autogluon.common==0.7.1b20230526
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>0.1.5
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```


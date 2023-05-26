# Comparing `tmp/miacag-0.0.81.tar.gz` & `tmp/miacag-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miacag-0.0.81.tar", last modified: Mon Apr 17 09:05:13 2023, max compression
+gzip compressed data, was "miacag-0.0.82.tar", last modified: Fri May 26 10:09:43 2023, max compression
```

## Comparing `miacag-0.0.81.tar` & `miacag-0.0.82.tar`

### file list

```diff
@@ -1,175 +1,186 @@
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-01 15:05:05.000000 miacag-0.0.81/LICENSE
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      129 2022-09-01 15:05:05.000000 miacag-0.0.81/MANIFEST.in
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-04-17 09:05:13.058542 miacag-0.0.81/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      111 2022-10-20 03:13:52.000000 miacag-0.0.81/README.md
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/classification/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/classification/_3D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/classification/_3D/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/classification/_3D/lca_rca/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/classification/_3D/lca_rca/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3800 2022-09-20 09:25:18.000000 miacag-0.0.81/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/classification/_3D/stenosis_detection_rca/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9668 2022-09-20 09:25:18.000000 miacag-0.0.81/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/classification/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      823 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/config.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3229 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/options.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      881 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/update_configs.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/Classification/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/Classification/_2D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_2D/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12802 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13280 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    71072 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_2D/dataset_mil_2d.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/Classification/_3D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2088 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_avi_video.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9581 2023-04-13 12:05:57.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    23950 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    72019 2022-11-04 15:43:12.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/dataset_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Classification/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8869 2023-04-16 16:02:37.000000 miacag-0.0.81/miacag/dataloader/Classification/get_dataloader_classification.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2440 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/DistributedWeightedSampler.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/Representation/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Representation/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10772 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Representation/get_dataloader_representation.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5611 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/dataloader_base.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    24663 2023-04-17 08:45:34.000000 miacag-0.0.81/miacag/dataloader/dataloader_base_monai.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6113 2023-02-09 10:02:46.000000 miacag-0.0.81/miacag/dataloader/get_dataloader.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/metrics/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/metrics/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1180 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/metrics/cumulativeSumming.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4969 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/metrics/metrics.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12633 2023-02-10 10:26:52.000000 miacag-0.0.81/miacag/metrics/metrics_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/model_utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9549 2023-02-20 12:20:17.000000 miacag-0.0.81/miacag/model_utils/GradCam_model.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/model_utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    11960 2023-02-16 14:53:46.000000 miacag-0.0.81/miacag/model_utils/eval_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3993 2023-02-09 13:45:35.000000 miacag-0.0.81/miacag/model_utils/get_loss_func.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/model_utils/get_optimizer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10574 2023-02-16 15:15:54.000000 miacag-0.0.81/miacag/model_utils/get_test_pipeline.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9286 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/model_utils/grad_cam_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12228 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/model_utils/predict_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1576 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/model_utils/scheduler.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      785 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/model_utils/siam_loss.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6704 2023-02-16 14:52:08.000000 miacag-0.0.81/miacag/model_utils/train_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8655 2022-12-09 11:43:53.000000 miacag-0.0.81/miacag/models/BuildModel.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/backbone_encoders/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/backbone_encoders/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/backbone_encoders/tabular/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/backbone_encoders/tabular/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      212 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/backbone_encoders/tabular/base_encoders.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      670 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/cnns.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12742 2023-04-17 08:46:16.000000 miacag-0.0.81/miacag/models/get_encoder.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    11806 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/models/milmodel3d.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1769 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/mlps.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13303 2023-04-17 08:43:21.000000 miacag-0.0.81/miacag/models/modeling_finetune.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13780 2023-04-17 07:32:41.000000 miacag-0.0.81/miacag/models/modeling_pretrain.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8388 2023-04-17 08:44:09.000000 miacag-0.0.81/miacag/models/modules.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13824 2023-04-16 15:10:08.000000 miacag-0.0.81/miacag/models/pretrained_vit.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/models/torchhub/2D/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/models/torchhub/2D/r50/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/models/torchhub/2D/r50/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/mvit_base_16x4/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/mvit_base_16x4/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/mvit_base_32x3/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/mvit_base_32x3/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/r2plus1_18/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/r2plus1_18/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/x3d_s/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/x3d_s/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/plots/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/plots/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1983 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/plots/angle_plotter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      408 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/plots/getDataFromPdf.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      795 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/plots/plot_histogram.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10561 2023-02-09 10:02:46.000000 miacag-0.0.81/miacag/plots/plot_roc_auc_all.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1277 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/plots/plot_scatter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1245 2023-01-27 08:30:25.000000 miacag-0.0.81/miacag/plots/plot_test.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    32951 2023-02-17 09:58:18.000000 miacag-0.0.81/miacag/plots/plotter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4543 2023-01-27 08:26:48.000000 miacag-0.0.81/miacag/plots/query_plot_agg_max.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/postprocessing/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/postprocessing/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3593 2022-12-16 18:58:11.000000 miacag-0.0.81/miacag/postprocessing/aggregate_pr_group.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1880 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/postprocessing/append_results.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4331 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/postprocessing/count_stenosis_pr_group.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5354 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/postprocessing/estimate_vessel_disease.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2527 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/predictor.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/preprocessing/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1319 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/add_columns.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1412 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/copy_column.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1321 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/copy_table.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/datasetFingerpring.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    21523 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/datasetFingerprint.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3232 2022-12-16 18:58:24.000000 miacag-0.0.81/miacag/preprocessing/labels_map.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7064 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/pre_process.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/preprocessing/process_labels/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/process_labels/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-12-16 18:59:24.000000 miacag-0.0.81/miacag/preprocessing/process_labels/process_dominance.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    15711 2023-03-02 17:26:57.000000 miacag-0.0.81/miacag/preprocessing/process_labels/process_total_occ.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3631 2023-02-09 12:23:35.000000 miacag-0.0.81/miacag/preprocessing/split_train_val.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2344 2022-12-16 18:58:52.000000 miacag-0.0.81/miacag/preprocessing/transform_missing_floats.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2521 2022-12-16 18:58:58.000000 miacag-0.0.81/miacag/preprocessing/transform_stenosis.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4756 2023-01-10 15:49:41.000000 miacag-0.0.81/miacag/preprocessing/transform_thresholds.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2591 2022-12-16 18:59:17.000000 miacag-0.0.81/miacag/preprocessing/transform_total_occlusion.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/preprocessing/utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1402 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/utils/check_experiments.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/scripts/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13571 2023-01-10 16:02:18.000000 miacag-0.0.81/miacag/scripts/aggregate_and_plot.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/angiography_classifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/angiography_classifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4725 2022-11-01 08:35:36.000000 miacag-0.0.81/miacag/scripts/angiography_classifier/predict_angio.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13153 2022-11-09 16:17:09.000000 miacag-0.0.81/miacag/scripts/angiography_classifier/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/angiography_classifier_stenosis_identifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/angiography_classifier_stenosis_identifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2093 2022-11-09 16:17:20.000000 miacag-0.0.81/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3675 2023-02-28 09:02:39.000000 miacag-0.0.81/miacag/scripts/compare_PCI_notPCI.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6510 2023-03-02 16:02:03.000000 miacag-0.0.81/miacag/scripts/predict_patologi_eyeball_vs_estimated.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_identifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/stenosis_identifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    22787 2023-01-10 15:51:19.000000 miacag-0.0.81/miacag/scripts/stenosis_identifier/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_identifier_mil/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/stenosis_identifier_mil/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    16366 2023-01-02 10:46:44.000000 miacag-0.0.81/miacag/scripts/stenosis_identifier_mil/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_regression/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/stenosis_regression/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    27197 2023-04-16 15:00:01.000000 miacag-0.0.81/miacag/scripts/stenosis_regression/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_regression_full/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/stenosis_regression_full/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7208 2022-11-09 16:15:58.000000 miacag-0.0.81/miacag/scripts/stenosis_regression_full/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_regression_with_pretraining/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-04-16 14:46:27.000000 miacag-0.0.81/miacag/scripts/stenosis_regression_with_pretraining/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    27334 2023-04-16 14:50:42.000000 miacag-0.0.81/miacag/scripts/stenosis_regression_with_pretraining/submit_angio.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2864 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/tester.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/tests/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/tests/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2109 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/tests/test_sql_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4804 2023-02-10 08:51:02.000000 miacag-0.0.81/miacag/trainer.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2886 2023-02-23 08:19:40.000000 miacag-0.0.81/miacag/utils/common_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1313 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/utils/script_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6205 2023-02-20 16:23:18.000000 miacag-0.0.81/miacag/utils/sql_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag.egg-info/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-04-17 09:05:13.000000 miacag-0.0.81/miacag.egg-info/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5377 2023-04-17 09:05:13.000000 miacag-0.0.81/miacag.egg-info/SOURCES.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-04-17 09:05:13.000000 miacag-0.0.81/miacag.egg-info/dependency_links.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        7 2023-04-17 09:05:13.000000 miacag-0.0.81/miacag.egg-info/top_level.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      106 2022-09-01 15:05:05.000000 miacag-0.0.81/pyproject.toml
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      524 2023-04-17 09:05:13.062542 miacag-0.0.81/setup.cfg
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-01 15:05:05.000000 miacag-0.0.82/LICENSE
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      129 2022-09-01 15:05:05.000000 miacag-0.0.82/MANIFEST.in
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-05-26 10:09:43.438565 miacag-0.0.82/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      111 2022-10-20 03:13:52.000000 miacag-0.0.82/README.md
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/classification/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/classification/_3D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/classification/_3D/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/classification/_3D/lca_rca/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/classification/_3D/lca_rca/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3800 2022-09-20 09:25:18.000000 miacag-0.0.82/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/configs/classification/_3D/stenosis_detection_rca/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9668 2022-09-20 09:25:18.000000 miacag-0.0.82/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/classification/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      823 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/config.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3229 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/options.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      881 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/configs/update_configs.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag/dataloader/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/dataloader/Classification/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/dataloader/Classification/_2D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/dataloader/Classification/_2D/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12802 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    14190 2023-05-19 09:24:28.000000 miacag-0.0.82/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    71072 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/dataloader/Classification/_2D/dataset_mil_2d.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/dataloader/Classification/_3D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2088 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_avi_video.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9581 2023-05-16 11:27:04.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    24226 2023-05-19 09:12:51.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    72019 2022-11-04 15:43:12.000000 miacag-0.0.82/miacag/dataloader/Classification/_3D/dataset_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Classification/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9370 2023-05-17 13:50:58.000000 miacag-0.0.82/miacag/dataloader/Classification/get_dataloader_classification.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2440 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/DistributedWeightedSampler.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/dataloader/Representation/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Representation/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    10772 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/Representation/get_dataloader_representation.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5611 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/dataloader/dataloader_base.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    24810 2023-05-19 06:35:38.000000 miacag-0.0.82/miacag/dataloader/dataloader_base_monai.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6113 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/dataloader/get_dataloader.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/metrics/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/metrics/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1180 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/metrics/cumulativeSumming.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4969 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/metrics/metrics.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13559 2023-05-23 12:24:10.000000 miacag-0.0.82/miacag/metrics/metrics_utils.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/model_utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9549 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/model_utils/GradCam_model.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/model_utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12046 2023-05-23 13:56:02.000000 miacag-0.0.82/miacag/model_utils/eval_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4045 2023-05-19 07:50:15.000000 miacag-0.0.82/miacag/model_utils/get_loss_func.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2023-05-19 08:49:06.000000 miacag-0.0.82/miacag/model_utils/get_optimizer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    10922 2023-05-24 05:35:58.000000 miacag-0.0.82/miacag/model_utils/get_test_pipeline.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9286 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/model_utils/grad_cam_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12228 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/model_utils/predict_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1576 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/model_utils/scheduler.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      785 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/model_utils/siam_loss.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6720 2023-05-23 12:03:48.000000 miacag-0.0.82/miacag/model_utils/train_utils.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/models/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8774 2023-05-19 08:51:15.000000 miacag-0.0.82/miacag/models/BuildModel.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/models/backbone_encoders/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/backbone_encoders/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/models/backbone_encoders/tabular/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/backbone_encoders/tabular/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      212 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/backbone_encoders/tabular/base_encoders.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      670 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/cnns.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.430565 miacag-0.0.82/miacag/models/dino_utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-16 12:42:02.000000 miacag-0.0.82/miacag/models/dino_utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6468 2023-05-17 12:25:03.000000 miacag-0.0.82/miacag/models/dino_utils/dino_pretrained.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13826 2023-05-19 09:49:15.000000 miacag-0.0.82/miacag/models/get_encoder.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/mae_st_util/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-04-25 13:02:50.000000 miacag-0.0.82/miacag/models/mae_st_util/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3130 2023-04-25 13:03:31.000000 miacag-0.0.82/miacag/models/mae_st_util/logging.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6395 2023-04-25 13:05:51.000000 miacag-0.0.82/miacag/models/mae_st_util/models_vit.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4915 2023-04-25 13:44:14.000000 miacag-0.0.82/miacag/models/mae_st_util/video_vit.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    11884 2023-05-19 06:59:56.000000 miacag-0.0.82/miacag/models/milmodel3d.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12926 2023-05-17 12:55:21.000000 miacag-0.0.82/miacag/models/milmodel_from_features.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1769 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/mlps.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13303 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/models/modeling_finetune.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13780 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/models/modeling_pretrain.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8584 2023-05-23 10:13:32.000000 miacag-0.0.82/miacag/models/modules.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13824 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/models/pretrained_vit.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/models/torchhub/2D/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D/r50/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/models/torchhub/2D/r50/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/mvit_base_16x4/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/mvit_base_16x4/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/mvit_base_32x3/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/mvit_base_32x3/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/r2plus1_18/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/r2plus1_18/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/models/torchhub/2D+T/x3d_s/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/2D+T/x3d_s/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/models/torchhub/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/plots/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/plots/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1983 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/plots/angle_plotter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      408 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/plots/getDataFromPdf.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      795 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/plots/plot_histogram.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4724 2023-05-25 10:22:04.000000 miacag-0.0.82/miacag/plots/plot_pathology_treatment_pred.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5167 2023-05-25 11:08:34.000000 miacag-0.0.82/miacag/plots/plot_predict_coronary_pathology.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    10561 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/plots/plot_roc_auc_all.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1277 2022-11-01 13:34:24.000000 miacag-0.0.82/miacag/plots/plot_scatter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1245 2023-01-27 08:30:25.000000 miacag-0.0.82/miacag/plots/plot_test.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    33279 2023-05-22 15:55:28.000000 miacag-0.0.82/miacag/plots/plotter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4543 2023-01-27 08:26:48.000000 miacag-0.0.82/miacag/plots/query_plot_agg_max.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/postprocessing/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/postprocessing/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3593 2022-12-16 18:58:11.000000 miacag-0.0.82/miacag/postprocessing/aggregate_pr_group.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1880 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/postprocessing/append_results.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4331 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/postprocessing/count_stenosis_pr_group.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5354 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/postprocessing/estimate_vessel_disease.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2527 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/predictor.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/preprocessing/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1319 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/add_columns.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1412 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/copy_column.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1321 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/copy_table.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/datasetFingerpring.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    21523 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/datasetFingerprint.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3232 2023-05-25 09:45:44.000000 miacag-0.0.82/miacag/preprocessing/labels_map.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7064 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/pre_process.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/preprocessing/process_labels/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/process_labels/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-12-16 18:59:24.000000 miacag-0.0.82/miacag/preprocessing/process_labels/process_dominance.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15711 2023-03-02 17:26:57.000000 miacag-0.0.82/miacag/preprocessing/process_labels/process_total_occ.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3631 2023-05-23 08:44:57.000000 miacag-0.0.82/miacag/preprocessing/split_train_val.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2344 2022-12-16 18:58:52.000000 miacag-0.0.82/miacag/preprocessing/transform_missing_floats.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2521 2022-12-16 18:58:58.000000 miacag-0.0.82/miacag/preprocessing/transform_stenosis.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4756 2023-01-10 15:49:41.000000 miacag-0.0.82/miacag/preprocessing/transform_thresholds.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2591 2022-12-16 18:59:17.000000 miacag-0.0.82/miacag/preprocessing/transform_total_occlusion.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.434565 miacag-0.0.82/miacag/preprocessing/utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1402 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/preprocessing/utils/check_experiments.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13571 2023-01-10 16:02:18.000000 miacag-0.0.82/miacag/scripts/aggregate_and_plot.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/angiography_classifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/angiography_classifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4842 2023-05-19 07:46:19.000000 miacag-0.0.82/miacag/scripts/angiography_classifier/predict_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13266 2023-05-23 10:33:43.000000 miacag-0.0.82/miacag/scripts/angiography_classifier/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/angiography_classifier_stenosis_identifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/angiography_classifier_stenosis_identifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2206 2023-05-19 07:46:41.000000 miacag-0.0.82/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3675 2023-02-28 09:02:39.000000 miacag-0.0.82/miacag/scripts/compare_PCI_notPCI.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6510 2023-03-02 16:02:03.000000 miacag-0.0.82/miacag/scripts/predict_patologi_eyeball_vs_estimated.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/pretraining_downstreams/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-15 17:03:06.000000 miacag-0.0.82/miacag/scripts/pretraining_downstreams/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    21016 2023-05-25 10:58:02.000000 miacag-0.0.82/miacag/scripts/pretraining_downstreams/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/stenosis_identifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/stenosis_identifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    22900 2023-05-19 07:46:49.000000 miacag-0.0.82/miacag/scripts/stenosis_identifier/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/stenosis_identifier_mil/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/stenosis_identifier_mil/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    16479 2023-05-19 07:46:55.000000 miacag-0.0.82/miacag/scripts/stenosis_identifier_mil/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/stenosis_regression/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/stenosis_regression/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    27314 2023-05-19 07:47:03.000000 miacag-0.0.82/miacag/scripts/stenosis_regression/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/scripts/stenosis_regression_full/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/scripts/stenosis_regression_full/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7325 2023-05-19 07:47:08.000000 miacag-0.0.82/miacag/scripts/stenosis_regression_full/submit_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2933 2023-05-19 08:24:26.000000 miacag-0.0.82/miacag/tester.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/tests/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/tests/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2109 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/tests/test_sql_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4836 2023-05-19 08:16:57.000000 miacag-0.0.82/miacag/trainer.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.438565 miacag-0.0.82/miacag/utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3070 2023-05-23 12:08:55.000000 miacag-0.0.82/miacag/utils/common_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1313 2022-09-01 15:05:05.000000 miacag-0.0.82/miacag/utils/script_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6241 2023-05-23 10:53:47.000000 miacag-0.0.82/miacag/utils/sql_utils.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-26 10:09:43.426565 miacag-0.0.82/miacag.egg-info/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-05-26 10:09:43.000000 miacag-0.0.82/miacag.egg-info/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5720 2023-05-26 10:09:43.000000 miacag-0.0.82/miacag.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-26 10:09:43.000000 miacag-0.0.82/miacag.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        7 2023-05-26 10:09:43.000000 miacag-0.0.82/miacag.egg-info/top_level.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      106 2022-09-01 15:05:05.000000 miacag-0.0.82/pyproject.toml
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      524 2023-05-26 10:09:43.438565 miacag-0.0.82/setup.cfg
```

### Comparing `miacag-0.0.81/LICENSE` & `miacag-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/PKG-INFO` & `miacag-0.0.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miacag
-Version: 0.0.81
+Version: 0.0.82
 Summary: miacag angio DL tools
 Home-page: https://github.com/ChristianEschen/miacag
 Author: Christian Eschen
 Author-email: christian_eschen@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miacag-0.0.81/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml` & `miacag-0.0.82/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml` & `miacag-0.0.82/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/configs/config.py` & `miacag-0.0.82/miacag/configs/config.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/configs/options.py` & `miacag-0.0.82/miacag/configs/options.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/configs/update_configs.py` & `miacag-0.0.82/miacag/configs/update_configs.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py` & `miacag-0.0.82/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py` & `miacag-0.0.82/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,26 +145,33 @@
             self.data_par_train = monai.data.partition_dataset(
                 data=self.data,
                 num_partitions=dist.get_world_size(),
                 shuffle=True,
                 even_divisible=True,
             )[dist.get_rank()]
 
-        # create a training data loader
-        if self.config['cache_num'] != 'None':
+        # create a training data loader'
+        if self.config['cache_num'] not in ['standard', 'None']:
             train_ds = SmartCacheDataset(
                 config=self.config,
                 features=self.features,
                 data=self.data_par_train,
                 transform=train_transforms,
                 copy_cache=True,
                 cache_num=self.config['cache_num'],
                 num_init_workers=int(self.config['num_workers']/2),
                 replace_rate=self.config['replace_rate'],
                 num_replace_workers=int(self.config['num_workers']/2))
+        
+        elif self.config['cache_num'] == 'standard':
+            train_ds = Dataset(
+                        config=self.config,
+                        features=self.features,
+                        data=self.data_par_train, transform=train_transforms
+                    )
         else:
             train_ds = CacheDataset(
                 config=self.config,
                 features=self.features,
                 data=self.data_par_train,
                 transform=train_transforms,
                 copy_cache=True,
@@ -214,25 +221,31 @@
             data=self.data,
             num_partitions=dist.get_world_size(),
             shuffle=False,
             even_divisible=True if self.config['loaders']['mode'] not in ['testing', 'prediction'] else False,
         )[dist.get_rank()]
         rowids = [i["rowid"] for i in self.data_par_val]
         if self.config['loaders']['mode'] not in ['prediction', 'testing']:
-            if self.config['cache_num'] != 'None':
+            if self.config['cache_num'] not in ['standard', 'None']:
                 val_ds = SmartCacheDataset(
                     config=self.config,
                     features=self.features,
                     data=self.data_par_val,
                     transform=val_transforms,
                     copy_cache=True,
                     cache_num=self.config['cache_num'],
                     num_init_workers=int(self.config['num_workers']/2),
                     replace_rate=self.config['replace_rate'],
                     num_replace_workers=int(self.config['num_workers']/2))
+            elif self.config['cache_num'] == 'standard':
+                val_ds = Dataset(
+                            config=self.config,
+                            features=self.features,
+                            data=self.data_par_val, transform=val_transforms
+                        )
             else:
                 val_ds = CacheDataset(
                     config=self.config,
                     features=self.features,
                     data=self.data_par_val,
                     transform=val_transforms,
                     copy_cache=True,
@@ -248,14 +261,20 @@
                         num_workers=self.config['num_workers'])
             elif self.config['cache_test'] == "False":
                 val_ds = Dataset(
                         config=self.config,
                         features=self.features,
                         data=self.data_par_val, transform=val_transforms
                     )
+            elif self.config['cache_num'] == 'standard':
+                val_ds = Dataset(
+                            config=self.config,
+                            features=self.features,
+                            data=self.data_par_val, transform=val_transforms
+                        )
             elif self.config['cache_test'] == "persistant":
                 cachDir = os.path.join(
                     self.config['model']['pretrain_model'],
                     'persistent_cache')
                 val_ds = PersistentDataset(
                         config=self.config,
                         features=self.features,
```

### Comparing `miacag-0.0.81/miacag/dataloader/Classification/_2D/dataset_mil_2d.py` & `miacag-0.0.82/miacag/dataloader/Classification/_2D/dataset_mil_2d.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_avi_video.py` & `miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_avi_video.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py` & `miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py` & `miacag-0.0.82/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,20 @@
                 data=self.data_par_train,
                 transform=train_transforms,
                 copy_cache=True,
                 cache_num=self.config['cache_num'],
                 num_init_workers=int(self.config['num_workers']/2),
                 replace_rate=self.config['replace_rate'],
                 num_replace_workers=int(self.config['num_workers']/2))
+        elif self.config['cache_num'] == 'standard':
+            train_ds = Dataset(
+                        config=self.config,
+                        features=self.features,
+                        data=self.data_par_train, transform=train_transforms
+                    )
         else:
             train_ds = CacheDataset(
                 config=self.config,
                 features=self.features,
                 data=self.data_par_train,
                 transform=train_transforms,
                 copy_cache=True,
```

### Comparing `miacag-0.0.81/miacag/dataloader/Classification/_3D/dataset_mil.py` & `miacag-0.0.82/miacag/dataloader/Classification/_3D/dataset_mil.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/Classification/get_dataloader_classification.py` & `miacag-0.0.82/miacag/dataloader/Classification/get_dataloader_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,28 +55,36 @@
                     from miacag.dataloader.Classification._3D.dataloader_monai_classification_3D_mil import \
                         train_monai_classification_loader
                     from miacag.dataloader.Classification._3D.dataloader_monai_classification_3D_mil import \
                         val_monai_classification_loader
                 elif config['model']['dimension'] in ['2D']:
                     from miacag.dataloader.Classification._2D.dataloader_monai_classification_2D_mil import \
                         train_monai_classification_loader, val_monai_classification_loader
+                elif config['model']['dimension'] in ['1D']:
+                    from miacag.dataloader.Classification._1D.Feature_vector_dataset import \
+                        train_monai_classification_loader, val_monai_classification_loader
                 else:
                     raise ValueError('model dimension is not implemented')
         elif config['loaders']['format'] in ['db']:
             from \
                 miacag.dataloader.Classification.tabular.dataloader_monai_classification_tabular import \
                 train_monai_classification_loader, val_monai_classification_loader
         elif config['loaders']['format'] in ['dicom_db']:
             print('NOT implemented')
         else:
             raise ValueError("Invalid validation moode %s" % repr(
                     config['loaders']['val_method']['type']))
+       # if config['model']['dimension'] != '1D':
         train_ds = train_monai_classification_loader(
             self.train_df,
             config)
+        # else:
+        #     from miacag.dataloader.Classification._1D.Feature_vector_dataset import FeatureVectorDataset
+        #     train_ds = FeatureVectorDataset(self.train_df, config)
+            
 
 
         if config['weighted_sampler'] == 'True':
             weights = train_ds.weights
             train_ds = train_ds()
             sampler = DistributedWeightedRandomSampler(
                 dataset=train_ds,
```

### Comparing `miacag-0.0.81/miacag/dataloader/DistributedWeightedSampler.py` & `miacag-0.0.82/miacag/dataloader/DistributedWeightedSampler.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/Representation/get_dataloader_representation.py` & `miacag-0.0.82/miacag/dataloader/Representation/get_dataloader_representation.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/dataloader_base.py` & `miacag-0.0.82/miacag/dataloader/dataloader_base.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/dataloader/dataloader_base_monai.py` & `miacag-0.0.82/miacag/dataloader/dataloader_base_monai.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,27 +372,31 @@
     def maybeNormalize(self):
         if self.config['model']['backbone'] in [
             'x3d_s', 'slowfast8x8', "mvit_base_16x4", 'mvit_base_32x3', 'debug_3d',
             "pretrain_videomae_base_patch16_224",
             'pretrain_videomae_small_patch16_224',
             "vit_base_patch16_224", 
             "vit_large_patch16_224", 
-            "vit_small_patch16_224"]:
+            "vit_small_patch16_224",
+            'vit_base_patch16',
+            'vit_small_patch16',
+            'vit_large_patch16',
+            'vit_huge_patch14']:
             normalize = NormalizeIntensityd(
                 keys=self.features,
                 subtrahend=(0.45, 0.45, 0.45),#(0.43216, 0.394666, 0.37645),
                 divisor=(0.225, 0.225, 0.225),#(0.22803, 0.22145, 0.216989),
                 channel_wise=True)
         elif self.config['model']['backbone'] == 'r2plus1_18':
             normalize = NormalizeIntensityd(
                 keys=self.features,
                 subtrahend=(0.43216, 0.394666, 0.37645),
                 divisor=(0.22803, 0.22145, 0.216989),
                 channel_wise=True)
-        elif self.config['model']['backbone'] in ['r50']:
+        elif self.config['model']['backbone'] in ['r50', 'dinov2_vits14']:
             normalize = NormalizeIntensityd(
                 keys=self.features,
                 subtrahend=(0.485, 0.456, 0.406),
                 divisor=(0.229, 0.224, 0.225),
                 channel_wise=True)
         else:
             raise ValueError('not implemented')
```

### Comparing `miacag-0.0.81/miacag/dataloader/get_dataloader.py` & `miacag-0.0.82/miacag/dataloader/get_dataloader.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/metrics/cumulativeSumming.py` & `miacag-0.0.82/miacag/metrics/cumulativeSumming.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/metrics/metrics.py` & `miacag-0.0.82/miacag/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/metrics/metrics_utils.py` & `miacag-0.0.82/miacag/metrics/metrics_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     else:
         loss_types = config['loss']['groups_names'] + ['total']
         for c_idx, loss_type in enumerate(loss_types):
             metrics_labels.append(loss_type)
     return metrics_labels
 
 
-def init_metrics(metrics, config, ptype=None):
+def init_metrics(metrics, config, device, ptype=None):
     metrics = getMetricForEachLabel(metrics, config, ptype)
     dicts = {}
     keys = [0.0] * len(metrics)
     idx = range(len(keys))
     for i in idx:
         if metrics[i].startswith('CE'):
             dicts[metrics[i]] = CumulativeAverage()
@@ -119,14 +119,16 @@
         elif metrics[i].startswith('acc_top_1'):
             dicts[metrics[i]] = ConfusionMatrixMetric(
                 metric_name='accuracy', reduction="mean",
                 include_background=False)
         else:
             raise NotImplementedError(
                 'This metric {} is not implemented!'.format(metrics[i]))
+        #dicts[metrics[i]].count = dicts[metrics[i]].count.to(device)
+        #dicts[metrics[i]].sum = dicts[metrics[i]].sum.to(device)
     return dicts
 
 
 def write_tensorboard(losses, metrics, writer, tb_step_writer, phase):
     if torch.distributed.get_rank() == 0:
         for loss in losses:
             writer.add_scalar("{}/{}".format(loss, phase),
@@ -137,16 +139,18 @@
                               metrics[metric],
                               tb_step_writer)
     return losses, metrics
 
 
 def remove_nans(labels, outputs):
     mask = labels == 99998
-    labels = labels[~mask]
-    outputs = outputs[~mask]
+    mask_outputs = torch.unsqueeze(mask, 1).repeat(1, outputs.shape[1])
+
+    labels = labels.masked_select(~mask_outputs)
+    outputs = outputs.masked_select(~mask_outputs)
     mask_nan = torch.isnan(labels)
     labels = labels[~mask_nan]
     outputs = outputs[~mask_nan]
     return labels, outputs
 
 
 def get_metrics(outputs,
@@ -159,15 +163,15 @@
                 num_classes):
     
     #metrics_dicts = {}
     for metric in metrics:
         if metric.endswith(label_name):
             c = 0
             if metric.startswith('acc_top_1'):
-                labels, outputs = remove_nans(labels, outputs)
+            #    labels, outputs = remove_nans(labels, outputs)
                 if outputs.nelement() != 0:
                     labels = F.one_hot(
                         labels,
                         num_classes=num_classes)
                     if metric.startswith('acc_top_1_BCE'):
                         outputs = torch.nn.Sigmoid()(outputs)
                         outputs = (outputs >= 0.5).float()
@@ -300,28 +304,34 @@
         running_loss,
         losses,
         losses_metric
         )
     return metrics, losses_metric
 
 
-def normalize_metrics(running_metrics):
+def normalize_metrics(running_metrics, device):
     metric_dict = {}
     for running_metric in running_metrics:
         if running_metric.startswith('CE'):
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('BCE'):
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('total'):
+            running_metrics[running_metric].val = running_metrics[running_metric].val.to(device)
+            running_metrics[running_metric].count = running_metrics[running_metric].count.to(device)# Move to GPU memory if available
+            running_metrics[running_metric].sum = running_metrics[running_metric].sum.to(device)
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('RMSE'):
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('MSE'):
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('L1smooth'):
+            running_metrics[running_metric].val = running_metrics[running_metric].val.to(device)
+            running_metrics[running_metric].count = running_metrics[running_metric].count.to(device)# Move to GPU memory if available
+            running_metrics[running_metric].sum = running_metrics[running_metric].sum.to(device)
             metric_tb = running_metrics[running_metric].aggregate().item()
         elif running_metric.startswith('_L1'):
             metric_tb = running_metrics[running_metric].aggregate().item()
         else:
             metric_tb = running_metrics[running_metric].aggregate()[0].item()
         metric_dict[running_metric] = metric_tb
         running_metrics[running_metric].reset()
```

### Comparing `miacag-0.0.81/miacag/model_utils/GradCam_model.py` & `miacag-0.0.82/miacag/model_utils/GradCam_model.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/model_utils/eval_utils.py` & `miacag-0.0.82/miacag/model_utils/eval_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,18 +195,18 @@
             saliency_maps,
             running_metric_val, running_loss_val)
     running_metric_val, running_loss_val, _, _ = eval_outputs
 
     # Normalize the metrics from the entire epoch
     if config['task_type'] != "representation_learning":
         running_metric_val, metric_tb = normalize_metrics(
-            running_metric_val)
+            running_metric_val, device)
 
     running_loss_val, loss_tb = normalize_metrics(
-        running_loss_val)
+        running_loss_val, device)
 
     if writer is not False:
         loss_tb, metric_tb = write_tensorboard(
             loss_tb,
             metric_tb,
             writer, epoch, 'val')
 
@@ -229,32 +229,33 @@
         running_metric_val, running_loss_val, df_result_i, _ = eval_outputs
 
         df_result = pd.concat(
                         [df_result, df_result_i], ignore_index=True)
 
     if config['task_type'] != "representation_learning":
         running_metric_val, metric_tb = normalize_metrics(
-            running_metric_val)
+            running_metric_val, device)
 
     running_loss_val, loss_tb = normalize_metrics(
-        running_loss_val)
+        running_loss_val, device)
     df_result = maybe_softmax_transform(df_result, config)
     return metric_tb, df_result
 
 
 def maybe_softmax_transform(df, config):
     cols = df.columns
     # remove rowid from the list
     cols = cols.drop('rowid')
     logits_return = []
     for c, logit in enumerate(cols):
         logit_conf = logit + '_confidence'
         if config['loss']['name'][c].startswith('CE'):
-            raise(ValueError('this transform is not implemented'))
-            logits_return.append(softmax_transform(logit.float()))
+            df[logit_conf] = df[logit]
+            #raise(ValueError('this transform is not implemented'))
+            df[logit_conf] = softmax_transform(torch.tensor(df[logit])).tolist()
         elif config['loss']['name'][c] == 'MSE':
             logits_return.append(logit.float())
         elif config['loss']['name'][c] in ['_L1', 'L1smooth']:
             df[logit_conf] = df[logit]
         elif config['loss']['name'][c].startswith('BCE'):
             logits_return.append(torch.nn.Sigmoid()(logit.float()))
         else:
```

### Comparing `miacag-0.0.81/miacag/model_utils/get_loss_func.py` & `miacag-0.0.82/miacag/model_utils/get_loss_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 #     # Compute the loss as the mean of the smooth L1 loss over all samples
 #     return diff.mean()
 
 def l1_loss_smooth(predictions, targets, beta=1):
     mask = torch.isnan(targets)
     loss = 0
-    predictions = predictions[~mask]
+    #predictions = predictions[~mask]
+    predictions = predictions.masked_select(~mask)
     targets = targets[~mask]
     if predictions.shape[0] != 0:
         for x, y in zip(predictions, targets):
             if abs(x-y) < beta:
                 loss += (0.5*(x-y)**2 / beta).mean()
             else:
                 loss += (abs(x-y) - 0.5 * beta).mean()
```

### Comparing `miacag-0.0.81/miacag/model_utils/get_optimizer.py` & `miacag-0.0.82/miacag/model_utils/get_optimizer.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/model_utils/get_test_pipeline.py` & `miacag-0.0.82/miacag/model_utils/get_test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,16 @@
         return conf_list_tuple
 
     def tuple2key(self, t, delimiter=u';'):
         return delimiter.join(t)
 
     def saveCsvFiles(self, label_name, df, config, count):
         if config['loss']['name'][count].startswith('CE'):
-            confidences = confidences[count]
+            confidences = label_name + '_confidence'
+           # confidences = confidences[count]
             confidence_col = [
                 label_name + '_confidence_' +
                 str(i) for i in range(0, config['model']['num_classes'][count])]
         else:
             confidences = label_name + '_confidence'
          #   df[confidences] = np.expand_dims(df[confidences], 1)
             confidence_col = [
@@ -207,14 +208,20 @@
         label_name_csv_files = os.path.join(csv_files, label_name)
         mkFolder(label_name_csv_files)
         array = np.concatenate(
             (np.expand_dims(df[confidences].to_numpy(), 1),
              np.expand_dims(df["rowid"].to_numpy(), 1)), axis=1)
       
         cols = confidence_col + ['rowid']
+        if config['loss']['name'][count].startswith('CE'):
+            # convert array with rows with liusts to liste
+            liste = []
+            for i in range(0, config['model']['num_classes'][count]):
+                liste.append(array[i, 0] + [array[i,1]])
+            array = liste
         df = pd.DataFrame(
             array,
             columns=cols)
         df.to_csv(
             os.path.join(label_name_csv_files, str(torch.distributed.get_rank()))+'.csv')
         return csv_files
       #  df.to_csv()
```

### Comparing `miacag-0.0.81/miacag/model_utils/grad_cam_utils.py` & `miacag-0.0.82/miacag/model_utils/grad_cam_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/model_utils/predict_utils.py` & `miacag-0.0.82/miacag/model_utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/model_utils/scheduler.py` & `miacag-0.0.82/miacag/model_utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/model_utils/siam_loss.py` & `miacag-0.0.82/miacag/model_utils/siam_loss.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/model_utils/train_utils.py` & `miacag-0.0.82/miacag/model_utils/train_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,17 @@
         #                                          metrics)
        # running_loss_train = increment_metrics(running_loss_train, loss)
     
     if lr_scheduler is not False:
         lr_scheduler.step()
 
     running_metric_train, metric_tb = normalize_metrics(
-        metrics)
+        metrics, device)
     running_loss_train, loss_tb = normalize_metrics(
-        loss_metric)
+        loss_metric, device)
     # running_loss_train = normalize_metrics(
     #     running_loss_train,
     #     config,
     #     len(train_loader.dataset.data)
     #     if config['cache_num'] == 'None' else config['cache_num_train'])
 
     loss_tbe, metric_tb = write_tensorboard(loss_tb,
```

### Comparing `miacag-0.0.81/miacag/models/BuildModel.py` & `miacag-0.0.82/miacag/models/BuildModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import yaml
 import torch
 import os
-
+from miacag.models.milmodel_from_features import MILModel
 
 class ModelBuilder():
     def __init__(self, config, device):
         self.config = config
         self.device = device
 
     def getFingerPrint(self, filename):
@@ -59,28 +59,21 @@
                 pass
             else:
                 new_state.pop(key, None)
         return new_state
 
     def get_ImageToScalar_model(self):
         path_model = self.config['model']['pretrain_model']
-        # if self.config['task_type'] == "regression":
-        #     from miacag.models.modules import RegressionModel as m
-        # elif self.config['task_type'] == "classification":
-        #     from miacag.models.modules import ClassificationModel as m
         if self.config['task_type'] in ["classification", "regression"]:
             from miacag.models.modules import ImageToScalarModel as m
         elif self.config['task_type'] in ["mil_classification"]:
             from miacag.models.milmodel3d import MILModel as m
         model = m(self.config, self.device)
         model = self.get_mayby_DDP(model)
-        # if path_encoder != 'None':
-        #     state = torch.load(os.path.join(path_encoder, 'model.pt'))
-        #     state = self.drop_not_encoder_modules(state)
-        #     model.module.load_state_dict(state)
+
         if self.config['loaders']['mode'] in ['testing', 'prediction']:
             if path_model != 'None':
                 if self.config["use_DDP"] == "False":
                     #if self.config['use_DDP'] == 'True':
                     model.load_state_dict(
                         torch.load(os.path.join(path_model, 'model.pt')))
                 else:
@@ -137,14 +130,26 @@
     def get_model(self):
         if self.config['task_type'] == "representation_learning":
             model = self.get_representation_learning_model()
         elif self.config['task_type'] in ["classification", "regression", "mil_classification"]:
             model = self.get_ImageToScalar_model()
         elif self.config['task_type'] == "segmentation":
             model = self.get_segmentation_model()
+        else:
+            raise ValueError('model not implemented')
+        # maybe freeze backbone
+        if self.config['model']['freeze_backbone']:
+            for param in model.module.parameters():
+                param.requires_grad = False
+        #else:
+         #   if self.config['model']['model_name'] in "dinov2_vits14":
+            for param in model.module.fcs.parameters():
+                param.requires_grad = True
+            for param in model.module.attention.parameters():
+                param.requires_grad = True
         return model
 
     def __call__(self):
         if self.config['datasetFingerprintFile'] is not None:
             self.config = self.unpack_fingerprint(self.config)
         model = self.get_model()
         return model
```

### Comparing `miacag-0.0.81/miacag/models/cnns.py` & `miacag-0.0.82/miacag/models/cnns.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/models/get_encoder.py` & `miacag-0.0.82/miacag/models/get_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from monai.networks import nets
 from torch import nn
 import torch
 import os
-from timm.models import create_model
-from models import modeling_finetune
+from dinov2.models.vision_transformer import \
+    vit_large, vit_small
+#from timm.models import create_model
+#from models import modeling_finetune
 from collections import OrderedDict
-
+#from miacag.models.milmodel_from_features import MILModel
 
 class Identity(nn.Module):
     def __init__(self):
         super(Identity, self).__init__()
 
     def forward(self, x):
         return x
@@ -129,14 +131,24 @@
         "vit_large_patch16_224",
         "vit_small_patch16_224"]:
         model = get_model(config)
         model.head = Identity()
         in_features = model.fc_norm.normalized_shape[0]
         if config['loaders']['mode'] != 'testing':
             model = getPretrainedWeights(config, model, device)
+            
+    elif config['model']['backbone'] in ['vit_small_patch16',
+            'vit_base_patch16', 'vit_large_patch16']:
+        import miacag.models.mae_st_util.models_vit as models_vit
+        config['num_frames'] = config['loaders']['Crop_depth']
+        model = models_vit.__dict__[config['model']['backbone']](**config)
+        in_features = model.head.in_features
+        model.head = Identity()
+      #  print('not implemented jet'    )
+        
     elif config['model']['backbone'] == 'linear':
         from miacag.models.backbone_encoders.tabular.base_encoders \
             import LinearEncoder
         model = LinearEncoder(config['model']['incomming_features'])
         in_features = config['model']['incomming_features']
 
     elif config['model']['backbone'] == 'mlp':
@@ -152,28 +164,43 @@
         in_features = model.fc.in_features
         model = nn.Sequential(*list(model.children())[:-2])
     elif config['model']['backbone'] == 'debug_3d':
         from miacag.models.cnns import debug_3d
         in_features = 16
         model = debug_3d(in_features)
         model = getPretrainedWeights(config, model, device)
-        
+    elif config['model']['backbone'] == 'dinov2_vits14':
+        model = vit_small(
+                patch_size=14,
+                img_size=config['loaders']['Resize_height'],
+                init_values=1.0,
+                block_chunks=0)
+        model = getPretrainedWeights(config, model, device)
+        in_features = model.norm.normalized_shape[0]
+       
     else:
         raise ValueError('not implemented')
+
+            
     return model, in_features
 
 
 def modelsRequiredPermute():
     model_list = [
         'r3d_18', 'r2plus1_18',
         'x3d_l', 'x3d_s', "mvit_base_16x4", 'mvit_base_32x3', 'slowfast8x8',
         'pretrain_videomae_base_patch16_224',
         'vit_base_patch16_224',
         "vit_large_patch16_224", 
-        "vit_small_patch16_224"]
+        "vit_small_patch16_224",
+        "vit_small_patch16",
+        "vit_base_patch16",
+        "vit_large_patch16",
+        "vit_huge_patch14",
+        ]
     return model_list
 
 
 # from VideoMAE
 
 def get_model(config):
     print(f"Creating model: {config['model']['backbone']}")
```

### Comparing `miacag-0.0.81/miacag/models/milmodel3d.py` & `miacag-0.0.82/miacag/models/milmodel3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,11 +306,12 @@
     def reduce_feature_space(self, x):
         if self.config['model']['dimension'] in ['3D', '2D+T']:
             if self.config['model']['backbone'] not in ["mvit_base_16x4", "mvit_base_32x3"]:
                 x = x.mean(dim=(-3, -2, -1))
             else:
                 pass
         elif self.config['model']['dimension'] in ['2D']:
-            x = x.mean(dim=(-2, -1))
+            if self.config['model']['backbone'] not in ["dinov2_vits14"]:
+                x = x.mean(dim=(-2, -1))
         else:
             raise ValueError('this dimension is not implemented')
         return x
```

### Comparing `miacag-0.0.81/miacag/models/mlps.py` & `miacag-0.0.82/miacag/models/mlps.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/models/modeling_finetune.py` & `miacag-0.0.82/miacag/models/modeling_finetune.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/models/modeling_pretrain.py` & `miacag-0.0.82/miacag/models/modeling_pretrain.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/models/modules.py` & `miacag-0.0.82/miacag/models/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,47 +140,52 @@
             #     num_classes = get_num_class_for_loss_group(
             #         self.config['loss']['name'],
             #         loss_type, self.config['model']['num_classes'])
             count_loss = self.config['loss']['groups_counts'][loss_count_idx]
             if loss_type.startswith('CE'):
                 self.fcs.append(nn.Linear(
                         self.in_features,
-                        num_classes).to(device))
+                        config['model']['num_classes'][loss_count_idx]).to(device))
             elif loss_type.startswith(tuple(['BCE_multilabel'])):
                 self.fcs.append(
                     nn.Sequential(
-                        nn.Linear(
-                            self.in_features, self.in_features),
+                        # nn.Linear(
+                        #     self.in_features, self.in_features),
                         nn.Linear(
                             self.in_features, count_loss)
                         ).to(device))
             # test if loss_type startswith three conditions
             
             elif loss_type.startswith(tuple(['MSE', '_L1', 'L1smooth'])):
                 # if config['model']['sigm'] == 'True':
                 self.fcs.append(
                     nn.Sequential(
-                        nn.Linear(
-                            self.in_features, self.in_features),
+                        # nn.Linear(
+                        #     self.in_features, self.in_features),
                         nn.Linear(
                             self.in_features,
                             count_loss).to(device)
                         ))
  
             else:
                 raise ValueError('loss not implemented')
+            
+        
         self.dimension = config['model']['dimension']
-
+        
+        
     def forward(self, x):
         x = maybePermuteInput(x, self.config)
         p = self.encoder(x)
         if self.dimension in ['3D', '2D+T']:
             if self.config['model']['backbone'] not in [
                 "mvit_base_16x4", "mvit_base_32x3", "vit_base_patch16_224",
-                "vit_small_patch16_224", "vit_large_patch16_224"]:
+                "vit_small_patch16_224", "vit_large_patch16_224",
+                "vit_base_patch16", "vit_small_patch16", "vit_large_patch16",
+                "vit_huge_patch14"]:
                 p = p.mean(dim=(-3, -2, -1))
             else:
                 pass
         elif self.dimension == 'tabular':
             p = p
         else:
             p = p.mean(dim=(-2, -1))
```

### Comparing `miacag-0.0.81/miacag/models/pretrained_vit.py` & `miacag-0.0.82/miacag/models/pretrained_vit.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/plots/angle_plotter.py` & `miacag-0.0.82/miacag/plots/angle_plotter.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/plots/plot_histogram.py` & `miacag-0.0.82/miacag/plots/plot_histogram.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/plots/plot_roc_auc_all.py` & `miacag-0.0.82/miacag/plots/plot_roc_auc_all.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/plots/plot_scatter.py` & `miacag-0.0.82/miacag/plots/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/plots/plot_test.py` & `miacag-0.0.82/miacag/plots/plot_test.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/plots/plotter.py` & `miacag-0.0.82/miacag/plots/plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 from miacag.utils.sql_utils import getDataFromDatabase
 from sklearn.metrics import mean_squared_error
 from sklearn.metrics import mean_absolute_error
 
 from sklearn.metrics import f1_score, \
-     accuracy_score, confusion_matrix, plot_confusion_matrix
+     accuracy_score, confusion_matrix#, plot_confusion_matrix
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 from matplotlib import ticker
 import matplotlib
 from matplotlib.ticker import MaxNLocator
 matplotlib.use('Agg')
@@ -370,42 +370,43 @@
 def wrap_plot_all_sten_reg(df, label_names, confidence_names, output_plots,
                            group_aggregated, config):
     threshold_ffr = config['loaders']['val_method']['threshold_ffr']
     threshold_sten = config['loaders']['val_method']['threshold_sten']
     df_sten = df.copy()
     sten_cols_conf = select_relevant_columns(confidence_names, 'sten')
     sten_cols_true = select_relevant_columns(label_names, 'sten')
-    if not group_aggregated:
-        for sten_col_conf in sten_cols_conf:
-            df_sten[sten_col_conf] = convertConfFloats(
-                df[sten_col_conf],
-                config['loss']['name'][0])
-    sten_trues_concat = []      
-    sten_conf_concat = []  
-    #concantenating all stenosis columns
-    # df_sten['stenosis'] = []
-    for idx, label in enumerate(sten_cols_true):
-        sten_trues_concat.append(df_sten[label])
-        sten_conf_concat.append(df_sten[sten_cols_conf[idx]])
-    stenosis = pd.concat(
-        [pd.concat(sten_trues_concat), pd.concat(sten_conf_concat)],
-        axis=1)
-    if len(sten_cols_true) >= 2:
-        plot_col = [0, 1]
-    else:
-        plot_col = [sten_cols_true[0], sten_cols_conf[0]]
+    if len(sten_cols_conf) > 0:
+        if not group_aggregated:
+            for sten_col_conf in sten_cols_conf:
+                df_sten[sten_col_conf] = convertConfFloats(
+                    df[sten_col_conf],
+                    config['loss']['name'][0])
+        sten_trues_concat = []      
+        sten_conf_concat = []  
+        #concantenating all stenosis columns
+        # df_sten['stenosis'] = []
+        for idx, label in enumerate(sten_cols_true):
+            sten_trues_concat.append(df_sten[label])
+            sten_conf_concat.append(df_sten[sten_cols_conf[idx]])
+        stenosis = pd.concat(
+            [pd.concat(sten_trues_concat), pd.concat(sten_conf_concat)],
+            axis=1)
+        if len(sten_cols_true) >= 2:
+            plot_col = [0, 1]
+        else:
+            plot_col = [sten_cols_true[0], sten_cols_conf[0]]
 
-    plot_regression_density(x=stenosis[plot_col[0]], y=stenosis[plot_col[1]],
-                            cmap='jet', ylab='prediction', xlab='true',
-                            bins=100,
-                            figsize=(5, 4),
-                            snsbins=60,
-                            plot_type='stenosis',
-                            output_folder=output_plots,
-                            label_name_ori='sten_all')
+        plot_regression_density(x=stenosis[plot_col[0]], y=stenosis[plot_col[1]],
+                                cmap='jet', ylab='prediction', xlab='true',
+                                bins=100,
+                                figsize=(5, 4),
+                                snsbins=60,
+                                plot_type='stenosis',
+                                output_folder=output_plots,
+                                label_name_ori='sten_all')
     df_ffr = df.copy()
     ffr_cols_true = select_relevant_columns(label_names, 'ffr')
     if len(ffr_cols_true) > 0:
         ffr_cols_conf = select_relevant_columns(confidence_names, 'ffr')
         if not group_aggregated:
             for ffr_col_conf in ffr_cols_conf:
                 df_ffr[ffr_col_conf] = convertConfFloats(
@@ -445,23 +446,24 @@
     #     threshold_ffr = 0.5
     #     threshold_sten = 0.5
 
         
     df_sten = df.copy()
     sten_cols_conf = select_relevant_columns(confidence_names, 'sten')
     sten_cols_true = select_relevant_columns(label_names, 'sten')
-    if not group_aggregated:
-        for sten_col_conf in sten_cols_conf:
-            df_sten[sten_col_conf] = convertConfFloats(
-                df[sten_col_conf],
-                config['loss']['name'][0])
-    plot_roc_all(df_sten, sten_cols_true, sten_cols_conf, output_plots,
-                 plot_type='stenosis',
-                 config=config,
-                 theshold=threshold_sten)
+    if len(sten_cols_true) > 0:
+        if not group_aggregated:
+            for sten_col_conf in sten_cols_conf:
+                df_sten[sten_col_conf] = convertConfFloats(
+                    df[sten_col_conf],
+                    config['loss']['name'][0])
+        plot_roc_all(df_sten, sten_cols_true, sten_cols_conf, output_plots,
+                    plot_type='stenosis',
+                    config=config,
+                    theshold=threshold_sten)
     df_ffr = df.copy()
     ffr_cols_true = select_relevant_columns(label_names, 'ffr')
     if len(ffr_cols_true) > 0:
         ffr_cols_conf = select_relevant_columns(confidence_names, 'ffr')
         if not group_aggregated:
             for ffr_col_conf in ffr_cols_conf:
                 df_ffr[ffr_col_conf] = convertConfFloats(
@@ -483,16 +485,19 @@
 
 def plot_results(sql_config, label_names, prediction_names, output_plots,
                  num_classes, config, confidence_names,
                  group_aggregated=False):
     df, _ = getDataFromDatabase(sql_config)
     if group_aggregated:
         confidence_names = [c + '_aggregated' for c in confidence_names]
+    # test if a element is a list starts with a string: "sten"
+    stens = select_relevant_columns(label_names, 'sten')
+    
     wrap_plot_all_sten_reg(df, label_names, confidence_names, output_plots,
-                           group_aggregated, config)    
+                        group_aggregated, config)    
     wrap_plot_all_roc(df, label_names, confidence_names, output_plots,
                       group_aggregated,
                       config=config)
 
     for c, label_name in enumerate(label_names):
         confidence_name = confidence_names[c]
         prediction_name = prediction_names[c]
```

### Comparing `miacag-0.0.81/miacag/plots/query_plot_agg_max.py` & `miacag-0.0.82/miacag/plots/query_plot_agg_max.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/postprocessing/aggregate_pr_group.py` & `miacag-0.0.82/miacag/postprocessing/aggregate_pr_group.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/postprocessing/append_results.py` & `miacag-0.0.82/miacag/postprocessing/append_results.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/postprocessing/count_stenosis_pr_group.py` & `miacag-0.0.82/miacag/postprocessing/count_stenosis_pr_group.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/postprocessing/estimate_vessel_disease.py` & `miacag-0.0.82/miacag/postprocessing/estimate_vessel_disease.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/predictor.py` & `miacag-0.0.82/miacag/predictor.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/add_columns.py` & `miacag-0.0.82/miacag/preprocessing/add_columns.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/copy_column.py` & `miacag-0.0.82/miacag/preprocessing/copy_column.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/copy_table.py` & `miacag-0.0.82/miacag/preprocessing/copy_table.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/datasetFingerprint.py` & `miacag-0.0.82/miacag/preprocessing/datasetFingerprint.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/labels_map.py` & `miacag-0.0.82/miacag/preprocessing/labels_map.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/pre_process.py` & `miacag-0.0.82/miacag/preprocessing/pre_process.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/process_labels/process_dominance.py` & `miacag-0.0.82/miacag/preprocessing/process_labels/process_dominance.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/process_labels/process_total_occ.py` & `miacag-0.0.82/miacag/preprocessing/process_labels/process_total_occ.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/split_train_val.py` & `miacag-0.0.82/miacag/preprocessing/split_train_val.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/transform_missing_floats.py` & `miacag-0.0.82/miacag/preprocessing/transform_missing_floats.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/transform_stenosis.py` & `miacag-0.0.82/miacag/preprocessing/transform_stenosis.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/transform_thresholds.py` & `miacag-0.0.82/miacag/preprocessing/transform_thresholds.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/transform_total_occlusion.py` & `miacag-0.0.82/miacag/preprocessing/transform_total_occlusion.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/preprocessing/utils/check_experiments.py` & `miacag-0.0.82/miacag/preprocessing/utils/check_experiments.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/scripts/aggregate_and_plot.py` & `miacag-0.0.82/miacag/scripts/aggregate_and_plot.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/scripts/angiography_classifier/predict_angio.py` & `miacag-0.0.82/miacag/scripts/angiography_classifier/predict_angio.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
             "--local_rank", type=int,
             help="Local rank: torch.distributed.launch.")    
 parser.add_argument(
+            "--local-rank", type=int,
+            help="Local rank: torch.distributed.launch.")
+parser.add_argument(
             "--num_workers", type=int,
             help="Number of cpu workers for training")
 parser.add_argument(
     '--config_path', type=str,
     help="path to folder with config files")
 parser.add_argument(
     "--model_path", type=str,
```

### Comparing `miacag-0.0.81/miacag/scripts/angiography_classifier/submit_angio.py` & `miacag-0.0.82/miacag/scripts/angiography_classifier/submit_angio.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 parser = argparse.ArgumentParser(
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
             "--local_rank", type=int,
-            help="Local rank: torch.distributed.launch.")    
+            help="Local rank: torch.distributed.launch.")
+parser.add_argument(
+            "--local-rank", type=int,
+            help="Local rank: torch.distributed.launch.")
 parser.add_argument(
             "--num_workers", type=int,
             help="Number of cpu workers for training")
 parser.add_argument(
     '--config_path', type=str,
     help="path to folder with config files")
```

### Comparing `miacag-0.0.81/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py` & `miacag-0.0.82/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 parser = argparse.ArgumentParser(
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
             "--local_rank", type=int,
-            help="Local rank: torch.distributed.launch.")    
+            help="Local rank: torch.distributed.launch.")
+parser.add_argument(
+            "--local-rank", type=int,
+            help="Local rank: torch.distributed.launch.")
 parser.add_argument(
             "--num_workers", type=int,
             help="Number of cpu workers for training")    
 parser.add_argument(
     '--config_path_lca_rca', type=str,
     help="path to folder with config files")
 parser.add_argument(
```

### Comparing `miacag-0.0.81/miacag/scripts/compare_PCI_notPCI.py` & `miacag-0.0.82/miacag/scripts/compare_PCI_notPCI.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/scripts/predict_patologi_eyeball_vs_estimated.py` & `miacag-0.0.82/miacag/scripts/predict_patologi_eyeball_vs_estimated.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/scripts/stenosis_identifier/submit_angio.py` & `miacag-0.0.82/miacag/scripts/stenosis_identifier/submit_angio.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,18 @@
 parser = argparse.ArgumentParser(
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
             "--local_rank", type=int,
-            help="Local rank: torch.distributed.launch.")    
+            help="Local rank: torch.distributed.launch.")
+parser.add_argument(
+            "--local-rank", type=int,
+            help="Local rank: torch.distributed.launch.")
 parser.add_argument(
             "--num_workers", type=int,
             help="Number of cpu workers for training")    
 parser.add_argument(
     '--config_path', type=str,
     help="path to folder with config files")
```

### Comparing `miacag-0.0.81/miacag/scripts/stenosis_identifier_mil/submit_angio.py` & `miacag-0.0.82/miacag/scripts/stenosis_identifier_mil/submit_angio.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,18 @@
 parser = argparse.ArgumentParser(
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
             "--local_rank", type=int,
-            help="Local rank: torch.distributed.launch.")    
+            help="Local rank: torch.distributed.launch.")
+parser.add_argument(
+            "--local-rank", type=int,
+            help="Local rank: torch.distributed.launch.")
 parser.add_argument(
             "--num_workers", type=int,
             help="Number of cpu workers for training")    
 parser.add_argument(
     '--config_path', type=str,
     help="path to folder with config files")
```

### Comparing `miacag-0.0.81/miacag/scripts/stenosis_regression/submit_angio.py` & `miacag-0.0.82/miacag/scripts/stenosis_regression/submit_angio.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
     "--local_rank", type=int,
     help="Local rank: torch.distributed.launch.")
 parser.add_argument(
+            "--local-rank", type=int,
+            help="Local rank: torch.distributed.launch.")
+parser.add_argument(
     "--num_workers", type=int,
     help="Number of cpu workers for training")
 parser.add_argument(
     '--config_path', type=str,
     help="path to folder with config files")
```

### Comparing `miacag-0.0.81/miacag/scripts/stenosis_regression_full/submit_angio.py` & `miacag-0.0.82/miacag/scripts/stenosis_regression_full/submit_angio.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 parser.add_argument(
     '--cpu', type=str,
     help="if cpu 'True' else 'False'")
 parser.add_argument(
             "--local_rank", type=int,
             help="Local rank: torch.distributed.launch.")    
 parser.add_argument(
+            "--local-rank", type=int,
+            help="Local rank: torch.distributed.launch.")
+parser.add_argument(
             "--num_workers", type=int,
             help="Number of cpu workers for training")    
 parser.add_argument(
     '--config_path_stenosis_rca_r_dom', type=str,
     help="path to folder with config files")
 parser.add_argument(
     '--config_path_stenosis_rca_l_dom', type=str,
```

### Comparing `miacag-0.0.81/miacag/tester.py` & `miacag-0.0.82/miacag/tester.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,20 @@
     test_loader = get_dataloader_test(config)
 
     # Get loss func
     criterion = get_loss_func(config)
     config['loss']['name'] = config['loss']['name'] + ['total']
     running_loss_test = init_metrics(config['loss']['name'],
                                      config,
+                                     device,
                                      ptype='loss')
     running_metric_test = init_metrics(
                 config['eval_metric_val']['name'],
-                config)
+                config,
+                device)
 
     pipeline = TestPipeline()
     pipeline.get_test_pipeline(model, criterion, config, test_loader,
                                device, init_metrics,
                                normalize_metrics,
                                running_metric_test, running_loss_test)
```

### Comparing `miacag-0.0.81/miacag/tests/test_sql_utils.py` & `miacag-0.0.82/miacag/tests/test_sql_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/trainer.py` & `miacag-0.0.82/miacag/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
         torch.cuda.set_device(device)
         torch.backends.cudnn.benchmark = True
 
     # Get metrics
     config['loss']['groups_names'], config['loss']['groups_counts'], \
         config['loss']['group_idx'], config['groups_weights'] \
         = get_loss_names_groups(config)
-    running_loss_train = init_metrics(config['loss']['name'], config,
+    running_loss_train = init_metrics(config['loss']['name'], config, device,
                                       ptype='loss')
     running_metric_train = init_metrics(
-            config['eval_metric_train']['name'], config)
-    running_loss_val = init_metrics(config['loss']['name'], config,
+            config['eval_metric_train']['name'], config, device)
+    running_loss_val = init_metrics(config['loss']['name'], config, device,
                                     ptype='loss')
     running_metric_val = init_metrics(
-                config['eval_metric_val']['name'], config)
+                config['eval_metric_val']['name'], config, device)
 
     # Get model
     BuildModel = ModelBuilder(config, device)
     model = BuildModel()
 
     # Get data loaders
     train_loader, val_loader, train_ds, _ = get_dataloader_train(config)
```

### Comparing `miacag-0.0.81/miacag/utils/common_utils.py` & `miacag-0.0.82/miacag/utils/common_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,25 @@
 
 
 #
 def wrap_outputs_to_dict(outputs, config):
     outputs_dict = {}
     for group_count, group in enumerate(config['loss']['groups_names']):
         outputs_group = outputs[group_count]
-        for segment_idx in range(0, outputs_group.shape[-1]):
-            output_segment = outputs_group[:, segment_idx]
-            label_name_idx = config['loss'][
-                'group_idx']['loss_group'][group_count][segment_idx]
-            output_name = config['labels_names'][label_name_idx]
-            outputs_dict[output_name] = output_segment
+        if group.startswith('CE'):
+            dim = 0
+            outputs_dict[config['labels_names'][dim]] = outputs[dim]
+        else:
+            dim = outputs_group.shape[-1]
+            for segment_idx in range(0, dim):
+                output_segment = outputs_group[:, segment_idx]
+                label_name_idx = config['loss'][
+                    'group_idx']['loss_group'][group_count][segment_idx]
+                output_name = config['labels_names'][label_name_idx]
+                outputs_dict[output_name] = output_segment
     return outputs_dict
 
 
 # this function is used to get the loss for each task
 def get_losses_class(config, outputs, data, criterion, device):
     losses = []
     loss_tot = torch.tensor([0]).float()
```

### Comparing `miacag-0.0.81/miacag/utils/script_utils.py` & `miacag-0.0.82/miacag/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.81/miacag/utils/sql_utils.py` & `miacag-0.0.82/miacag/utils/sql_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,16 @@
             host=sql_config['host'],
             database=sql_config['database'],
             user=sql_config['username'],
             password=sql_config['password'])
         data_type = data_types[count]
         sql = """
         ALTER TABLE "{schema_name}"."{table_name}"
-        ALTER COLUMN "{col_name}" TYPE {dtype};""".format(
+        ALTER COLUMN "{col_name}" TYPE {dtype}
+        USING "{col_name}"::{dtype};""".format(
             schema_name=sql_config['schema_name'],
             table_name=sql_config["table_name"],
             col_name=columnm_name,
             dtype=data_type
             )
         cursor = connection.cursor()
```

### Comparing `miacag-0.0.81/miacag.egg-info/PKG-INFO` & `miacag-0.0.82/miacag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miacag
-Version: 0.0.81
+Version: 0.0.82
 Summary: miacag angio DL tools
 Home-page: https://github.com/ChristianEschen/miacag
 Author: Christian Eschen
 Author-email: christian_eschen@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miacag-0.0.81/miacag.egg-info/SOURCES.txt` & `miacag-0.0.82/miacag.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -54,34 +54,43 @@
 miacag/model_utils/siam_loss.py
 miacag/model_utils/train_utils.py
 miacag/models/BuildModel.py
 miacag/models/__init__.py
 miacag/models/cnns.py
 miacag/models/get_encoder.py
 miacag/models/milmodel3d.py
+miacag/models/milmodel_from_features.py
 miacag/models/mlps.py
 miacag/models/modeling_finetune.py
 miacag/models/modeling_pretrain.py
 miacag/models/modules.py
 miacag/models/pretrained_vit.py
 miacag/models/backbone_encoders/__init__.py
 miacag/models/backbone_encoders/tabular/__init__.py
 miacag/models/backbone_encoders/tabular/base_encoders.py
+miacag/models/dino_utils/__init__.py
+miacag/models/dino_utils/dino_pretrained.py
+miacag/models/mae_st_util/__init__.py
+miacag/models/mae_st_util/logging.py
+miacag/models/mae_st_util/models_vit.py
+miacag/models/mae_st_util/video_vit.py
 miacag/models/torchhub/__init__.py
 miacag/models/torchhub/2D/__init__.py
 miacag/models/torchhub/2D+T/__init__.py
 miacag/models/torchhub/2D+T/mvit_base_16x4/__init__.py
 miacag/models/torchhub/2D+T/mvit_base_32x3/__init__.py
 miacag/models/torchhub/2D+T/r2plus1_18/__init__.py
 miacag/models/torchhub/2D+T/x3d_s/__init__.py
 miacag/models/torchhub/2D/r50/__init__.py
 miacag/plots/__init__.py
 miacag/plots/angle_plotter.py
 miacag/plots/getDataFromPdf.py
 miacag/plots/plot_histogram.py
+miacag/plots/plot_pathology_treatment_pred.py
+miacag/plots/plot_predict_coronary_pathology.py
 miacag/plots/plot_roc_auc_all.py
 miacag/plots/plot_scatter.py
 miacag/plots/plot_test.py
 miacag/plots/plotter.py
 miacag/plots/query_plot_agg_max.py
 miacag/postprocessing/__init__.py
 miacag/postprocessing/aggregate_pr_group.py
@@ -111,23 +120,23 @@
 miacag/scripts/compare_PCI_notPCI.py
 miacag/scripts/predict_patologi_eyeball_vs_estimated.py
 miacag/scripts/angiography_classifier/__init__.py
 miacag/scripts/angiography_classifier/predict_angio.py
 miacag/scripts/angiography_classifier/submit_angio.py
 miacag/scripts/angiography_classifier_stenosis_identifier/__init__.py
 miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py
+miacag/scripts/pretraining_downstreams/__init__.py
+miacag/scripts/pretraining_downstreams/submit_angio.py
 miacag/scripts/stenosis_identifier/__init__.py
 miacag/scripts/stenosis_identifier/submit_angio.py
 miacag/scripts/stenosis_identifier_mil/__init__.py
 miacag/scripts/stenosis_identifier_mil/submit_angio.py
 miacag/scripts/stenosis_regression/__init__.py
 miacag/scripts/stenosis_regression/submit_angio.py
 miacag/scripts/stenosis_regression_full/__init__.py
 miacag/scripts/stenosis_regression_full/submit_angio.py
-miacag/scripts/stenosis_regression_with_pretraining/__init__.py
-miacag/scripts/stenosis_regression_with_pretraining/submit_angio.py
 miacag/tests/__init__.py
 miacag/tests/test_sql_utils.py
 miacag/utils/__init__.py
 miacag/utils/common_utils.py
 miacag/utils/script_utils.py
 miacag/utils/sql_utils.py
```

### Comparing `miacag-0.0.81/setup.cfg` & `miacag-0.0.82/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = miacag
-version = 0.0.81
+version = 0.0.82
 author = Christian Eschen
 author_email = christian_eschen@hotmail.com
 description = miacag angio DL tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ChristianEschen/miacag
 classifiers =
```


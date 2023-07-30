# Comparing `tmp/monai-weekly-1.3.dev2330.tar.gz` & `tmp/monai-weekly-1.3.dev2331.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-weekly-1.3.dev2330.tar", last modified: Sun Jul 23 02:23:51 2023, max compression
+gzip compressed data, was "monai-weekly-1.3.dev2331.tar", last modified: Sun Jul 30 02:18:15 2023, max compression
```

## Comparing `monai-weekly-1.3.dev2330.tar` & `monai-weekly-1.3.dev2331.tar`

### file list

```diff
@@ -1,1147 +1,1152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.359347 monai-weekly-1.3.dev2330/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-23 02:23:51.359347 monai-weekly-1.3.dev2330/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.363347 monai-weekly-1.3.dev2330/monai/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-23 02:21:55.000000 monai-weekly-1.3.dev2330/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.887339 monai-weekly-1.3.dev2330/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.887339 monai-weekly-1.3.dev2330/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-23 02:23:51.363347 monai-weekly-1.3.dev2330/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.891339 monai-weekly-1.3.dev2330/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.895339 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27506 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.895339 monai-weekly-1.3.dev2330/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.895339 monai-weekly-1.3.dev2330/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.899340 monai-weekly-1.3.dev2330/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.899340 monai-weekly-1.3.dev2330/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.899340 monai-weekly-1.3.dev2330/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.903339 monai-weekly-1.3.dev2330/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    69282 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.907340 monai-weekly-1.3.dev2330/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.907340 monai-weekly-1.3.dev2330/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.907340 monai-weekly-1.3.dev2330/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48577 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.907340 monai-weekly-1.3.dev2330/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.911340 monai-weekly-1.3.dev2330/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.911340 monai-weekly-1.3.dev2330/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.911340 monai-weekly-1.3.dev2330/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.911340 monai-weekly-1.3.dev2330/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.911340 monai-weekly-1.3.dev2330/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.911340 monai-weekly-1.3.dev2330/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.915340 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.915340 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.915340 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.919340 monai-weekly-1.3.dev2330/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.919340 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.919340 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.919340 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.923340 monai-weekly-1.3.dev2330/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.923340 monai-weekly-1.3.dev2330/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.923340 monai-weekly-1.3.dev2330/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.927340 monai-weekly-1.3.dev2330/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.931340 monai-weekly-1.3.dev2330/monai/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.943340 monai-weekly-1.3.dev2330/monai/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    68912 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    27511 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65554 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49494 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.943340 monai-weekly-1.3.dev2330/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.943340 monai-weekly-1.3.dev2330/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.947340 monai-weekly-1.3.dev2330/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.947340 monai-weekly-1.3.dev2330/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.963341 monai-weekly-1.3.dev2330/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22501 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.963341 monai-weekly-1.3.dev2330/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.971341 monai-weekly-1.3.dev2330/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.979341 monai-weekly-1.3.dev2330/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    42239 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.979341 monai-weekly-1.3.dev2330/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.991341 monai-weekly-1.3.dev2330/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:50.995341 monai-weekly-1.3.dev2330/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.015341 monai-weekly-1.3.dev2330/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/daf3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40667 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/quicknat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.015341 monai-weekly-1.3.dev2330/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.023342 monai-weekly-1.3.dev2330/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.027341 monai-weekly-1.3.dev2330/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75075 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    61070 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.027341 monai-weekly-1.3.dev2330/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107785 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.031342 monai-weekly-1.3.dev2330/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25374 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.031342 monai-weekly-1.3.dev2330/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/lazy/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/lazy/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.031342 monai-weekly-1.3.dev2330/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.035342 monai-weekly-1.3.dev2330/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40802 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.035342 monai-weekly-1.3.dev2330/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/signal/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.035342 monai-weekly-1.3.dev2330/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.039342 monai-weekly-1.3.dev2330/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179599 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (123)   127418 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.043342 monai-weekly-1.3.dev2330/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70963 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76167 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    81426 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.047342 monai-weekly-1.3.dev2330/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29761 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.051342 monai-weekly-1.3.dev2330/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.055342 monai-weekly-1.3.dev2330/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-23 02:23:50.000000 monai-weekly-1.3.dev2330/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34350 2023-07-23 02:23:50.000000 monai-weekly-1.3.dev2330/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 02:23:50.000000 monai-weekly-1.3.dev2330/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 02:23:50.000000 monai-weekly-1.3.dev2330/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-23 02:23:50.000000 monai-weekly-1.3.dev2330/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-23 02:23:50.000000 monai-weekly-1.3.dev2330/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-23 02:23:51.363347 monai-weekly-1.3.dev2330/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 02:23:51.359347 monai-weekly-1.3.dev2330/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_add_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_as_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_as_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_auto3dseg_bundlegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25175 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_daf3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_download_url_yandex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23538 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_parallel_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_parallel_execution_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_quicknat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_scale_intensity_fixed_meand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_split_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_split_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_version_leq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_wsi_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_zarr_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-07-23 02:21:52.000000 monai-weekly-1.3.dev2330/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.670950 monai-weekly-1.3.dev2331/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-07-30 02:18:15.670950 monai-weekly-1.3.dev2331/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.674950 monai-weekly-1.3.dev2331/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-30 02:16:21.000000 monai-weekly-1.3.dev2331/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.326950 monai-weekly-1.3.dev2331/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.326950 monai-weekly-1.3.dev2331/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-30 02:18:15.674950 monai-weekly-1.3.dev2331/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.326950 monai-weekly-1.3.dev2331/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.330950 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.334950 monai-weekly-1.3.dev2331/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.334950 monai-weekly-1.3.dev2331/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41979 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.334950 monai-weekly-1.3.dev2331/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.334950 monai-weekly-1.3.dev2331/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.338950 monai-weekly-1.3.dev2331/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.338950 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69282 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.342950 monai-weekly-1.3.dev2331/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.342950 monai-weekly-1.3.dev2331/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.346950 monai-weekly-1.3.dev2331/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48577 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.346950 monai-weekly-1.3.dev2331/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.346950 monai-weekly-1.3.dev2331/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.346950 monai-weekly-1.3.dev2331/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.354950 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.354950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.354950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.354950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.358950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.358950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.358950 monai-weekly-1.3.dev2331/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.358950 monai-weekly-1.3.dev2331/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.362950 monai-weekly-1.3.dev2331/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.366950 monai-weekly-1.3.dev2331/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.374950 monai-weekly-1.3.dev2331/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78913 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/ultrasound_confidence_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65554 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49494 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.378950 monai-weekly-1.3.dev2331/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.378950 monai-weekly-1.3.dev2331/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.378950 monai-weekly-1.3.dev2331/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.382950 monai-weekly-1.3.dev2331/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.394950 monai-weekly-1.3.dev2331/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22501 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.394950 monai-weekly-1.3.dev2331/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.398950 monai-weekly-1.3.dev2331/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/cldice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46558 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.406950 monai-weekly-1.3.dev2331/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42239 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.406950 monai-weekly-1.3.dev2331/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.418950 monai-weekly-1.3.dev2331/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.422950 monai-weekly-1.3.dev2331/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.434950 monai-weekly-1.3.dev2331/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40667 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.434950 monai-weekly-1.3.dev2331/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.442950 monai-weekly-1.3.dev2331/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.442950 monai-weekly-1.3.dev2331/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75075 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61070 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.446950 monai-weekly-1.3.dev2331/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112239 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82785 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.446950 monai-weekly-1.3.dev2331/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25374 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.446950 monai-weekly-1.3.dev2331/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.450950 monai-weekly-1.3.dev2331/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.450950 monai-weekly-1.3.dev2331/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40802 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.450950 monai-weekly-1.3.dev2331/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/signal/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.450950 monai-weekly-1.3.dev2331/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.454950 monai-weekly-1.3.dev2331/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179715 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.454950 monai-weekly-1.3.dev2331/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70963 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76167 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81426 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.458950 monai-weekly-1.3.dev2331/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.462950 monai-weekly-1.3.dev2331/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.462950 monai-weekly-1.3.dev2331/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34514 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-30 02:18:15.670950 monai-weekly-1.3.dev2331/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.670950 monai-weekly-1.3.dev2331/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cldice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25175 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_download_url_yandex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gdsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_parallel_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_parallel_execution_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity_fixed_meand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_split_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_split_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23814 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ultrasound_confidence_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_version_leq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_wsi_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zarr_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/versioneer.py
```

### Comparing `monai-weekly-1.3.dev2330/LICENSE` & `monai-weekly-1.3.dev2331/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/PKG-INFO` & `monai-weekly-1.3.dev2331/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.3.dev2330
+Version: 1.3.dev2331
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -28,14 +28,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: all
 Provides-Extra: nibabel
 Provides-Extra: ninja
 Provides-Extra: skimage
+Provides-Extra: scipy
 Provides-Extra: pillow
 Provides-Extra: tensorboard
 Provides-Extra: gdown
 Provides-Extra: ignite
 Provides-Extra: torchvision
 Provides-Extra: itk
 Provides-Extra: tqdm
```

### Comparing `monai-weekly-1.3.dev2330/README.md` & `monai-weekly-1.3.dev2331/README.md`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/__init__.py` & `monai-weekly-1.3.dev2331/monai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,8 +74,8 @@
     "metrics",
     "networks",
     "optimizers",
     "transforms",
     "utils",
     "visualize",
 ]
-__commit_id__ = "644c9e5d58082f442e3e8230fcf6ae1d6e8ee5b8"
+__commit_id__ = "5feb353030e0bb204e21e1de338cd81b5972bb8a"
```

### Comparing `monai-weekly-1.3.dev2330/monai/_extensions/__init__.py` & `monai-weekly-1.3.dev2331/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm.cpp` & `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm.h` & `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm_cpu.cpp` & `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm_cuda.cu` & `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/_extensions/loader.py` & `monai-weekly-1.3.dev2331/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/__main__.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/auto_runner.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/auto_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/bundle_gen.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/bundle_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/data_analyzer.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/ensemble_builder.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/hpo_gen.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/hpo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/transforms.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/auto3dseg/utils.py` & `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/datasets.py` & `monai-weekly-1.3.dev2331/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/deepedit/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/deepedit/interaction.py` & `monai-weekly-1.3.dev2331/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/deepedit/transforms.py` & `monai-weekly-1.3.dev2331/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/deepgrow/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/deepgrow/dataset.py` & `monai-weekly-1.3.dev2331/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/deepgrow/interaction.py` & `monai-weekly-1.3.dev2331/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/deepgrow/transforms.py` & `monai-weekly-1.3.dev2331/monai/apps/deepgrow/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,16 +437,16 @@
         )
 
         center = list(np.mean([box_start, box_end], axis=0).astype(int, copy=False))
         current_size = list(np.subtract(box_end, box_start).astype(int, copy=False))
 
         if np.all(np.less(current_size, self.spatial_size)):
             cropper = SpatialCrop(roi_center=center, roi_size=self.spatial_size)
-            box_start = np.array([s.start for s in cropper.slices])  # type: ignore
-            box_end = np.array([s.stop for s in cropper.slices])  # type: ignore
+            box_start = np.array([s.start for s in cropper.slices])
+            box_end = np.array([s.stop for s in cropper.slices])
         else:
             cropper = SpatialCrop(roi_start=box_start, roi_end=box_end)
 
         for key, meta_key, meta_key_postfix in self.key_iterator(d, self.meta_keys, self.meta_key_postfix):
             meta_key = meta_key or f"{key}_{meta_key_postfix}"
             d[meta_key][self.start_coord_key] = box_start
             d[meta_key][self.end_coord_key] = box_end
```

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/metrics/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/metrics/coco.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/metrics/matching.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/networks/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/networks/retinanet_detector.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/networks/retinanet_network.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/transforms/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/transforms/array.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/transforms/box_ops.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/transforms/dictionary.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/utils/ATSS_matcher.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/utils/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/utils/anchor_utils.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/utils/box_coder.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/utils/box_selector.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/utils/detector_utils.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/utils/hard_negative_sampler.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/detection/utils/predict_utils.py` & `monai-weekly-1.3.dev2331/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/mmars/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/mmars/mmars.py` & `monai-weekly-1.3.dev2331/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/mmars/model_desc.py` & `monai-weekly-1.3.dev2331/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/nnunet/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/nnunet/__main__.py` & `monai-weekly-1.3.dev2331/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/nnunet/nnunetv2_runner.py` & `monai-weekly-1.3.dev2331/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/nnunet/utils.py` & `monai-weekly-1.3.dev2331/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/nuclick/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/nuclick/transforms.py` & `monai-weekly-1.3.dev2331/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/engines/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/engines/utils.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/handlers/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/handlers/utils.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/inferers/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/inferers/inferer.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/losses/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/losses/hovernet_loss.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/metrics/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/metrics/lesion_froc.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/post/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/post/array.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/post/dictionary.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/stain/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/stain/array.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/transforms/stain/dictionary.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/pathology/utils.py` & `monai-weekly-1.3.dev2331/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/complex_utils.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/fastmri_reader.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/mri_utils.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/utils.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/networks/nets/varnet.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/transforms/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/transforms/array.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/reconstruction/transforms/dictionary.py` & `monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/tcia/__init__.py` & `monai-weekly-1.3.dev2331/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/tcia/label_desc.py` & `monai-weekly-1.3.dev2331/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/tcia/utils.py` & `monai-weekly-1.3.dev2331/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/apps/utils.py` & `monai-weekly-1.3.dev2331/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/auto3dseg/__init__.py` & `monai-weekly-1.3.dev2331/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/auto3dseg/algo_gen.py` & `monai-weekly-1.3.dev2331/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/auto3dseg/analyzer.py` & `monai-weekly-1.3.dev2331/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/auto3dseg/operations.py` & `monai-weekly-1.3.dev2331/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/auto3dseg/seg_summarizer.py` & `monai-weekly-1.3.dev2331/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/auto3dseg/utils.py` & `monai-weekly-1.3.dev2331/monai/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/__init__.py` & `monai-weekly-1.3.dev2331/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/__main__.py` & `monai-weekly-1.3.dev2331/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/config_item.py` & `monai-weekly-1.3.dev2331/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/config_parser.py` & `monai-weekly-1.3.dev2331/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/properties.py` & `monai-weekly-1.3.dev2331/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/reference_resolver.py` & `monai-weekly-1.3.dev2331/monai/bundle/reference_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,16 @@
         """
         if id in self.resolved_content:
             return self.resolved_content[id]
         try:
             item = look_up_option(id, self.items, print_all_options=False, default=kwargs.get("default", "no_default"))
         except ValueError as err:
             raise KeyError(f"id='{id}' is not found in the config resolver.") from err
+        if not isinstance(item, ConfigItem):
+            return item
         item_config = item.get_config()
 
         if waiting_list is None:
             waiting_list = set()
         waiting_list.add(id)
 
         for t, v in self.items.items():
@@ -147,19 +149,18 @@
             # check whether the component has any unresolved references
             if d not in self.resolved_content:
                 # this referring item is not resolved
                 try:
                     look_up_option(d, self.items, print_all_options=False)
                 except ValueError as err:
                     msg = f"the referring item `@{d}` is not defined in the config content."
-                    if self.allow_missing_reference:
-                        warnings.warn(msg)
-                        continue
-                    else:
+                    if not self.allow_missing_reference:
                         raise ValueError(msg) from err
+                    warnings.warn(msg)
+                    continue
                 # recursively resolve the reference first
                 self._resolve_one_item(id=d, waiting_list=waiting_list, **kwargs)
                 waiting_list.discard(d)
 
         # all references are resolved, then try to resolve current config item
         new_config = self.update_config_with_refs(config=item_config, id=id, refs=self.resolved_content)
         item.update_config(config=new_config)
```

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/scripts.py` & `monai-weekly-1.3.dev2331/monai/bundle/scripts.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/utils.py` & `monai-weekly-1.3.dev2331/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/bundle/workflows.py` & `monai-weekly-1.3.dev2331/monai/bundle/workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/config/__init__.py` & `monai-weekly-1.3.dev2331/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/config/deviceconfig.py` & `monai-weekly-1.3.dev2331/monai/config/deviceconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     """
     output = OrderedDict()
 
     output["Pytorch Ignite"] = get_package_version("ignite")
     output["ITK"] = get_package_version("itk")
     output["Nibabel"] = get_package_version("nibabel")
     output["scikit-image"] = get_package_version("skimage")
+    output["scipy"] = get_package_version("scipy")
     output["Pillow"] = get_package_version("PIL")
     output["Tensorboard"] = get_package_version("tensorboard")
     output["gdown"] = get_package_version("gdown")
     output["TorchVision"] = get_package_version("torchvision")
     output["tqdm"] = get_package_version("tqdm")
     output["lmdb"] = get_package_version("lmdb")
     output["psutil"] = psutil_version
```

### Comparing `monai-weekly-1.3.dev2330/monai/config/type_definitions.py` & `monai-weekly-1.3.dev2331/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/__init__.py` & `monai-weekly-1.3.dev2331/monai/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .dataset import (
     ArrayDataset,
     CacheDataset,
     CacheNTransDataset,
     CSVDataset,
     Dataset,
     DatasetFunc,
+    GDSDataset,
     LMDBDataset,
     NPZDictItemDataset,
     PersistentDataset,
     SmartCacheDataset,
     ZipDataset,
 )
 from .dataset_summary import DatasetSummary
@@ -146,7 +147,9 @@
             meta_tensor.stride(),
             meta_tensor.requires_grad,
             meta_tensor.__dict__,
         )
         return _rebuild_meta, (type(meta_tensor), storage, dtype, metadata)
 
     ForkingPickler.register(MetaTensor, reduce_meta_tensor)
+
+from .ultrasound_confidence_map import UltrasoundConfidenceMap
```

### Comparing `monai-weekly-1.3.dev2330/monai/data/box_utils.py` & `monai-weekly-1.3.dev2331/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/csv_saver.py` & `monai-weekly-1.3.dev2331/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/dataloader.py` & `monai-weekly-1.3.dev2331/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/dataset.py` & `monai-weekly-1.3.dev2331/monai/data/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,36 +30,39 @@
 import numpy as np
 import torch
 from torch.multiprocessing import Manager
 from torch.serialization import DEFAULT_PROTOCOL
 from torch.utils.data import Dataset as _TorchDataset
 from torch.utils.data import Subset
 
+from monai.data.meta_tensor import MetaTensor
 from monai.data.utils import SUPPORTED_PICKLE_MOD, convert_tables_to_dicts, pickle_hashing
 from monai.transforms import (
     Compose,
     Randomizable,
     RandomizableTrait,
     Transform,
     apply_transform,
     convert_to_contiguous,
     reset_ops_id,
 )
-from monai.utils import MAX_SEED, get_seed, look_up_option, min_version, optional_import
+from monai.utils import MAX_SEED, convert_to_tensor, get_seed, look_up_option, min_version, optional_import
 from monai.utils.misc import first
 
 if TYPE_CHECKING:
     from tqdm import tqdm
 
     has_tqdm = True
 else:
     tqdm, has_tqdm = optional_import("tqdm", "4.47.0", min_version, "tqdm")
 
+cp, _ = optional_import("cupy")
 lmdb, _ = optional_import("lmdb")
 pd, _ = optional_import("pandas")
+kvikio_numpy, _ = optional_import("kvikio.numpy")
 
 
 class Dataset(_TorchDataset):
     """
     A generic dataset with a length property and an optional callable data transform
     when fetching a data sample.
     If passing slicing indices, will return a PyTorch Subset, for example: `data: Subset = dataset[1:4]`,
@@ -322,15 +325,14 @@
         """
         if not isinstance(self.transform, Compose):
             raise ValueError("transform must be an instance of monai.transforms.Compose.")
 
         first_random = self.transform.get_index_of_first(
             lambda t: isinstance(t, RandomizableTrait) or not isinstance(t, Transform)
         )
-
         item_transformed = self.transform(item_transformed, end=first_random, threading=True)
 
         if self.reset_ops_id:
             reset_ops_id(item_transformed)
         return item_transformed
 
     def _post_transform(self, item_transformed):
@@ -1506,7 +1508,184 @@
             else:
                 raise ValueError("`src` must be file path or pandas `DataFrame`.")
 
         data = convert_tables_to_dicts(
             dfs=dfs, row_indices=row_indices, col_names=col_names, col_types=col_types, col_groups=col_groups, **kwargs
         )
         super().__init__(data=data, transform=transform)
+
+
+class GDSDataset(PersistentDataset):
+    """
+    An extension of the PersistentDataset using direct memory access(DMA) data path between
+    GPU memory and storage, thus avoiding a bounce buffer through the CPU. This direct path can increase system
+    bandwidth while decreasing latency and utilization load on the CPU and GPU.
+
+    A tutorial is available: https://github.com/Project-MONAI/tutorials/blob/main/modules/GDS_dataset.ipynb.
+
+    See also: https://github.com/rapidsai/kvikio
+    """
+
+    def __init__(
+        self,
+        data: Sequence,
+        transform: Sequence[Callable] | Callable,
+        cache_dir: Path | str | None,
+        device: int,
+        hash_func: Callable[..., bytes] = pickle_hashing,
+        hash_transform: Callable[..., bytes] | None = None,
+        reset_ops_id: bool = True,
+        **kwargs: Any,
+    ) -> None:
+        """
+        Args:
+            data: input data file paths to load and transform to generate dataset for model.
+                `GDSDataset` expects input data to be a list of serializable
+                and hashes them as cache keys using `hash_func`.
+            transform: transforms to execute operations on input data.
+            cache_dir: If specified, this is the location for gpu direct storage
+                of pre-computed transformed data tensors. The cache_dir is computed once, and
+                persists on disk until explicitly removed.  Different runs, programs, experiments
+                may share a common cache dir provided that the transforms pre-processing is consistent.
+                If `cache_dir` doesn't exist, will automatically create it.
+                If `cache_dir` is `None`, there is effectively no caching.
+            device: target device to put the output Tensor data. Note that only int can be used to
+                specify the gpu to be used.
+            hash_func: a callable to compute hash from data items to be cached.
+                defaults to `monai.data.utils.pickle_hashing`.
+            hash_transform: a callable to compute hash from the transform information when caching.
+                This may reduce errors due to transforms changing during experiments. Default to None (no hash).
+                Other options are `pickle_hashing` and `json_hashing` functions from `monai.data.utils`.
+            reset_ops_id: whether to set `TraceKeys.ID` to ``Tracekys.NONE``, defaults to ``True``.
+                When this is enabled, the traced transform instance IDs will be removed from the cached MetaTensors.
+                This is useful for skipping the transform instance checks when inverting applied operations
+                using the cached content and with re-created transform instances.
+
+        """
+        super().__init__(
+            data=data,
+            transform=transform,
+            cache_dir=cache_dir,
+            hash_func=hash_func,
+            hash_transform=hash_transform,
+            reset_ops_id=reset_ops_id,
+            **kwargs,
+        )
+        self.device = device
+        self._meta_cache: dict[Any, dict[Any, Any]] = {}
+
+    def _cachecheck(self, item_transformed):
+        """
+        In order to enable direct storage to the GPU when loading the hashfile, rewritten this function.
+        Note that in this function, it will always return `torch.Tensor` when load data from cache.
+
+        Args:
+            item_transformed: The current data element to be mutated into transformed representation
+
+        Returns:
+            The transformed data_element, either from cache, or explicitly computing it.
+
+        Warning:
+            The current implementation does not encode transform information as part of the
+            hashing mechanism used for generating cache names when `hash_transform` is None.
+            If the transforms applied are changed in any way, the objects in the cache dir will be invalid.
+
+        """
+        hashfile = None
+        # compute a cache id
+        if self.cache_dir is not None:
+            data_item_md5 = self.hash_func(item_transformed).decode("utf-8")
+            data_item_md5 += self.transform_hash
+            hashfile = self.cache_dir / f"{data_item_md5}.pt"
+
+        if hashfile is not None and hashfile.is_file():  # cache hit
+            with cp.cuda.Device(self.device):
+                if isinstance(item_transformed, dict):
+                    item: dict[Any, Any] = {}  # type:ignore
+                    for k in item_transformed:
+                        meta_k = self._load_meta_cache(meta_hash_file_name=f"{hashfile.name}-{k}-meta")
+                        item[k] = kvikio_numpy.fromfile(f"{hashfile}-{k}", dtype=meta_k["dtype"], like=cp.empty(()))
+                        item[k] = convert_to_tensor(item[k].reshape(meta_k["shape"]), device=f"cuda:{self.device}")
+                        item[f"{k}_meta_dict"] = meta_k
+                    return item
+                elif isinstance(item_transformed, (np.ndarray, torch.Tensor)):
+                    _meta = self._load_meta_cache(meta_hash_file_name=f"{hashfile.name}-meta")
+                    _data = kvikio_numpy.fromfile(f"{hashfile}", dtype=_meta["dtype"], like=cp.empty(()))
+                    _data = convert_to_tensor(_data.reshape(_meta["shape"]), device=f"cuda:{self.device}")
+                    filtered_keys = list(filter(lambda key: key not in ["dtype", "shape"], _meta.keys()))
+                    if bool(filtered_keys):
+                        return (_data, _meta)
+                    return _data
+                else:
+                    item: list[dict[Any, Any]] = [{} for _ in range(len(item_transformed))]  # type:ignore
+                    for i, _item in enumerate(item_transformed):
+                        for k in _item:
+                            meta_i_k = self._load_meta_cache(meta_hash_file_name=f"{hashfile.name}-{k}-meta-{i}")
+                            item_k = kvikio_numpy.fromfile(
+                                f"{hashfile}-{k}-{i}", dtype=meta_i_k["dtype"], like=cp.empty(())
+                            )
+                            item_k = convert_to_tensor(item[i].reshape(meta_i_k["shape"]), device=f"cuda:{self.device}")
+                            item[i].update({k: item_k, f"{k}_meta_dict": meta_i_k})
+                    return item
+
+        # create new cache
+        _item_transformed = self._pre_transform(deepcopy(item_transformed))  # keep the original hashed
+        if hashfile is None:
+            return _item_transformed
+        if isinstance(_item_transformed, dict):
+            for k in _item_transformed:
+                data_hashfile = f"{hashfile}-{k}"
+                meta_hash_file_name = f"{hashfile.name}-{k}-meta"
+                if isinstance(_item_transformed[k], (np.ndarray, torch.Tensor)):
+                    self._create_new_cache(_item_transformed[k], data_hashfile, meta_hash_file_name)
+                else:
+                    return _item_transformed
+        elif isinstance(_item_transformed, (np.ndarray, torch.Tensor)):
+            data_hashfile = f"{hashfile}"
+            meta_hash_file_name = f"{hashfile.name}-meta"
+            self._create_new_cache(_item_transformed, data_hashfile, meta_hash_file_name)
+        else:
+            for i, _item in enumerate(_item_transformed):
+                for k in _item:
+                    data_hashfile = f"{hashfile}-{k}-{i}"
+                    meta_hash_file_name = f"{hashfile.name}-{k}-meta-{i}"
+                    self._create_new_cache(_item, data_hashfile, meta_hash_file_name)
+        open(hashfile, "a").close()  # store cacheid
+        return _item_transformed
+
+    def _create_new_cache(self, data, data_hashfile, meta_hash_file_name):
+        self._meta_cache[meta_hash_file_name] = copy(data.meta) if isinstance(data, MetaTensor) else {}
+        _item_transformed_data = data.array if isinstance(data, MetaTensor) else data
+        if isinstance(_item_transformed_data, torch.Tensor):
+            _item_transformed_data = _item_transformed_data.numpy()
+        self._meta_cache[meta_hash_file_name]["shape"] = _item_transformed_data.shape
+        self._meta_cache[meta_hash_file_name]["dtype"] = str(_item_transformed_data.dtype)
+        kvikio_numpy.tofile(_item_transformed_data, data_hashfile)
+        try:
+            # NOTE: Writing to a temporary directory and then using a nearly atomic rename operation
+            #       to make the cache more robust to manual killing of parent process
+            #       which may leave partially written cache files in an incomplete state
+            with tempfile.TemporaryDirectory() as tmpdirname:
+                meta_hash_file = self.cache_dir / meta_hash_file_name
+                temp_hash_file = Path(tmpdirname) / meta_hash_file_name
+                torch.save(
+                    obj=self._meta_cache[meta_hash_file_name],
+                    f=temp_hash_file,
+                    pickle_module=look_up_option(self.pickle_module, SUPPORTED_PICKLE_MOD),
+                    pickle_protocol=self.pickle_protocol,
+                )
+                if temp_hash_file.is_file() and not meta_hash_file.is_file():
+                    # On Unix, if target exists and is a file, it will be replaced silently if the
+                    # user has permission.
+                    # for more details: https://docs.python.org/3/library/shutil.html#shutil.move.
+                    try:
+                        shutil.move(str(temp_hash_file), meta_hash_file)
+                    except FileExistsError:
+                        pass
+        except PermissionError:  # project-monai/monai issue #3613
+            pass
+
+    def _load_meta_cache(self, meta_hash_file_name):
+        if meta_hash_file_name in self._meta_cache:
+            return self._meta_cache[meta_hash_file_name]
+        else:
+            return torch.load(self.cache_dir / meta_hash_file_name)  # type:ignore
```

### Comparing `monai-weekly-1.3.dev2330/monai/data/dataset_summary.py` & `monai-weekly-1.3.dev2331/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/decathlon_datalist.py` & `monai-weekly-1.3.dev2331/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/fft_utils.py` & `monai-weekly-1.3.dev2331/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/folder_layout.py` & `monai-weekly-1.3.dev2331/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/grid_dataset.py` & `monai-weekly-1.3.dev2331/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/image_dataset.py` & `monai-weekly-1.3.dev2331/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/image_reader.py` & `monai-weekly-1.3.dev2331/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/image_writer.py` & `monai-weekly-1.3.dev2331/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/iterable_dataset.py` & `monai-weekly-1.3.dev2331/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/itk_torch_bridge.py` & `monai-weekly-1.3.dev2331/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/meta_obj.py` & `monai-weekly-1.3.dev2331/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/meta_tensor.py` & `monai-weekly-1.3.dev2331/monai/data/meta_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             the input type was not `MetaTensor`, then no modifications will have been
             made. If global parameters have been set to false (e.g.,
             `not get_track_meta()`), then any `MetaTensor` will be converted to
             `torch.Tensor`. Else, metadata will be propagated as necessary (see
             :py:func:`MetaTensor._copy_meta`).
         """
         out = []
-        metas = None
+        metas = None  # optional output metadicts for each of the return value in `rets`
         is_batch = any(x.is_batch for x in MetaObj.flatten_meta_objs(args, kwargs.values()) if hasattr(x, "is_batch"))
         for idx, ret in enumerate(rets):
             # if not `MetaTensor`, nothing to do.
             if not isinstance(ret, MetaTensor):
                 pass
             # if not tracking, convert to `torch.Tensor`.
             elif not get_track_meta():
@@ -215,64 +215,70 @@
             else:
                 meta_args = MetaObj.flatten_meta_objs(args, kwargs.values())
                 ret.is_batch = is_batch
                 ret.copy_meta_from(meta_args, copy_attr=not is_batch)
                 # the following is not implemented but the network arch may run into this case:
                 # if func == torch.cat and any(m.is_batch if hasattr(m, "is_batch") else False for m in meta_args):
                 #     raise NotImplementedError("torch.cat is not implemented for batch of MetaTensors.")
-
-                # If we have a batch of data, then we need to be careful if a slice of
-                # the data is returned. Depending on how the data are indexed, we return
-                # some or all of the metadata, and the return object may or may not be a
-                # batch of data (e.g., `batch[:,-1]` versus `batch[0]`).
                 if is_batch:
-                    # if indexing e.g., `batch[0]`
-                    if func == torch.Tensor.__getitem__:
-                        batch_idx = args[1]
-                        if isinstance(batch_idx, Sequence):
-                            batch_idx = batch_idx[0]
-                        # if using e.g., `batch[:, -1]` or `batch[..., -1]`, then the
-                        # first element will be `slice(None, None, None)` and `Ellipsis`,
-                        # respectively. Don't need to do anything with the metadata.
-                        if batch_idx not in (slice(None, None, None), Ellipsis, None) and idx == 0:
-                            ret_meta = decollate_batch(args[0], detach=False)[batch_idx]
-                            if isinstance(ret_meta, list) and ret_meta:  # e.g. batch[0:2], re-collate
-                                try:
-                                    ret_meta = list_data_collate(ret_meta)
-                                except (TypeError, ValueError, RuntimeError, IndexError) as e:
-                                    raise ValueError(
-                                        "Inconsistent batched metadata dicts when slicing a batch of MetaTensors, "
-                                        "please convert it into a torch Tensor using `x.as_tensor()` or "
-                                        "a numpy array using `x.array`."
-                                    ) from e
-                            elif isinstance(ret_meta, MetaObj):  # e.g. `batch[0]` or `batch[0, 1]`, batch_idx is int
-                                ret_meta.is_batch = False
-                            if hasattr(ret_meta, "__dict__"):
-                                ret.__dict__ = ret_meta.__dict__.copy()
-                    # `unbind` is used for `next(iter(batch))`. Also for `decollate_batch`.
-                    # But we only want to split the batch if the `unbind` is along the 0th
-                    # dimension.
-                    elif func == torch.Tensor.unbind:
-                        if len(args) > 1:
-                            dim = args[1]
-                        elif "dim" in kwargs:
-                            dim = kwargs["dim"]
-                        else:
-                            dim = 0
-                        if dim == 0:
-                            if metas is None:
-                                metas = decollate_batch(args[0], detach=False)
-                            ret.__dict__ = metas[idx].__dict__.copy()
-                            ret.is_batch = False
-
+                    ret = MetaTensor._handle_batched(ret, idx, metas, func, args, kwargs)
             out.append(ret)
         # if the input was a tuple, then return it as a tuple
         return tuple(out) if isinstance(rets, tuple) else out
 
     @classmethod
+    def _handle_batched(cls, ret, idx, metas, func, args, kwargs):
+        """utility function to handle batched MetaTensors."""
+        # If we have a batch of data, then we need to be careful if a slice of
+        # the data is returned. Depending on how the data are indexed, we return
+        # some or all of the metadata, and the return object may or may not be a
+        # batch of data (e.g., `batch[:,-1]` versus `batch[0]`).
+        # if indexing e.g., `batch[0]`
+        if func == torch.Tensor.__getitem__:
+            if idx > 0 or len(args) < 2 or len(args[0]) < 1:
+                return ret
+            batch_idx = args[1][0] if isinstance(args[1], Sequence) else args[1]
+            # if using e.g., `batch[:, -1]` or `batch[..., -1]`, then the
+            # first element will be `slice(None, None, None)` and `Ellipsis`,
+            # respectively. Don't need to do anything with the metadata.
+            if batch_idx in (slice(None, None, None), Ellipsis, None) or isinstance(batch_idx, torch.Tensor):
+                return ret
+            dec_batch = decollate_batch(args[0], detach=False)
+            ret_meta = dec_batch[batch_idx]
+            if isinstance(ret_meta, list) and ret_meta:  # e.g. batch[0:2], re-collate
+                try:
+                    ret_meta = list_data_collate(ret_meta)
+                except (TypeError, ValueError, RuntimeError, IndexError) as e:
+                    raise ValueError(
+                        "Inconsistent batched metadata dicts when slicing a batch of MetaTensors, "
+                        "please consider converting it into a torch Tensor using `x.as_tensor()` or "
+                        "a numpy array using `x.array`."
+                    ) from e
+            elif isinstance(ret_meta, MetaObj):  # e.g. `batch[0]` or `batch[0, 1]`, batch_idx is int
+                ret_meta.is_batch = False
+            if hasattr(ret_meta, "__dict__"):
+                ret.__dict__ = ret_meta.__dict__.copy()
+        # `unbind` is used for `next(iter(batch))`. Also for `decollate_batch`.
+        # But we only want to split the batch if the `unbind` is along the 0th dimension.
+        elif func == torch.Tensor.unbind:
+            if len(args) > 1:
+                dim = args[1]
+            elif "dim" in kwargs:
+                dim = kwargs["dim"]
+            else:
+                dim = 0
+            if dim == 0:
+                if metas is None:
+                    metas = decollate_batch(args[0], detach=False)
+                if hasattr(metas[idx], "__dict__"):
+                    ret.__dict__ = metas[idx].__dict__.copy()
+                ret.is_batch = False
+        return ret
+
+    @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None) -> Any:
         """Wraps all torch functions."""
         if kwargs is None:
             kwargs = {}
         ret = super().__torch_function__(func, types, args, kwargs)
         # if `out` has been used as argument, metadata is not copied, nothing to do.
         # if "out" in kwargs:
```

### Comparing `monai-weekly-1.3.dev2330/monai/data/samplers.py` & `monai-weekly-1.3.dev2331/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/synthetic.py` & `monai-weekly-1.3.dev2331/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/test_time_augmentation.py` & `monai-weekly-1.3.dev2331/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/thread_buffer.py` & `monai-weekly-1.3.dev2331/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/torchscript_utils.py` & `monai-weekly-1.3.dev2331/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/utils.py` & `monai-weekly-1.3.dev2331/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/video_dataset.py` & `monai-weekly-1.3.dev2331/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/wsi_datasets.py` & `monai-weekly-1.3.dev2331/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/data/wsi_reader.py` & `monai-weekly-1.3.dev2331/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/engines/__init__.py` & `monai-weekly-1.3.dev2331/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/engines/evaluator.py` & `monai-weekly-1.3.dev2331/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/engines/multi_gpu_supervised_trainer.py` & `monai-weekly-1.3.dev2331/monai/engines/multi_gpu_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/engines/trainer.py` & `monai-weekly-1.3.dev2331/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/engines/utils.py` & `monai-weekly-1.3.dev2331/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/engines/workflow.py` & `monai-weekly-1.3.dev2331/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/fl/__init__.py` & `monai-weekly-1.3.dev2331/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/fl/client/__init__.py` & `monai-weekly-1.3.dev2331/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/fl/client/client_algo.py` & `monai-weekly-1.3.dev2331/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/fl/client/monai_algo.py` & `monai-weekly-1.3.dev2331/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/fl/utils/__init__.py` & `monai-weekly-1.3.dev2331/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/fl/utils/constants.py` & `monai-weekly-1.3.dev2331/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/fl/utils/exchange_object.py` & `monai-weekly-1.3.dev2331/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/fl/utils/filters.py` & `monai-weekly-1.3.dev2331/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/__init__.py` & `monai-weekly-1.3.dev2331/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/checkpoint_loader.py` & `monai-weekly-1.3.dev2331/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/checkpoint_saver.py` & `monai-weekly-1.3.dev2331/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/classification_saver.py` & `monai-weekly-1.3.dev2331/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/clearml_handlers.py` & `monai-weekly-1.3.dev2331/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/confusion_matrix.py` & `monai-weekly-1.3.dev2331/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/decollate_batch.py` & `monai-weekly-1.3.dev2331/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/earlystop_handler.py` & `monai-weekly-1.3.dev2331/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/garbage_collector.py` & `monai-weekly-1.3.dev2331/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/hausdorff_distance.py` & `monai-weekly-1.3.dev2331/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/ignite_metric.py` & `monai-weekly-1.3.dev2331/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/logfile_handler.py` & `monai-weekly-1.3.dev2331/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/lr_schedule_handler.py` & `monai-weekly-1.3.dev2331/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/mean_dice.py` & `monai-weekly-1.3.dev2331/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/mean_iou.py` & `monai-weekly-1.3.dev2331/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/metric_logger.py` & `monai-weekly-1.3.dev2331/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/metrics_reloaded_handler.py` & `monai-weekly-1.3.dev2331/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/metrics_saver.py` & `monai-weekly-1.3.dev2331/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/mlflow_handler.py` & `monai-weekly-1.3.dev2331/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/nvtx_handlers.py` & `monai-weekly-1.3.dev2331/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/panoptic_quality.py` & `monai-weekly-1.3.dev2331/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/parameter_scheduler.py` & `monai-weekly-1.3.dev2331/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/postprocessing.py` & `monai-weekly-1.3.dev2331/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/probability_maps.py` & `monai-weekly-1.3.dev2331/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/regression_metrics.py` & `monai-weekly-1.3.dev2331/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/roc_auc.py` & `monai-weekly-1.3.dev2331/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/smartcache_handler.py` & `monai-weekly-1.3.dev2331/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/stats_handler.py` & `monai-weekly-1.3.dev2331/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/surface_distance.py` & `monai-weekly-1.3.dev2331/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/tensorboard_handlers.py` & `monai-weekly-1.3.dev2331/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/utils.py` & `monai-weekly-1.3.dev2331/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/handlers/validation_handler.py` & `monai-weekly-1.3.dev2331/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/inferers/__init__.py` & `monai-weekly-1.3.dev2331/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/inferers/inferer.py` & `monai-weekly-1.3.dev2331/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/inferers/merger.py` & `monai-weekly-1.3.dev2331/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/inferers/splitter.py` & `monai-weekly-1.3.dev2331/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/inferers/utils.py` & `monai-weekly-1.3.dev2331/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/__init__.py` & `monai-weekly-1.3.dev2331/monai/losses/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from .cldice import SoftclDiceLoss, SoftDiceclDiceLoss
 from .contrastive import ContrastiveLoss
 from .deform import BendingEnergyLoss
 from .dice import (
     Dice,
     DiceCELoss,
     DiceFocalLoss,
     DiceLoss,
```

### Comparing `monai-weekly-1.3.dev2330/monai/losses/contrastive.py` & `monai-weekly-1.3.dev2331/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/deform.py` & `monai-weekly-1.3.dev2331/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/dice.py` & `monai-weekly-1.3.dev2331/monai/losses/dice.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,15 @@
                 - ``"none"``: no reduction will be applied.
                 - ``"mean"``: the sum of the output will be divided by the number of elements in the output.
                 - ``"sum"``: the output will be summed.
             smooth_nr: a small constant added to the numerator to avoid zero.
             smooth_dr: a small constant added to the denominator to avoid nan.
             batch: whether to sum the intersection and union areas over the batch dimension before the dividing.
                 Defaults to False, intersection over union is computed from each item in the batch.
+                If True, the class-weighted intersection and union areas are first summed across the batches.
 
         Raises:
             TypeError: When ``other_act`` is not an ``Optional[Callable]``.
             ValueError: When more than 1 of [``sigmoid=True``, ``softmax=True``, ``other_act is not None``].
                 Incompatible values.
 
         """
@@ -356,16 +357,17 @@
             w[infs] = 0.0
             w = w + infs * torch.max(w)
         else:
             w[infs] = 0.0
             max_values = torch.max(w, dim=1)[0].unsqueeze(dim=1)
             w = w + infs * max_values
 
-        numer = 2.0 * (intersection * w) + self.smooth_nr
-        denom = (denominator * w) + self.smooth_dr
+        final_reduce_dim = 0 if self.batch else 1
+        numer = 2.0 * (intersection * w).sum(final_reduce_dim, keepdim=True) + self.smooth_nr
+        denom = (denominator * w).sum(final_reduce_dim, keepdim=True) + self.smooth_dr
         f: torch.Tensor = 1.0 - (numer / denom)
 
         if self.reduction == LossReduction.MEAN.value:
             f = torch.mean(f)  # the batch and channel average
         elif self.reduction == LossReduction.SUM.value:
             f = torch.sum(f)  # sum over the batch and channel dims
         elif self.reduction == LossReduction.NONE.value:
```

### Comparing `monai-weekly-1.3.dev2330/monai/losses/ds_loss.py` & `monai-weekly-1.3.dev2331/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/focal_loss.py` & `monai-weekly-1.3.dev2331/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/giou_loss.py` & `monai-weekly-1.3.dev2331/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/image_dissimilarity.py` & `monai-weekly-1.3.dev2331/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/multi_scale.py` & `monai-weekly-1.3.dev2331/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/spatial_mask.py` & `monai-weekly-1.3.dev2331/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/ssim_loss.py` & `monai-weekly-1.3.dev2331/monai/losses/ssim_loss.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 - ``"none"``: no reduction will be applied.
                 - ``"mean"``: the sum of the output will be divided by the number of elements in the output.
                 - ``"sum"``: the output will be summed.
 
         """
         super().__init__(reduction=LossReduction(reduction).value)
         self.spatial_dims = spatial_dims
-        self.data_range = data_range
+        self._data_range = data_range
         self.kernel_type = kernel_type
 
         if not isinstance(win_size, Sequence):
             win_size = ensure_tuple_rep(win_size, spatial_dims)
         self.kernel_size = win_size
 
         if not isinstance(kernel_sigma, Sequence):
@@ -73,22 +73,31 @@
         self.kernel_sigma = kernel_sigma
 
         self.k1 = k1
         self.k2 = k2
 
         self.ssim_metric = SSIMMetric(
             spatial_dims=self.spatial_dims,
-            data_range=self.data_range,
+            data_range=self._data_range,
             kernel_type=self.kernel_type,
             win_size=self.kernel_size,
             kernel_sigma=self.kernel_sigma,
             k1=self.k1,
             k2=self.k2,
         )
 
+    @property
+    def data_range(self) -> float:
+        return self._data_range
+
+    @data_range.setter
+    def data_range(self, value: float) -> None:
+        self._data_range = value
+        self.ssim_metric.data_range = value
+
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         """
         Args:
             input: batch of predicted images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
             target: batch of target images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
 
         Returns:
```

### Comparing `monai-weekly-1.3.dev2330/monai/losses/tversky.py` & `monai-weekly-1.3.dev2331/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/losses/unified_focal_loss.py` & `monai-weekly-1.3.dev2331/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/__init__.py` & `monai-weekly-1.3.dev2331/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/active_learning_metrics.py` & `monai-weekly-1.3.dev2331/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/confusion_matrix.py` & `monai-weekly-1.3.dev2331/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/cumulative_average.py` & `monai-weekly-1.3.dev2331/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/f_beta_score.py` & `monai-weekly-1.3.dev2331/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/froc.py` & `monai-weekly-1.3.dev2331/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/generalized_dice.py` & `monai-weekly-1.3.dev2331/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/hausdorff_distance.py` & `monai-weekly-1.3.dev2331/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/loss_metric.py` & `monai-weekly-1.3.dev2331/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/meandice.py` & `monai-weekly-1.3.dev2331/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/meaniou.py` & `monai-weekly-1.3.dev2331/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/metric.py` & `monai-weekly-1.3.dev2331/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/panoptic_quality.py` & `monai-weekly-1.3.dev2331/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/regression.py` & `monai-weekly-1.3.dev2331/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/rocauc.py` & `monai-weekly-1.3.dev2331/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/surface_dice.py` & `monai-weekly-1.3.dev2331/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/surface_distance.py` & `monai-weekly-1.3.dev2331/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/utils.py` & `monai-weekly-1.3.dev2331/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/metrics/wrapper.py` & `monai-weekly-1.3.dev2331/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/__init__.py` & `monai-weekly-1.3.dev2331/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/__init__.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/acti_norm.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/activation.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/aspp.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/backbone_fpn_utils.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/convolutions.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/crf.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/denseblock.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/dints_block.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/downsample.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/dynunet_block.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/encoder.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/fcn.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/feature_pyramid_network.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/fft_utils_t.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/localnet_block.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/mlp.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/patchembedding.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/regunet_block.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/segresnet_block.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/selfattention.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/squeeze_and_excitation.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/text_embedding.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/transformerblock.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/unetr_block.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/upsample.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/blocks/warp.py` & `monai-weekly-1.3.dev2331/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/__init__.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/convutils.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/drop_path.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/factories.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/filtering.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/gmm.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/simplelayers.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/spatial_transforms.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/utils.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/layers/weight_init.py` & `monai-weekly-1.3.dev2331/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/__init__.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/ahnet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/attentionunet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/autoencoder.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/basic_unet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/basic_unetplusplus.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/classifier.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/daf3d.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/daf3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/densenet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/dints.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/dynunet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/efficientnet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/flexible_unet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/fullyconnectednet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/generator.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/highresnet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/hovernet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/milmodel.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/netadapter.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/quicknat.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/quicknat.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/regressor.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/regunet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/resnet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/segresnet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/segresnet_ds.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/senet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/swin_unetr.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/torchvision_fc.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/transchex.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/unet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/unetr.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/varautoencoder.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/vit.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/vitautoenc.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/networks/nets/vnet.py` & `monai-weekly-1.3.dev2331/monai/networks/nets/vnet.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from __future__ import annotations
 
 import torch
 import torch.nn as nn
 
 from monai.networks.blocks.convolutions import Convolution
 from monai.networks.layers.factories import Act, Conv, Dropout, Norm, split_args
+from monai.utils import deprecated_arg
 
 __all__ = ["VNet"]
 
 
 def get_acti_layer(act: tuple[str, dict] | str, nchan: int = 0):
     if act == "prelu":
         act = ("prelu", {"num_parameters": nchan})
@@ -129,27 +130,27 @@
     def __init__(
         self,
         spatial_dims: int,
         in_channels: int,
         out_channels: int,
         nconvs: int,
         act: tuple[str, dict] | str,
-        dropout_prob: float | None = None,
+        dropout_prob: tuple[float | None, float] = (None, 0.5),
         dropout_dim: int = 3,
     ):
         super().__init__()
 
         conv_trans_type: type[nn.ConvTranspose2d | nn.ConvTranspose3d] = Conv[Conv.CONVTRANS, spatial_dims]
         norm_type: type[nn.BatchNorm2d | nn.BatchNorm3d] = Norm[Norm.BATCH, spatial_dims]
         dropout_type: type[nn.Dropout | nn.Dropout2d | nn.Dropout3d] = Dropout[Dropout.DROPOUT, dropout_dim]
 
         self.up_conv = conv_trans_type(in_channels, out_channels // 2, kernel_size=2, stride=2)
         self.bn1 = norm_type(out_channels // 2)
-        self.dropout = dropout_type(dropout_prob) if dropout_prob is not None else None
-        self.dropout2 = dropout_type(0.5)
+        self.dropout = dropout_type(dropout_prob[0]) if dropout_prob[0] is not None else None
+        self.dropout2 = dropout_type(dropout_prob[1])
         self.act_function1 = get_acti_layer(act, out_channels // 2)
         self.act_function2 = get_acti_layer(act, out_channels)
         self.ops = _make_nconv(spatial_dims, out_channels, nconvs, act)
 
     def forward(self, x, skipx):
         if self.dropout is not None:
             out = self.dropout(x)
@@ -202,48 +203,63 @@
 
     Args:
         spatial_dims: spatial dimension of the input data. Defaults to 3.
         in_channels: number of input channels for the network. Defaults to 1.
             The value should meet the condition that ``16 % in_channels == 0``.
         out_channels: number of output channels for the network. Defaults to 1.
         act: activation type in the network. Defaults to ``("elu", {"inplace": True})``.
-        dropout_prob: dropout ratio. Defaults to 0.5.
-        dropout_dim: determine the dimensions of dropout. Defaults to 3.
+        dropout_prob_down: dropout ratio for DownTransition blocks. Defaults to 0.5.
+        dropout_prob_up: dropout ratio for UpTransition blocks. Defaults to (0.5, 0.5).
+        dropout_dim: determine the dimensions of dropout. Defaults to (0.5, 0.5).
 
             - ``dropout_dim = 1``, randomly zeroes some of the elements for each channel.
             - ``dropout_dim = 2``, Randomly zeroes out entire channels (a channel is a 2D feature map).
             - ``dropout_dim = 3``, Randomly zeroes out entire channels (a channel is a 3D feature map).
         bias: whether to have a bias term in convolution blocks. Defaults to False.
             According to `Performance Tuning Guide <https://pytorch.org/tutorials/recipes/recipes/tuning_guide.html>`_,
             if a conv layer is directly followed by a batch norm layer, bias should be False.
 
+    .. deprecated:: 1.2
+        ``dropout_prob`` is deprecated in favor of ``dropout_prob_down`` and ``dropout_prob_up``.
+
     """
 
+    @deprecated_arg(
+        name="dropout_prob",
+        since="1.2",
+        new_name="dropout_prob_down",
+        msg_suffix="please use `dropout_prob_down` instead.",
+    )
+    @deprecated_arg(
+        name="dropout_prob", since="1.2", new_name="dropout_prob_up", msg_suffix="please use `dropout_prob_up` instead."
+    )
     def __init__(
         self,
         spatial_dims: int = 3,
         in_channels: int = 1,
         out_channels: int = 1,
         act: tuple[str, dict] | str = ("elu", {"inplace": True}),
-        dropout_prob: float = 0.5,
+        dropout_prob: float | None = 0.5,  # deprecated
+        dropout_prob_down: float | None = 0.5,
+        dropout_prob_up: tuple[float | None, float] = (0.5, 0.5),
         dropout_dim: int = 3,
         bias: bool = False,
     ):
         super().__init__()
 
         if spatial_dims not in (2, 3):
             raise AssertionError("spatial_dims can only be 2 or 3.")
 
         self.in_tr = InputTransition(spatial_dims, in_channels, 16, act, bias=bias)
         self.down_tr32 = DownTransition(spatial_dims, 16, 1, act, bias=bias)
         self.down_tr64 = DownTransition(spatial_dims, 32, 2, act, bias=bias)
-        self.down_tr128 = DownTransition(spatial_dims, 64, 3, act, dropout_prob=dropout_prob, bias=bias)
-        self.down_tr256 = DownTransition(spatial_dims, 128, 2, act, dropout_prob=dropout_prob, bias=bias)
-        self.up_tr256 = UpTransition(spatial_dims, 256, 256, 2, act, dropout_prob=dropout_prob)
-        self.up_tr128 = UpTransition(spatial_dims, 256, 128, 2, act, dropout_prob=dropout_prob)
+        self.down_tr128 = DownTransition(spatial_dims, 64, 3, act, dropout_prob=dropout_prob_down, bias=bias)
+        self.down_tr256 = DownTransition(spatial_dims, 128, 2, act, dropout_prob=dropout_prob_down, bias=bias)
+        self.up_tr256 = UpTransition(spatial_dims, 256, 256, 2, act, dropout_prob=dropout_prob_up)
+        self.up_tr128 = UpTransition(spatial_dims, 256, 128, 2, act, dropout_prob=dropout_prob_up)
         self.up_tr64 = UpTransition(spatial_dims, 128, 64, 1, act)
         self.up_tr32 = UpTransition(spatial_dims, 64, 32, 1, act)
         self.out_tr = OutputTransition(spatial_dims, 32, out_channels, act, bias=bias)
 
     def forward(self, x):
         out16 = self.in_tr(x)
         out32 = self.down_tr32(out16)
```

### Comparing `monai-weekly-1.3.dev2330/monai/networks/utils.py` & `monai-weekly-1.3.dev2331/monai/networks/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/optimizers/__init__.py` & `monai-weekly-1.3.dev2331/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/optimizers/lr_finder.py` & `monai-weekly-1.3.dev2331/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/optimizers/lr_scheduler.py` & `monai-weekly-1.3.dev2331/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/optimizers/novograd.py` & `monai-weekly-1.3.dev2331/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/optimizers/utils.py` & `monai-weekly-1.3.dev2331/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     ScaleIntensity,
     ScaleIntensityFixedMean,
     ScaleIntensityRange,
     ScaleIntensityRangePercentiles,
     ShiftIntensity,
     StdShiftIntensity,
     ThresholdIntensity,
+    UltrasoundConfidenceMapTransform,
 )
 from .intensity.dictionary import (
     AdjustContrastd,
     AdjustContrastD,
     AdjustContrastDict,
     ComputeHoVerMapsd,
     ComputeHoVerMapsD,
```

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/adaptors.py` & `monai-weekly-1.3.dev2331/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/compose.py` & `monai-weekly-1.3.dev2331/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/croppad/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/croppad/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/croppad/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/croppad/batch.py` & `monai-weekly-1.3.dev2331/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/croppad/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/croppad/functional.py` & `monai-weekly-1.3.dev2331/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/intensity/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/intensity/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/intensity/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 import numpy as np
 import torch
 
 from monai.config import DtypeLike
 from monai.config.type_definitions import NdarrayOrTensor, NdarrayTensor
 from monai.data.meta_obj import get_track_meta
+from monai.data.ultrasound_confidence_map import UltrasoundConfidenceMap
 from monai.data.utils import get_random_patch, get_valid_patch_size
 from monai.networks.layers import GaussianFilter, HilbertTransform, MedianFilter, SavitzkyGolayFilter
 from monai.transforms.transform import RandomizableTransform, Transform
 from monai.transforms.utils import Fourier, equalize_hist, is_positive, rescale_array
 from monai.transforms.utils_pytorch_numpy_unification import clip, percentile, where
 from monai.utils.enums import TransformBackends
 from monai.utils.misc import ensure_tuple, ensure_tuple_rep, ensure_tuple_size, fall_back_tuple
@@ -73,14 +74,15 @@
     "RandCoarseDropout",
     "RandCoarseShuffle",
     "HistogramNormalize",
     "IntensityRemap",
     "RandIntensityRemap",
     "ForegroundMask",
     "ComputeHoVerMaps",
+    "UltrasoundConfidenceMapTransform",
 ]
 
 
 class RandGaussianNoise(RandomizableTransform):
     """
     Add Gaussian noise to image.
 
@@ -487,16 +489,16 @@
         """
         Args:
             factor: factor scale by ``v = v * (1 + factor)``.
             preserve_range: clips the output array/tensor to the range of the input array/tensor
             fixed_mean: subtract the mean intensity before scaling with `factor`, then add the same value after scaling
                 to ensure that the output has the same mean as the input.
             channel_wise: if True, scale on each channel separately. `preserve_range` and `fixed_mean` are also applied
-            on each channel separately if `channel_wise` is True. Please ensure that the first dimension represents the
-            channel of the image if True.
+                on each channel separately if `channel_wise` is True. Please ensure that the first dimension represents the
+                channel of the image if True.
             dtype: output data type, if None, same as input image. defaults to float32.
         """
         self.factor = factor
         self.preserve_range = preserve_range
         self.fixed_mean = fixed_mean
         self.channel_wise = channel_wise
         self.dtype = dtype
@@ -627,51 +629,72 @@
     """
     Randomly scale the intensity of input image by ``v = v * (1 + factor)`` where the `factor`
     is randomly picked.
     """
 
     backend = ScaleIntensity.backend
 
-    def __init__(self, factors: tuple[float, float] | float, prob: float = 0.1, dtype: DtypeLike = np.float32) -> None:
+    def __init__(
+        self,
+        factors: tuple[float, float] | float,
+        prob: float = 0.1,
+        channel_wise: bool = False,
+        dtype: DtypeLike = np.float32,
+    ) -> None:
         """
         Args:
             factors: factor range to randomly scale by ``v = v * (1 + factor)``.
                 if single number, factor value is picked from (-factors, factors).
             prob: probability of scale.
+            channel_wise: if True, scale on each channel separately. Please ensure
+                that the first dimension represents the channel of the image if True.
             dtype: output data type, if None, same as input image. defaults to float32.
 
         """
         RandomizableTransform.__init__(self, prob)
         if isinstance(factors, (int, float)):
             self.factors = (min(-factors, factors), max(-factors, factors))
         elif len(factors) != 2:
             raise ValueError(f"factors should be a number or pair of numbers, got {factors}.")
         else:
             self.factors = (min(factors), max(factors))
         self.factor = self.factors[0]
+        self.channel_wise = channel_wise
         self.dtype = dtype
 
     def randomize(self, data: Any | None = None) -> None:
         super().randomize(None)
         if not self._do_transform:
             return None
-        self.factor = self.R.uniform(low=self.factors[0], high=self.factors[1])
+        if self.channel_wise:
+            self.factor = [self.R.uniform(low=self.factors[0], high=self.factors[1]) for _ in range(data.shape[0])]  # type: ignore
+        else:
+            self.factor = self.R.uniform(low=self.factors[0], high=self.factors[1])
 
     def __call__(self, img: NdarrayOrTensor, randomize: bool = True) -> NdarrayOrTensor:
         """
         Apply the transform to `img`.
         """
         img = convert_to_tensor(img, track_meta=get_track_meta())
         if randomize:
-            self.randomize()
+            self.randomize(img)
 
         if not self._do_transform:
             return convert_data_type(img, dtype=self.dtype)[0]
 
-        return ScaleIntensity(minv=None, maxv=None, factor=self.factor, dtype=self.dtype)(img)
+        ret: NdarrayOrTensor
+        if self.channel_wise:
+            out = []
+            for i, d in enumerate(img):
+                out_channel = ScaleIntensity(minv=None, maxv=None, factor=self.factor[i], dtype=self.dtype)(d)  # type: ignore
+                out.append(out_channel)
+            ret = torch.stack(out)  # type: ignore
+        else:
+            ret = ScaleIntensity(minv=None, maxv=None, factor=self.factor, dtype=self.dtype)(img)
+        return ret
 
 
 class RandBiasField(RandomizableTransform):
     """
     Random bias field augmentation for MR images.
     The bias field is considered as a linear combination of smoothly varying basis (polynomial)
     functions, as described in `Automated Model-Based Tissue Classification of MR Images of the Brain
@@ -2573,7 +2596,84 @@
             v_dist[v_dist > 0] /= np.amax(v_dist)
 
             h_map[h_map == region.label] = h_dist
             v_map[v_map == region.label] = v_dist
 
         hv_maps = convert_to_tensor(np.concatenate([h_map, v_map]), track_meta=get_track_meta())
         return hv_maps
+
+
+class UltrasoundConfidenceMapTransform(Transform):
+    """Compute confidence map from an ultrasound image.
+    This transform uses the method introduced by Karamalis et al. in https://doi.org/10.1016/j.media.2012.07.005.
+    It generates a confidence map by setting source and sink points in the image and computing the probability
+    for random walks to reach the source for each pixel.
+
+    Args:
+        alpha (float, optional): Alpha parameter. Defaults to 2.0.
+        beta (float, optional): Beta parameter. Defaults to 90.0.
+        gamma (float, optional): Gamma parameter. Defaults to 0.05.
+        mode (str, optional): 'RF' or 'B' mode data. Defaults to 'B'.
+        sink_mode (str, optional): Sink mode. Defaults to 'all'. If 'mask' is selected, a mask must be when
+            calling the transform. Can be one of 'all', 'mid', 'min', 'mask'.
+    """
+
+    def __init__(self, alpha: float = 2.0, beta: float = 90.0, gamma: float = 0.05, mode="B", sink_mode="all") -> None:
+        self.alpha = alpha
+        self.beta = beta
+        self.gamma = gamma
+        self.mode = mode
+        self.sink_mode = sink_mode
+
+        if self.mode not in ["B", "RF"]:
+            raise ValueError(f"Unknown mode: {self.mode}. Supported modes are 'B' and 'RF'.")
+
+        if self.sink_mode not in ["all", "mid", "min", "mask"]:
+            raise ValueError(
+                f"Unknown sink mode: {self.sink_mode}. Supported modes are 'all', 'mid', 'min' and 'mask'."
+            )
+
+        self._compute_conf_map = UltrasoundConfidenceMap(self.alpha, self.beta, self.gamma, self.mode, self.sink_mode)
+
+    def __call__(self, img: NdarrayOrTensor, mask: NdarrayOrTensor | None = None) -> NdarrayOrTensor:
+        """Compute confidence map from an ultrasound image.
+
+        Args:
+            img (ndarray or Tensor): Ultrasound image of shape [1, H, W] or [1, D, H, W]. If the image has channels,
+                they will be averaged before computing the confidence map.
+            mask (ndarray or Tensor, optional): Mask of shape [1, H, W]. Defaults to None. Must be
+                provided when sink mode is 'mask'. The non-zero values of the mask are used as sink points.
+
+        Returns:
+            ndarray or Tensor: Confidence map of shape [1, H, W].
+        """
+
+        if self.sink_mode == "mask" and mask is None:
+            raise ValueError("A mask must be provided when sink mode is 'mask'.")
+
+        if img.shape[0] != 1:
+            raise ValueError("The correct shape of the image is [1, H, W] or [1, D, H, W].")
+
+        _img = convert_to_tensor(img, track_meta=get_track_meta())
+        img_np, *_ = convert_data_type(_img, np.ndarray)
+        img_np = img_np[0]  # Remove the first dimension
+
+        mask_np = None
+        if mask is not None:
+            mask = convert_to_tensor(mask, dtype=torch.bool, track_meta=get_track_meta())
+            mask_np, *_ = convert_data_type(mask, np.ndarray)
+            mask_np = mask_np[0]  # Remove the first dimension
+
+        # If the image is RGB, convert it to grayscale
+        if len(img_np.shape) == 3:
+            img_np = np.mean(img_np, axis=0)
+
+        if mask_np is not None and mask_np.shape != img_np.shape:
+            raise ValueError("The mask must have the same shape as the image.")
+
+        # Compute confidence map
+        conf_map: NdarrayOrTensor = self._compute_conf_map(img_np, mask_np)
+
+        if type(img) is torch.Tensor:
+            conf_map = torch.from_numpy(conf_map)
+
+        return conf_map
```

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/intensity/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/intensity/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,32 +582,35 @@
     backend = RandScaleIntensity.backend
 
     def __init__(
         self,
         keys: KeysCollection,
         factors: tuple[float, float] | float,
         prob: float = 0.1,
+        channel_wise: bool = False,
         dtype: DtypeLike = np.float32,
         allow_missing_keys: bool = False,
     ) -> None:
         """
         Args:
             keys: keys of the corresponding items to be transformed.
                 See also: :py:class:`monai.transforms.compose.MapTransform`
             factors: factor range to randomly scale by ``v = v * (1 + factor)``.
                 if single number, factor value is picked from (-factors, factors).
             prob: probability of scale.
                 (Default 0.1, with 10% probability it returns a scaled array.)
+            channel_wise: if True, scale on each channel separately. Please ensure
+                that the first dimension represents the channel of the image if True.
             dtype: output data type, if None, same as input image. defaults to float32.
             allow_missing_keys: don't raise exception if key is missing.
 
         """
         MapTransform.__init__(self, keys, allow_missing_keys)
         RandomizableTransform.__init__(self, prob)
-        self.scaler = RandScaleIntensity(factors=factors, dtype=dtype, prob=1.0)
+        self.scaler = RandScaleIntensity(factors=factors, dtype=dtype, prob=1.0, channel_wise=channel_wise)
 
     def set_random_state(
         self, seed: int | None = None, state: np.random.RandomState | None = None
     ) -> RandScaleIntensityd:
         super().set_random_state(seed, state)
         self.scaler.set_random_state(seed, state)
         return self
@@ -616,16 +619,23 @@
         d = dict(data)
         self.randomize(None)
         if not self._do_transform:
             for key in self.key_iterator(d):
                 d[key] = convert_to_tensor(d[key], track_meta=get_track_meta())
             return d
 
+        # expect all the specified keys have same spatial shape and share same random holes
+        first_key: Hashable = self.first_key(d)
+        if first_key == ():
+            for key in self.key_iterator(d):
+                d[key] = convert_to_tensor(d[key], track_meta=get_track_meta())
+            return d
+
         # all the keys share the same random scale factor
-        self.scaler.randomize(None)
+        self.scaler.randomize(d[first_key])
         for key in self.key_iterator(d):
             d[key] = self.scaler(d[key], randomize=False)
         return d
 
 
 class RandScaleIntensityFixedMeand(RandomizableTransform, MapTransform):
     """
```

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/inverse.py` & `monai-weekly-1.3.dev2331/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/inverse_batch_transform.py` & `monai-weekly-1.3.dev2331/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/io/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/io/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/io/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/lazy/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/lazy/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/lazy/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/lazy/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/lazy/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/lazy/functional.py` & `monai-weekly-1.3.dev2331/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/lazy/utils.py` & `monai-weekly-1.3.dev2331/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/meta_utility/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/meta_utility/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/nvtx.py` & `monai-weekly-1.3.dev2331/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/post/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/post/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/post/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/signal/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/signal/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/smooth_field/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/smooth_field/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/smooth_field/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/spatial/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/spatial/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/spatial/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -2519,14 +2519,16 @@
         do_resampling = self._do_transform or (sp_size != ensure_tuple(ori_size))
         _mode = mode if mode is not None else self.mode
         _padding_mode = padding_mode if padding_mode is not None else self.padding_mode
         lazy_ = self.lazy if lazy is None else lazy
         img = convert_to_tensor(img, track_meta=get_track_meta())
         if lazy_:
             if self._do_transform:
+                if grid is None:
+                    self.rand_affine_grid(sp_size, randomize=randomize, lazy=True)
                 affine = self.rand_affine_grid.get_transformation_matrix()
             else:
                 affine = convert_to_dst_type(torch.eye(len(sp_size) + 1), img, dtype=self.rand_affine_grid.dtype)[0]
         else:
             if grid is None:
                 grid = self.get_identity_grid(sp_size, lazy_)
                 if self._do_transform:
```

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/spatial/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/spatial/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1137,14 +1137,15 @@
         do_resampling = self._do_transform or (sp_size != ensure_tuple(spatial_size))
         # converting affine to tensor because the resampler currently only support torch backend
         grid = None
         if do_resampling:  # need to prepare grid
             grid = self.rand_affine.get_identity_grid(sp_size, lazy=lazy_)
             if self._do_transform:  # add some random factors
                 grid = self.rand_affine.rand_affine_grid(sp_size, grid=grid, lazy=lazy_)
+        grid = 0 if grid is None else grid  # always provide a grid to self.rand_affine
 
         for key, mode, padding_mode in self.key_iterator(d, self.mode, self.padding_mode):
             # do the transform
             if do_resampling:
                 d[key] = self.rand_affine(d[key], None, mode, padding_mode, True, grid, lazy=lazy_)  # type: ignore
             else:
                 d[key] = convert_to_tensor(d[key], track_meta=get_track_meta(), dtype=torch.float32)
```

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/spatial/functional.py` & `monai-weekly-1.3.dev2331/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/traits.py` & `monai-weekly-1.3.dev2331/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/transform.py` & `monai-weekly-1.3.dev2331/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/utility/__init__.py` & `monai-weekly-1.3.dev2331/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/utility/array.py` & `monai-weekly-1.3.dev2331/monai/transforms/utility/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/utility/dictionary.py` & `monai-weekly-1.3.dev2331/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/utils.py` & `monai-weekly-1.3.dev2331/monai/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/utils_create_transform_ims.py` & `monai-weekly-1.3.dev2331/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/transforms/utils_pytorch_numpy_unification.py` & `monai-weekly-1.3.dev2331/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/__init__.py` & `monai-weekly-1.3.dev2331/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/aliases.py` & `monai-weekly-1.3.dev2331/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/decorators.py` & `monai-weekly-1.3.dev2331/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/deprecate_utils.py` & `monai-weekly-1.3.dev2331/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/dist.py` & `monai-weekly-1.3.dev2331/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/enums.py` & `monai-weekly-1.3.dev2331/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/jupyter_utils.py` & `monai-weekly-1.3.dev2331/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/misc.py` & `monai-weekly-1.3.dev2331/monai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/module.py` & `monai-weekly-1.3.dev2331/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/nvtx.py` & `monai-weekly-1.3.dev2331/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/profiling.py` & `monai-weekly-1.3.dev2331/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/state_cacher.py` & `monai-weekly-1.3.dev2331/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/utils/type_conversion.py` & `monai-weekly-1.3.dev2331/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/visualize/__init__.py` & `monai-weekly-1.3.dev2331/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/visualize/class_activation_maps.py` & `monai-weekly-1.3.dev2331/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/visualize/gradient_based.py` & `monai-weekly-1.3.dev2331/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/visualize/img2tensorboard.py` & `monai-weekly-1.3.dev2331/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/visualize/occlusion_sensitivity.py` & `monai-weekly-1.3.dev2331/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/visualize/utils.py` & `monai-weekly-1.3.dev2331/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai/visualize/visualizer.py` & `monai-weekly-1.3.dev2331/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/monai_weekly.egg-info/PKG-INFO` & `monai-weekly-1.3.dev2331/monai_weekly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.3.dev2330
+Version: 1.3.dev2331
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -28,14 +28,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: all
 Provides-Extra: nibabel
 Provides-Extra: ninja
 Provides-Extra: skimage
+Provides-Extra: scipy
 Provides-Extra: pillow
 Provides-Extra: tensorboard
 Provides-Extra: gdown
 Provides-Extra: ignite
 Provides-Extra: torchvision
 Provides-Extra: itk
 Provides-Extra: tqdm
```

### Comparing `monai-weekly-1.3.dev2330/monai_weekly.egg-info/SOURCES.txt` & `monai-weekly-1.3.dev2331/monai_weekly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 monai/data/meta_obj.py
 monai/data/meta_tensor.py
 monai/data/samplers.py
 monai/data/synthetic.py
 monai/data/test_time_augmentation.py
 monai/data/thread_buffer.py
 monai/data/torchscript_utils.py
+monai/data/ultrasound_confidence_map.py
 monai/data/utils.py
 monai/data/video_dataset.py
 monai/data/wsi_datasets.py
 monai/data/wsi_reader.py
 monai/engines/__init__.py
 monai/engines/evaluator.py
 monai/engines/multi_gpu_supervised_trainer.py
@@ -191,14 +192,15 @@
 monai/handlers/validation_handler.py
 monai/inferers/__init__.py
 monai/inferers/inferer.py
 monai/inferers/merger.py
 monai/inferers/splitter.py
 monai/inferers/utils.py
 monai/losses/__init__.py
+monai/losses/cldice.py
 monai/losses/contrastive.py
 monai/losses/deform.py
 monai/losses/dice.py
 monai/losses/ds_loss.py
 monai/losses/focal_loss.py
 monai/losses/giou_loss.py
 monai/losses/image_dissimilarity.py
@@ -447,14 +449,15 @@
 tests/test_center_spatial_crop.py
 tests/test_center_spatial_cropd.py
 tests/test_channel_pad.py
 tests/test_check_hash.py
 tests/test_check_missing_files.py
 tests/test_classes_to_indices.py
 tests/test_classes_to_indicesd.py
+tests/test_cldice_loss.py
 tests/test_complex_utils.py
 tests/test_component_locator.py
 tests/test_compose.py
 tests/test_compose_get_number_conversions.py
 tests/test_compute_confusion_matrix.py
 tests/test_compute_f_beta.py
 tests/test_compute_froc.py
@@ -574,14 +577,15 @@
 tests/test_fullyconnectednet.py
 tests/test_gaussian.py
 tests/test_gaussian_filter.py
 tests/test_gaussian_sharpen.py
 tests/test_gaussian_sharpend.py
 tests/test_gaussian_smooth.py
 tests/test_gaussian_smoothd.py
+tests/test_gdsdataset.py
 tests/test_generalized_dice_focal_loss.py
 tests/test_generalized_dice_loss.py
 tests/test_generalized_wasserstein_dice_loss.py
 tests/test_generate_distance_map.py
 tests/test_generate_distance_mapd.py
 tests/test_generate_instance_border.py
 tests/test_generate_instance_borderd.py
@@ -1045,14 +1049,15 @@
 tests/test_trainable_joint_bilateral.py
 tests/test_transchex.py
 tests/test_transform.py
 tests/test_transformerblock.py
 tests/test_transpose.py
 tests/test_transposed.py
 tests/test_tversky_loss.py
+tests/test_ultrasound_confidence_map_transform.py
 tests/test_unet.py
 tests/test_unetr.py
 tests/test_unetr_block.py
 tests/test_unified_focal_loss.py
 tests/test_upsample_block.py
 tests/test_utils_pytorch_numpy_unification.py
 tests/test_varautoencoder.py
```

### Comparing `monai-weekly-1.3.dev2330/monai_weekly.egg-info/requires.txt` & `monai-weekly-1.3.dev2331/monai_weekly.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 torch>=1.9
 numpy>=1.20
 
 [all]
 nibabel
 ninja
 scikit-image>=0.14.2
+scipy>=1.7.1
 pillow
 tensorboard
 gdown>=4.4.0
 pytorch-ignite==0.4.11
 torchvision
 itk>=5.2
 tqdm>=4.47.0
@@ -110,14 +111,17 @@
 
 [pynrrd]
 pynrrd
 
 [pyyaml]
 pyyaml
 
+[scipy]
+scipy>=1.7.1
+
 [skimage]
 scikit-image>=0.14.2
 
 [tensorboard]
 tensorboard
 
 [tensorboardX]
```

### Comparing `monai-weekly-1.3.dev2330/pyproject.toml` & `monai-weekly-1.3.dev2331/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/setup.cfg` & `monai-weekly-1.3.dev2331/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 	numpy>=1.20
 
 [options.extras_require]
 all = 
 	nibabel
 	ninja
 	scikit-image>=0.14.2
+	scipy>=1.7.1
 	pillow
 	tensorboard
 	gdown>=4.4.0
 	pytorch-ignite==0.4.11
 	torchvision
 	itk>=5.2
 	tqdm>=4.47.0
@@ -79,14 +80,16 @@
 	zarr
 nibabel = 
 	nibabel
 ninja = 
 	ninja
 skimage = 
 	scikit-image>=0.14.2
+scipy = 
+	scipy>=1.7.1
 pillow = 
 	pillow!=8.3.0
 tensorboard = 
 	tensorboard
 gdown = 
 	gdown>=4.4.0
 ignite =
```

### Comparing `monai-weekly-1.3.dev2330/setup.py` & `monai-weekly-1.3.dev2331/setup.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_acn_block.py` & `monai-weekly-1.3.dev2331/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_activations.py` & `monai-weekly-1.3.dev2331/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_activationsd.py` & `monai-weekly-1.3.dev2331/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_adaptors.py` & `monai-weekly-1.3.dev2331/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_add_channeld.py` & `monai-weekly-1.3.dev2331/tests/test_add_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_add_coordinate_channels.py` & `monai-weekly-1.3.dev2331/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_add_coordinate_channelsd.py` & `monai-weekly-1.3.dev2331/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_add_extreme_points_channel.py` & `monai-weekly-1.3.dev2331/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_add_extreme_points_channeld.py` & `monai-weekly-1.3.dev2331/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_adjust_contrast.py` & `monai-weekly-1.3.dev2331/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_adjust_contrastd.py` & `monai-weekly-1.3.dev2331/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_adn.py` & `monai-weekly-1.3.dev2331/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_affine.py` & `monai-weekly-1.3.dev2331/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_affine_grid.py` & `monai-weekly-1.3.dev2331/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_affine_transform.py` & `monai-weekly-1.3.dev2331/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_affined.py` & `monai-weekly-1.3.dev2331/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ahnet.py` & `monai-weekly-1.3.dev2331/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_alias.py` & `monai-weekly-1.3.dev2331/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_anchor_box.py` & `monai-weekly-1.3.dev2331/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_apply.py` & `monai-weekly-1.3.dev2331/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_apply_filter.py` & `monai-weekly-1.3.dev2331/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_arraydataset.py` & `monai-weekly-1.3.dev2331/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_as_channel_first.py` & `monai-weekly-1.3.dev2331/tests/test_as_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_as_channel_firstd.py` & `monai-weekly-1.3.dev2331/tests/test_as_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_as_channel_last.py` & `monai-weekly-1.3.dev2331/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_as_channel_lastd.py` & `monai-weekly-1.3.dev2331/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_as_discrete.py` & `monai-weekly-1.3.dev2331/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_as_discreted.py` & `monai-weekly-1.3.dev2331/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_atss_box_matcher.py` & `monai-weekly-1.3.dev2331/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_attentionunet.py` & `monai-weekly-1.3.dev2331/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_auto3dseg.py` & `monai-weekly-1.3.dev2331/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_auto3dseg_bundlegen.py` & `monai-weekly-1.3.dev2331/tests/test_auto3dseg_bundlegen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_auto3dseg_ensemble.py` & `monai-weekly-1.3.dev2331/tests/test_auto3dseg_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_auto3dseg_hpo.py` & `monai-weekly-1.3.dev2331/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_autoencoder.py` & `monai-weekly-1.3.dev2331/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_avg_merger.py` & `monai-weekly-1.3.dev2331/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_basic_unet.py` & `monai-weekly-1.3.dev2331/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_basic_unetplusplus.py` & `monai-weekly-1.3.dev2331/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bending_energy.py` & `monai-weekly-1.3.dev2331/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bilateral_approx_cpu.py` & `monai-weekly-1.3.dev2331/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bilateral_approx_cuda.py` & `monai-weekly-1.3.dev2331/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bilateral_precise.py` & `monai-weekly-1.3.dev2331/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_blend_images.py` & `monai-weekly-1.3.dev2331/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_border_pad.py` & `monai-weekly-1.3.dev2331/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_border_padd.py` & `monai-weekly-1.3.dev2331/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bounding_rect.py` & `monai-weekly-1.3.dev2331/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bounding_rectd.py` & `monai-weekly-1.3.dev2331/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_box_coder.py` & `monai-weekly-1.3.dev2331/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_box_transform.py` & `monai-weekly-1.3.dev2331/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_box_utils.py` & `monai-weekly-1.3.dev2331/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_ckpt_export.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_download.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_get_data.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_init_bundle.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_onnx_export.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_trt_export.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_utils.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_verify_metadata.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_verify_net.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_bundle_workflow.py` & `monai-weekly-1.3.dev2331/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cachedataset.py` & `monai-weekly-1.3.dev2331/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cachedataset_parallel.py` & `monai-weekly-1.3.dev2331/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cachedataset_persistent_workers.py` & `monai-weekly-1.3.dev2331/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cachentransdataset.py` & `monai-weekly-1.3.dev2331/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_call_dist.py` & `monai-weekly-1.3.dev2331/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cast_to_type.py` & `monai-weekly-1.3.dev2331/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cast_to_typed.py` & `monai-weekly-1.3.dev2331/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_center_scale_crop.py` & `monai-weekly-1.3.dev2331/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_center_scale_cropd.py` & `monai-weekly-1.3.dev2331/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_center_spatial_crop.py` & `monai-weekly-1.3.dev2331/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_center_spatial_cropd.py` & `monai-weekly-1.3.dev2331/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_channel_pad.py` & `monai-weekly-1.3.dev2331/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_check_hash.py` & `monai-weekly-1.3.dev2331/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_check_missing_files.py` & `monai-weekly-1.3.dev2331/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_classes_to_indices.py` & `monai-weekly-1.3.dev2331/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_classes_to_indicesd.py` & `monai-weekly-1.3.dev2331/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_complex_utils.py` & `monai-weekly-1.3.dev2331/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_component_locator.py` & `monai-weekly-1.3.dev2331/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compose.py` & `monai-weekly-1.3.dev2331/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compose_get_number_conversions.py` & `monai-weekly-1.3.dev2331/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_confusion_matrix.py` & `monai-weekly-1.3.dev2331/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_f_beta.py` & `monai-weekly-1.3.dev2331/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_froc.py` & `monai-weekly-1.3.dev2331/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_generalized_dice.py` & `monai-weekly-1.3.dev2331/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_ho_ver_maps.py` & `monai-weekly-1.3.dev2331/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_ho_ver_maps_d.py` & `monai-weekly-1.3.dev2331/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_meandice.py` & `monai-weekly-1.3.dev2331/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_meaniou.py` & `monai-weekly-1.3.dev2331/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_panoptic_quality.py` & `monai-weekly-1.3.dev2331/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_regression_metrics.py` & `monai-weekly-1.3.dev2331/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_roc_auc.py` & `monai-weekly-1.3.dev2331/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_compute_variance.py` & `monai-weekly-1.3.dev2331/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_concat_itemsd.py` & `monai-weekly-1.3.dev2331/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_config_item.py` & `monai-weekly-1.3.dev2331/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_config_parser.py` & `monai-weekly-1.3.dev2331/tests/test_config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
             self.assertTrue(isinstance(parser.get_parsed_content(id), cls))
         # test root content
         root = parser.get_parsed_content(id="")
         for v, cls in zip(root.values(), [Compose, Dataset, DataLoader]):
             self.assertTrue(isinstance(v, cls))
         # test default value
         self.assertEqual(parser.get_parsed_content(id="abc", default=ConfigItem(12345, "abc")), 12345)
+        self.assertEqual(parser.get_parsed_content(id="abcd", default=1), 1)
 
     @parameterized.expand([TEST_CASE_2])
     def test_function(self, config):
         parser = ConfigParser(config=config, globals={"TestClass": TestClass})
         for id in config:
             if id in ("compute", "cls_compute"):
                 parser[f"{id}#_mode_"] = "partial"
```

### Comparing `monai-weekly-1.3.dev2330/tests/test_contrastive_loss.py` & `monai-weekly-1.3.dev2331/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_convert_data_type.py` & `monai-weekly-1.3.dev2331/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_convert_to_multi_channel.py` & `monai-weekly-1.3.dev2331/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_convert_to_multi_channeld.py` & `monai-weekly-1.3.dev2331/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_convert_to_onnx.py` & `monai-weekly-1.3.dev2331/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_convert_to_torchscript.py` & `monai-weekly-1.3.dev2331/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_convert_to_trt.py` & `monai-weekly-1.3.dev2331/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_convolutions.py` & `monai-weekly-1.3.dev2331/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_copy_itemsd.py` & `monai-weekly-1.3.dev2331/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_copy_model_state.py` & `monai-weekly-1.3.dev2331/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_correct_crop_centers.py` & `monai-weekly-1.3.dev2331/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_create_cross_validation_datalist.py` & `monai-weekly-1.3.dev2331/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_create_grid_and_affine.py` & `monai-weekly-1.3.dev2331/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_crf_cpu.py` & `monai-weekly-1.3.dev2331/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_crf_cuda.py` & `monai-weekly-1.3.dev2331/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_crop_foreground.py` & `monai-weekly-1.3.dev2331/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_crop_foregroundd.py` & `monai-weekly-1.3.dev2331/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cross_validation.py` & `monai-weekly-1.3.dev2331/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_csv_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_csv_iterable_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_csv_saver.py` & `monai-weekly-1.3.dev2331/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cucim_dict_transform.py` & `monai-weekly-1.3.dev2331/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cucim_transform.py` & `monai-weekly-1.3.dev2331/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cumulative.py` & `monai-weekly-1.3.dev2331/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cumulative_average.py` & `monai-weekly-1.3.dev2331/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cumulative_average_dist.py` & `monai-weekly-1.3.dev2331/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_cv2_dist.py` & `monai-weekly-1.3.dev2331/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_daf3d.py` & `monai-weekly-1.3.dev2331/tests/test_daf3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_data_stats.py` & `monai-weekly-1.3.dev2331/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_data_statsd.py` & `monai-weekly-1.3.dev2331/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dataloader.py` & `monai-weekly-1.3.dev2331/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dataset_func.py` & `monai-weekly-1.3.dev2331/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dataset_summary.py` & `monai-weekly-1.3.dev2331/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_decathlondataset.py` & `monai-weekly-1.3.dev2331/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_decollate.py` & `monai-weekly-1.3.dev2331/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_deepedit_interaction.py` & `monai-weekly-1.3.dev2331/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_deepedit_transforms.py` & `monai-weekly-1.3.dev2331/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_deepgrow_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_deepgrow_interaction.py` & `monai-weekly-1.3.dev2331/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_deepgrow_transforms.py` & `monai-weekly-1.3.dev2331/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_delete_itemsd.py` & `monai-weekly-1.3.dev2331/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_denseblock.py` & `monai-weekly-1.3.dev2331/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_densenet.py` & `monai-weekly-1.3.dev2331/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_deprecated.py` & `monai-weekly-1.3.dev2331/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_detect_envelope.py` & `monai-weekly-1.3.dev2331/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_detection_coco_metrics.py` & `monai-weekly-1.3.dev2331/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_detector_boxselector.py` & `monai-weekly-1.3.dev2331/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_detector_utils.py` & `monai-weekly-1.3.dev2331/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dev_collate.py` & `monai-weekly-1.3.dev2331/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dice_ce_loss.py` & `monai-weekly-1.3.dev2331/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dice_focal_loss.py` & `monai-weekly-1.3.dev2331/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dice_loss.py` & `monai-weekly-1.3.dev2331/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dints_cell.py` & `monai-weekly-1.3.dev2331/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dints_mixop.py` & `monai-weekly-1.3.dev2331/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dints_network.py` & `monai-weekly-1.3.dev2331/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_discriminator.py` & `monai-weekly-1.3.dev2331/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_divisible_pad.py` & `monai-weekly-1.3.dev2331/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_divisible_padd.py` & `monai-weekly-1.3.dev2331/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_download_and_extract.py` & `monai-weekly-1.3.dev2331/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_download_url_yandex.py` & `monai-weekly-1.3.dev2331/tests/test_download_url_yandex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_downsample_block.py` & `monai-weekly-1.3.dev2331/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_drop_path.py` & `monai-weekly-1.3.dev2331/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ds_loss.py` & `monai-weekly-1.3.dev2331/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dvf2ddf.py` & `monai-weekly-1.3.dev2331/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dynunet.py` & `monai-weekly-1.3.dev2331/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_dynunet_block.py` & `monai-weekly-1.3.dev2331/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_efficientnet.py` & `monai-weekly-1.3.dev2331/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ensemble_evaluator.py` & `monai-weekly-1.3.dev2331/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ensure_channel_first.py` & `monai-weekly-1.3.dev2331/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ensure_channel_firstd.py` & `monai-weekly-1.3.dev2331/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ensure_tuple.py` & `monai-weekly-1.3.dev2331/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ensure_type.py` & `monai-weekly-1.3.dev2331/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ensure_typed.py` & `monai-weekly-1.3.dev2331/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_enum_bound_interp.py` & `monai-weekly-1.3.dev2331/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_eval_mode.py` & `monai-weekly-1.3.dev2331/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_evenly_divisible_all_gather_dist.py` & `monai-weekly-1.3.dev2331/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_factorized_increase.py` & `monai-weekly-1.3.dev2331/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_factorized_reduce.py` & `monai-weekly-1.3.dev2331/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fastmri_reader.py` & `monai-weekly-1.3.dev2331/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fft_utils.py` & `monai-weekly-1.3.dev2331/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fg_bg_to_indices.py` & `monai-weekly-1.3.dev2331/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fg_bg_to_indicesd.py` & `monai-weekly-1.3.dev2331/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_file_basename.py` & `monai-weekly-1.3.dev2331/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fill_holes.py` & `monai-weekly-1.3.dev2331/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fill_holesd.py` & `monai-weekly-1.3.dev2331/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fl_exchange_object.py` & `monai-weekly-1.3.dev2331/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fl_monai_algo.py` & `monai-weekly-1.3.dev2331/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fl_monai_algo_dist.py` & `monai-weekly-1.3.dev2331/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fl_monai_algo_stats.py` & `monai-weekly-1.3.dev2331/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_flatten_sub_keysd.py` & `monai-weekly-1.3.dev2331/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_flexible_unet.py` & `monai-weekly-1.3.dev2331/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_flip.py` & `monai-weekly-1.3.dev2331/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_flipd.py` & `monai-weekly-1.3.dev2331/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_focal_loss.py` & `monai-weekly-1.3.dev2331/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_folder_layout.py` & `monai-weekly-1.3.dev2331/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_foreground_mask.py` & `monai-weekly-1.3.dev2331/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_foreground_maskd.py` & `monai-weekly-1.3.dev2331/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fourier.py` & `monai-weekly-1.3.dev2331/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fpn_block.py` & `monai-weekly-1.3.dev2331/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_from_engine_hovernet.py` & `monai-weekly-1.3.dev2331/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_fullyconnectednet.py` & `monai-weekly-1.3.dev2331/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gaussian.py` & `monai-weekly-1.3.dev2331/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gaussian_filter.py` & `monai-weekly-1.3.dev2331/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gaussian_sharpen.py` & `monai-weekly-1.3.dev2331/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gaussian_sharpend.py` & `monai-weekly-1.3.dev2331/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gaussian_smooth.py` & `monai-weekly-1.3.dev2331/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gaussian_smoothd.py` & `monai-weekly-1.3.dev2331/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generalized_dice_focal_loss.py` & `monai-weekly-1.3.dev2331/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generalized_dice_loss.py` & `monai-weekly-1.3.dev2331/tests/test_generalized_dice_loss.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,53 +44,53 @@
     ],
     [  # shape: (2, 2, 3), (2, 1, 3)
         {"include_background": True, "to_onehot_y": True, "sigmoid": True, "smooth_nr": 1e-4, "smooth_dr": 1e-4},
         {
             "input": torch.tensor([[[-1.0, 0.0, 1.0], [1.0, 0.0, -1.0]], [[0.0, 0.0, 0.0], [0.0, 0.0, 0.0]]]),
             "target": torch.tensor([[[1.0, 0.0, 0.0]], [[1.0, 1.0, 0.0]]]),
         },
-        0.435035,
+        0.469964,
     ],
     [  # shape: (2, 2, 3), (2, 1, 3)
         {"include_background": True, "to_onehot_y": True, "softmax": True, "smooth_nr": 1e-4, "smooth_dr": 1e-4},
         {
             "input": torch.tensor([[[-1.0, 0.0, 1.0], [1.0, 0.0, -1.0]], [[0.0, 0.0, 0.0], [0.0, 0.0, 0.0]]]),
             "target": torch.tensor([[[1.0, 0.0, 0.0]], [[1.0, 1.0, 0.0]]]),
         },
-        0.3837,
+        0.414507,
     ],
     [  # shape: (2, 2, 3), (2, 1, 3)
         {
             "include_background": True,
             "to_onehot_y": True,
             "softmax": True,
             "reduction": "sum",
             "smooth_nr": 1e-4,
             "smooth_dr": 1e-4,
         },
         {
             "input": torch.tensor([[[-1.0, 0.0, 1.0], [1.0, 0.0, -1.0]], [[0.0, 0.0, 0.0], [0.0, 0.0, 0.0]]]),
             "target": torch.tensor([[[1.0, 0.0, 0.0]], [[1.0, 1.0, 0.0]]]),
         },
-        1.5348,
+        0.829015,
     ],
     [  # shape: (2, 2, 3), (2, 1, 3)
         {
             "include_background": True,
             "to_onehot_y": True,
             "softmax": True,
             "reduction": "none",
             "smooth_nr": 1e-4,
             "smooth_dr": 1e-4,
         },
         {
             "input": torch.tensor([[[-1.0, 0.0, 1.0], [1.0, 0.0, -1.0]], [[0.0, 0.0, 0.0], [0.0, 0.0, 0.0]]]),
             "target": torch.tensor([[[1.0, 0.0, 0.0]], [[1.0, 1.0, 0.0]]]),
         },
-        [[[0.210949], [0.295351]], [[0.599976], [0.428522]]],
+        [[[0.273476]], [[0.555539]]],
     ],
     [  # shape: (2, 2, 3), (2, 1, 3)
         {"include_background": False, "to_onehot_y": True, "smooth_nr": 1e-8, "smooth_dr": 1e-8},
         {
             "input": torch.tensor([[[1.0, 1.0, 0.0], [0.0, 0.0, 1.0]], [[1.0, 0.0, 1.0], [0.0, 1.0, 0.0]]]),
             "target": torch.tensor([[[0.0, 0.0, 0.0]], [[0.0, 0.0, 0.0]]]),
         },
@@ -110,15 +110,15 @@
             "smooth_nr": 0,
             "smooth_dr": 0,
         },
         {
             "input": torch.tensor([[[0.0, 10.0, 10.0, 10.0], [10.0, 0.0, 0.0, 0.0]]]),
             "target": torch.tensor([[[1, 1, 0, 0]]]),
         },
-        0.26669,
+        0.250023,
     ],
     [  # shape: (2, 1, 2, 2), (2, 1, 2, 2)
         {"include_background": True, "other_act": torch.tanh, "smooth_nr": 1e-4, "smooth_dr": 1e-4},
         {
             "input": torch.tensor([[[[1.0, -1.0], [-1.0, 1.0]]], [[[1.0, -1.0], [-1.0, 1.0]]]]),
             "target": torch.tensor([[[[1.0, 1.0], [1.0, 1.0]]], [[[1.0, 0.0], [1.0, 0.0]]]]),
         },
@@ -132,15 +132,15 @@
             "smooth_nr": 1e-4,
             "smooth_dr": 1e-4,
         },
         {
             "input": torch.tensor([[[-1.0, 0.0, 1.0], [1.0, 0.0, -1.0]], [[0.0, 0.0, 0.0], [0.0, 0.0, 0.0]]]),
             "target": torch.tensor([[[1.0, 0.0, 0.0]], [[1.0, 1.0, 0.0]]]),
         },
-        -8.55485,
+        -0.097833,
     ],
 ]
 
 
 class TestGeneralizedDiceLoss(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_shape(self, input_param, input_data, expected_val):
```

### Comparing `monai-weekly-1.3.dev2330/tests/test_generalized_wasserstein_dice_loss.py` & `monai-weekly-1.3.dev2331/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_distance_map.py` & `monai-weekly-1.3.dev2331/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_distance_mapd.py` & `monai-weekly-1.3.dev2331/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_instance_border.py` & `monai-weekly-1.3.dev2331/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_instance_borderd.py` & `monai-weekly-1.3.dev2331/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_instance_centroid.py` & `monai-weekly-1.3.dev2331/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_instance_centroidd.py` & `monai-weekly-1.3.dev2331/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_instance_contour.py` & `monai-weekly-1.3.dev2331/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_instance_contourd.py` & `monai-weekly-1.3.dev2331/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_instance_type.py` & `monai-weekly-1.3.dev2331/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_instance_typed.py` & `monai-weekly-1.3.dev2331/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_label_classes_crop_centers.py` & `monai-weekly-1.3.dev2331/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_param_groups.py` & `monai-weekly-1.3.dev2331/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_pos_neg_label_crop_centers.py` & `monai-weekly-1.3.dev2331/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_spatial_bounding_box.py` & `monai-weekly-1.3.dev2331/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_succinct_contour.py` & `monai-weekly-1.3.dev2331/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_succinct_contourd.py` & `monai-weekly-1.3.dev2331/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_watershed_markers.py` & `monai-weekly-1.3.dev2331/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_watershed_markersd.py` & `monai-weekly-1.3.dev2331/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_watershed_mask.py` & `monai-weekly-1.3.dev2331/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generate_watershed_maskd.py` & `monai-weekly-1.3.dev2331/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_generator.py` & `monai-weekly-1.3.dev2331/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_get_equivalent_dtype.py` & `monai-weekly-1.3.dev2331/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_get_extreme_points.py` & `monai-weekly-1.3.dev2331/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_get_layers.py` & `monai-weekly-1.3.dev2331/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_get_package_version.py` & `monai-weekly-1.3.dev2331/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_get_unique_labels.py` & `monai-weekly-1.3.dev2331/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gibbs_noise.py` & `monai-weekly-1.3.dev2331/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gibbs_noised.py` & `monai-weekly-1.3.dev2331/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_giou_loss.py` & `monai-weekly-1.3.dev2331/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_global_mutual_information_loss.py` & `monai-weekly-1.3.dev2331/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_globalnet.py` & `monai-weekly-1.3.dev2331/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_gmm.py` & `monai-weekly-1.3.dev2331/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_grid_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_grid_distortion.py` & `monai-weekly-1.3.dev2331/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_grid_distortiond.py` & `monai-weekly-1.3.dev2331/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_grid_patch.py` & `monai-weekly-1.3.dev2331/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_grid_patchd.py` & `monai-weekly-1.3.dev2331/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_grid_pull.py` & `monai-weekly-1.3.dev2331/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_grid_split.py` & `monai-weekly-1.3.dev2331/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_grid_splitd.py` & `monai-weekly-1.3.dev2331/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_checkpoint_loader.py` & `monai-weekly-1.3.dev2331/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_checkpoint_saver.py` & `monai-weekly-1.3.dev2331/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_classification_saver.py` & `monai-weekly-1.3.dev2331/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_classification_saver_dist.py` & `monai-weekly-1.3.dev2331/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_clearml_image.py` & `monai-weekly-1.3.dev2331/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_clearml_stats.py` & `monai-weekly-1.3.dev2331/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_confusion_matrix.py` & `monai-weekly-1.3.dev2331/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_confusion_matrix_dist.py` & `monai-weekly-1.3.dev2331/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_decollate_batch.py` & `monai-weekly-1.3.dev2331/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_early_stop.py` & `monai-weekly-1.3.dev2331/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_garbage_collector.py` & `monai-weekly-1.3.dev2331/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_hausdorff_distance.py` & `monai-weekly-1.3.dev2331/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_ignite_metric.py` & `monai-weekly-1.3.dev2331/tests/test_handler_ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_logfile.py` & `monai-weekly-1.3.dev2331/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_lr_scheduler.py` & `monai-weekly-1.3.dev2331/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_mean_dice.py` & `monai-weekly-1.3.dev2331/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_mean_iou.py` & `monai-weekly-1.3.dev2331/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_metric_logger.py` & `monai-weekly-1.3.dev2331/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_metrics_reloaded.py` & `monai-weekly-1.3.dev2331/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_metrics_saver.py` & `monai-weekly-1.3.dev2331/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_metrics_saver_dist.py` & `monai-weekly-1.3.dev2331/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_mlflow.py` & `monai-weekly-1.3.dev2331/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_nvtx.py` & `monai-weekly-1.3.dev2331/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_panoptic_quality.py` & `monai-weekly-1.3.dev2331/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_parameter_scheduler.py` & `monai-weekly-1.3.dev2331/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_post_processing.py` & `monai-weekly-1.3.dev2331/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_prob_map_producer.py` & `monai-weekly-1.3.dev2331/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_regression_metrics.py` & `monai-weekly-1.3.dev2331/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_regression_metrics_dist.py` & `monai-weekly-1.3.dev2331/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_rocauc.py` & `monai-weekly-1.3.dev2331/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_rocauc_dist.py` & `monai-weekly-1.3.dev2331/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_smartcache.py` & `monai-weekly-1.3.dev2331/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_stats.py` & `monai-weekly-1.3.dev2331/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_surface_distance.py` & `monai-weekly-1.3.dev2331/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_tb_image.py` & `monai-weekly-1.3.dev2331/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_tb_stats.py` & `monai-weekly-1.3.dev2331/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_handler_validation.py` & `monai-weekly-1.3.dev2331/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hardnegsampler.py` & `monai-weekly-1.3.dev2331/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hashing.py` & `monai-weekly-1.3.dev2331/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hausdorff_distance.py` & `monai-weekly-1.3.dev2331/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_header_correct.py` & `monai-weekly-1.3.dev2331/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_highresnet.py` & `monai-weekly-1.3.dev2331/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hilbert_transform.py` & `monai-weekly-1.3.dev2331/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_histogram_normalize.py` & `monai-weekly-1.3.dev2331/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_histogram_normalized.py` & `monai-weekly-1.3.dev2331/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hovernet.py` & `monai-weekly-1.3.dev2331/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hovernet_instance_map_post_processing.py` & `monai-weekly-1.3.dev2331/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hovernet_instance_map_post_processingd.py` & `monai-weekly-1.3.dev2331/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hovernet_loss.py` & `monai-weekly-1.3.dev2331/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hovernet_nuclear_type_post_processing.py` & `monai-weekly-1.3.dev2331/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai-weekly-1.3.dev2331/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_identity.py` & `monai-weekly-1.3.dev2331/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_identityd.py` & `monai-weekly-1.3.dev2331/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_image_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_image_filter.py` & `monai-weekly-1.3.dev2331/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_image_rw.py` & `monai-weekly-1.3.dev2331/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_img2tensorboard.py` & `monai-weekly-1.3.dev2331/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_init_reader.py` & `monai-weekly-1.3.dev2331/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_autorunner.py` & `monai-weekly-1.3.dev2331/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_bundle_run.py` & `monai-weekly-1.3.dev2331/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_classification_2d.py` & `monai-weekly-1.3.dev2331/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_determinism.py` & `monai-weekly-1.3.dev2331/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_fast_train.py` & `monai-weekly-1.3.dev2331/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_gpu_customization.py` & `monai-weekly-1.3.dev2331/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_lazy_samples.py` & `monai-weekly-1.3.dev2331/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_nnunetv2_runner.py` & `monai-weekly-1.3.dev2331/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_segmentation_3d.py` & `monai-weekly-1.3.dev2331/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_sliding_window.py` & `monai-weekly-1.3.dev2331/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_stn.py` & `monai-weekly-1.3.dev2331/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_unet_2d.py` & `monai-weekly-1.3.dev2331/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_workers.py` & `monai-weekly-1.3.dev2331/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_workflows.py` & `monai-weekly-1.3.dev2331/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_integration_workflows_gan.py` & `monai-weekly-1.3.dev2331/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_intensity_stats.py` & `monai-weekly-1.3.dev2331/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_intensity_statsd.py` & `monai-weekly-1.3.dev2331/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_inverse.py` & `monai-weekly-1.3.dev2331/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_inverse_array.py` & `monai-weekly-1.3.dev2331/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_inverse_collation.py` & `monai-weekly-1.3.dev2331/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_invert.py` & `monai-weekly-1.3.dev2331/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_invertd.py` & `monai-weekly-1.3.dev2331/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_is_supported_format.py` & `monai-weekly-1.3.dev2331/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_iterable_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_itk_torch_bridge.py` & `monai-weekly-1.3.dev2331/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_itk_writer.py` & `monai-weekly-1.3.dev2331/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_k_space_spike_noise.py` & `monai-weekly-1.3.dev2331/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_k_space_spike_noised.py` & `monai-weekly-1.3.dev2331/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_keep_largest_connected_component.py` & `monai-weekly-1.3.dev2331/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_keep_largest_connected_componentd.py` & `monai-weekly-1.3.dev2331/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_kspace_mask.py` & `monai-weekly-1.3.dev2331/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_label_filter.py` & `monai-weekly-1.3.dev2331/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_label_filterd.py` & `monai-weekly-1.3.dev2331/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_label_quality_score.py` & `monai-weekly-1.3.dev2331/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_label_to_contour.py` & `monai-weekly-1.3.dev2331/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_label_to_contourd.py` & `monai-weekly-1.3.dev2331/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_label_to_mask.py` & `monai-weekly-1.3.dev2331/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_label_to_maskd.py` & `monai-weekly-1.3.dev2331/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_lambda.py` & `monai-weekly-1.3.dev2331/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_lambdad.py` & `monai-weekly-1.3.dev2331/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_lesion_froc.py` & `monai-weekly-1.3.dev2331/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_list_data_collate.py` & `monai-weekly-1.3.dev2331/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_list_to_dict.py` & `monai-weekly-1.3.dev2331/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_lltm.py` & `monai-weekly-1.3.dev2331/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_lmdbdataset.py` & `monai-weekly-1.3.dev2331/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_lmdbdataset_dist.py` & `monai-weekly-1.3.dev2331/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_load_decathlon_datalist.py` & `monai-weekly-1.3.dev2331/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_load_image.py` & `monai-weekly-1.3.dev2331/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_load_imaged.py` & `monai-weekly-1.3.dev2331/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_load_spacing_orientation.py` & `monai-weekly-1.3.dev2331/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_loader_semaphore.py` & `monai-weekly-1.3.dev2331/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_local_normalized_cross_correlation_loss.py` & `monai-weekly-1.3.dev2331/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_localnet.py` & `monai-weekly-1.3.dev2331/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_localnet_block.py` & `monai-weekly-1.3.dev2331/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_look_up_option.py` & `monai-weekly-1.3.dev2331/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_loss_metric.py` & `monai-weekly-1.3.dev2331/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_lr_finder.py` & `monai-weekly-1.3.dev2331/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_lr_scheduler.py` & `monai-weekly-1.3.dev2331/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_make_nifti.py` & `monai-weekly-1.3.dev2331/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_map_binary_to_indices.py` & `monai-weekly-1.3.dev2331/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_map_classes_to_indices.py` & `monai-weekly-1.3.dev2331/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_map_label_value.py` & `monai-weekly-1.3.dev2331/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_map_label_valued.py` & `monai-weekly-1.3.dev2331/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_map_transform.py` & `monai-weekly-1.3.dev2331/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_mask_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_mask_intensityd.py` & `monai-weekly-1.3.dev2331/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_masked_dice_loss.py` & `monai-weekly-1.3.dev2331/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_masked_loss.py` & `monai-weekly-1.3.dev2331/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_masked_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_matshow3d.py` & `monai-weekly-1.3.dev2331/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_mean_ensemble.py` & `monai-weekly-1.3.dev2331/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_mean_ensembled.py` & `monai-weekly-1.3.dev2331/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_median_filter.py` & `monai-weekly-1.3.dev2331/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_median_smooth.py` & `monai-weekly-1.3.dev2331/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_median_smoothd.py` & `monai-weekly-1.3.dev2331/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_mednistdataset.py` & `monai-weekly-1.3.dev2331/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_meta_affine.py` & `monai-weekly-1.3.dev2331/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_meta_tensor.py` & `monai-weekly-1.3.dev2331/tests/test_meta_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,18 @@
 
     def test_slicing(self):
         x = MetaTensor(np.zeros((10, 3, 4)))
         self.assertEqual(x[slice(4, 1)].shape[0], 0)
         x.is_batch = True
         with self.assertRaises(ValueError):
             x[slice(0, 8)]
+        x = MetaTensor(np.zeros((3, 3, 4)))
+        x.is_batch = True
+        self.assertEqual(x[torch.tensor([True, False, True])].shape, (2, 3, 4))
+        self.assertEqual(x[[True, False, True]].shape, (2, 3, 4))
 
     @parameterized.expand(DTYPES)
     @SkipIfBeforePyTorchVersion((1, 8))
     def test_decollate(self, dtype):
         batch_size = 3
         ims = [self.get_im(dtype=dtype)[0] for _ in range(batch_size * 2)]
         ds = Dataset(ims)
```

### Comparing `monai-weekly-1.3.dev2330/tests/test_metatensor_integration.py` & `monai-weekly-1.3.dev2331/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_metrics_reloaded.py` & `monai-weekly-1.3.dev2331/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_milmodel.py` & `monai-weekly-1.3.dev2331/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_mlp.py` & `monai-weekly-1.3.dev2331/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_mmar_download.py` & `monai-weekly-1.3.dev2331/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_module_list.py` & `monai-weekly-1.3.dev2331/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_monai_env_vars.py` & `monai-weekly-1.3.dev2331/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_monai_utils_misc.py` & `monai-weekly-1.3.dev2331/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_mri_utils.py` & `monai-weekly-1.3.dev2331/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_multi_scale.py` & `monai-weekly-1.3.dev2331/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_net_adapter.py` & `monai-weekly-1.3.dev2331/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_network_consistency.py` & `monai-weekly-1.3.dev2331/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_nifti_endianness.py` & `monai-weekly-1.3.dev2331/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_nifti_header_revise.py` & `monai-weekly-1.3.dev2331/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_nifti_rw.py` & `monai-weekly-1.3.dev2331/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_normalize_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_normalize_intensityd.py` & `monai-weekly-1.3.dev2331/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_npzdictitemdataset.py` & `monai-weekly-1.3.dev2331/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_nrrd_reader.py` & `monai-weekly-1.3.dev2331/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_nuclick_transforms.py` & `monai-weekly-1.3.dev2331/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_numpy_reader.py` & `monai-weekly-1.3.dev2331/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_nvtx_decorator.py` & `monai-weekly-1.3.dev2331/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_nvtx_transform.py` & `monai-weekly-1.3.dev2331/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_occlusion_sensitivity.py` & `monai-weekly-1.3.dev2331/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_one_of.py` & `monai-weekly-1.3.dev2331/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_optim_novograd.py` & `monai-weekly-1.3.dev2331/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_optional_import.py` & `monai-weekly-1.3.dev2331/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ori_ras_lps.py` & `monai-weekly-1.3.dev2331/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_orientation.py` & `monai-weekly-1.3.dev2331/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_orientationd.py` & `monai-weekly-1.3.dev2331/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_p3d_block.py` & `monai-weekly-1.3.dev2331/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_pad_collation.py` & `monai-weekly-1.3.dev2331/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_pad_mode.py` & `monai-weekly-1.3.dev2331/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_parallel_execution.py` & `monai-weekly-1.3.dev2331/tests/test_parallel_execution.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_parallel_execution_dist.py` & `monai-weekly-1.3.dev2331/tests/test_parallel_execution_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_partition_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_partition_dataset_classes.py` & `monai-weekly-1.3.dev2331/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_patch_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_patch_inferer.py` & `monai-weekly-1.3.dev2331/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_patchembedding.py` & `monai-weekly-1.3.dev2331/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_pathology_he_stain.py` & `monai-weekly-1.3.dev2331/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_pathology_he_stain_dict.py` & `monai-weekly-1.3.dev2331/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_pathology_prob_nms.py` & `monai-weekly-1.3.dev2331/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_persistentdataset.py` & `monai-weekly-1.3.dev2331/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_persistentdataset_dist.py` & `monai-weekly-1.3.dev2331/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_phl_cpu.py` & `monai-weekly-1.3.dev2331/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_phl_cuda.py` & `monai-weekly-1.3.dev2331/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_pil_reader.py` & `monai-weekly-1.3.dev2331/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_plot_2d_or_3d_image.py` & `monai-weekly-1.3.dev2331/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_png_rw.py` & `monai-weekly-1.3.dev2331/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_polyval.py` & `monai-weekly-1.3.dev2331/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_prepare_batch_default.py` & `monai-weekly-1.3.dev2331/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_prepare_batch_default_dist.py` & `monai-weekly-1.3.dev2331/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_prepare_batch_extra_input.py` & `monai-weekly-1.3.dev2331/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_prepare_batch_hovernet.py` & `monai-weekly-1.3.dev2331/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_preset_filters.py` & `monai-weekly-1.3.dev2331/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_print_info.py` & `monai-weekly-1.3.dev2331/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_print_transform_backends.py` & `monai-weekly-1.3.dev2331/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_probnms.py` & `monai-weekly-1.3.dev2331/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_probnmsd.py` & `monai-weekly-1.3.dev2331/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_profiling.py` & `monai-weekly-1.3.dev2331/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_pytorch_version_after.py` & `monai-weekly-1.3.dev2331/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_query_memory.py` & `monai-weekly-1.3.dev2331/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_quicknat.py` & `monai-weekly-1.3.dev2331/tests/test_quicknat.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_adjust_contrast.py` & `monai-weekly-1.3.dev2331/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_adjust_contrastd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_affine.py` & `monai-weekly-1.3.dev2331/tests/test_rand_affine.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 
 class TestRandAffine(unittest.TestCase):
     @parameterized.expand(TESTS)
     def test_rand_affine(self, input_param, input_data, expected_val):
         g = RandAffine(**input_param)
         g.set_random_state(123)
         result = g(**input_data)
+        g.rand_affine_grid.affine = torch.eye(4, dtype=torch.float64)  # reset affine
         test_resampler_lazy(g, result, input_param, input_data, seed=123)
         if input_param.get("cache_grid", False):
             self.assertTrue(g._cached_grid is not None)
         assert_allclose(result, expected_val, rtol=_rtol, atol=1e-4, type_test="tensor")
 
     def test_ill_cache(self):
         with self.assertWarns(UserWarning):
```

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_affine_grid.py` & `monai-weekly-1.3.dev2331/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_affined.py` & `monai-weekly-1.3.dev2331/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_axis_flip.py` & `monai-weekly-1.3.dev2331/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_axis_flipd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_bias_field.py` & `monai-weekly-1.3.dev2331/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_bias_fieldd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_coarse_dropout.py` & `monai-weekly-1.3.dev2331/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_coarse_dropoutd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_coarse_shuffle.py` & `monai-weekly-1.3.dev2331/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_coarse_shuffled.py` & `monai-weekly-1.3.dev2331/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_crop_by_label_classes.py` & `monai-weekly-1.3.dev2331/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_crop_by_label_classesd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_crop_by_pos_neg_label.py` & `monai-weekly-1.3.dev2331/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai-weekly-1.3.dev2331/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_cucim_dict_transform.py` & `monai-weekly-1.3.dev2331/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_cucim_transform.py` & `monai-weekly-1.3.dev2331/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_deform_grid.py` & `monai-weekly-1.3.dev2331/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_elastic_2d.py` & `monai-weekly-1.3.dev2331/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_elastic_3d.py` & `monai-weekly-1.3.dev2331/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_elasticd_2d.py` & `monai-weekly-1.3.dev2331/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_elasticd_3d.py` & `monai-weekly-1.3.dev2331/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_flip.py` & `monai-weekly-1.3.dev2331/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_flipd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_gaussian_noise.py` & `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_gaussian_noised.py` & `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_gaussian_sharpen.py` & `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_gaussian_sharpend.py` & `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_gaussian_smooth.py` & `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_gaussian_smoothd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_gibbs_noise.py` & `monai-weekly-1.3.dev2331/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_gibbs_noised.py` & `monai-weekly-1.3.dev2331/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_grid_distortion.py` & `monai-weekly-1.3.dev2331/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_grid_distortiond.py` & `monai-weekly-1.3.dev2331/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_grid_patch.py` & `monai-weekly-1.3.dev2331/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_grid_patchd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_histogram_shift.py` & `monai-weekly-1.3.dev2331/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_histogram_shiftd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_k_space_spike_noise.py` & `monai-weekly-1.3.dev2331/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_k_space_spike_noised.py` & `monai-weekly-1.3.dev2331/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_lambda.py` & `monai-weekly-1.3.dev2331/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_lambdad.py` & `monai-weekly-1.3.dev2331/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_rician_noise.py` & `monai-weekly-1.3.dev2331/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_rician_noised.py` & `monai-weekly-1.3.dev2331/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_rotate.py` & `monai-weekly-1.3.dev2331/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_rotate90.py` & `monai-weekly-1.3.dev2331/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_rotate90d.py` & `monai-weekly-1.3.dev2331/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_rotated.py` & `monai-weekly-1.3.dev2331/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_scale_crop.py` & `monai-weekly-1.3.dev2331/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_scale_cropd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_scale_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity_fixed_meand.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,29 +10,32 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
-from parameterized import parameterized
 
-from monai.transforms import RandScaleIntensity
+from monai.transforms import RandScaleIntensityFixedMeand
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
 
-class TestRandScaleIntensity(NumpyImageTestCase2D):
-    @parameterized.expand([[p] for p in TEST_NDARRAYS])
-    def test_value(self, p):
-        scaler = RandScaleIntensity(factors=0.5, prob=1.0)
-        scaler.set_random_state(seed=0)
-        im = p(self.imt)
-        result = scaler(im)
-        np.random.seed(0)
-        # simulate the randomize() of transform
-        np.random.random()
-        expected = p((self.imt * (1 + np.random.uniform(low=-0.5, high=0.5))).astype(np.float32))
-        assert_allclose(result, p(expected), rtol=1e-7, atol=0, type_test="tensor")
+class TestRandScaleIntensityFixedMeand(NumpyImageTestCase2D):
+    def test_value(self):
+        key = "img"
+        for p in TEST_NDARRAYS:
+            scaler = RandScaleIntensityFixedMeand(keys=[key], factors=0.5, prob=1.0)
+            scaler.set_random_state(seed=0)
+            result = scaler({key: p(self.imt)})
+            np.random.seed(0)
+            # simulate the randomize function of transform
+            np.random.random()
+            im = self.imt
+            mn = im.mean()
+            im = im - mn
+            expected = (1 + np.random.uniform(low=-0.5, high=0.5)) * im
+            expected = expected + mn
+            assert_allclose(result[key], p(expected), type_test="tensor", atol=1e-6)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_scale_intensity_fixed_mean.py` & `monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_scale_intensity_fixed_meand.py` & `monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,32 +10,45 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
+from parameterized import parameterized
 
-from monai.transforms import RandScaleIntensityFixedMeand
+from monai.transforms import RandScaleIntensity
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
 
-class TestRandScaleIntensityFixedMeand(NumpyImageTestCase2D):
-    def test_value(self):
-        key = "img"
-        for p in TEST_NDARRAYS:
-            scaler = RandScaleIntensityFixedMeand(keys=[key], factors=0.5, prob=1.0)
-            scaler.set_random_state(seed=0)
-            result = scaler({key: p(self.imt)})
-            np.random.seed(0)
-            # simulate the randomize function of transform
-            np.random.random()
-            im = self.imt
-            mn = im.mean()
-            im = im - mn
-            expected = (1 + np.random.uniform(low=-0.5, high=0.5)) * im
-            expected = expected + mn
-            assert_allclose(result[key], p(expected), type_test="tensor", atol=1e-6)
+class TestRandScaleIntensity(NumpyImageTestCase2D):
+    @parameterized.expand([[p] for p in TEST_NDARRAYS])
+    def test_value(self, p):
+        scaler = RandScaleIntensity(factors=0.5, prob=1.0)
+        scaler.set_random_state(seed=0)
+        im = p(self.imt)
+        result = scaler(im)
+        np.random.seed(0)
+        # simulate the randomize() of transform
+        np.random.random()
+        expected = p((self.imt * (1 + np.random.uniform(low=-0.5, high=0.5))).astype(np.float32))
+        assert_allclose(result, p(expected), rtol=1e-7, atol=0, type_test="tensor")
+
+    @parameterized.expand([[p] for p in TEST_NDARRAYS])
+    def test_channel_wise(self, p):
+        scaler = RandScaleIntensity(factors=0.5, channel_wise=True, prob=1.0)
+        scaler.set_random_state(seed=0)
+        im = p(self.imt)
+        result = scaler(im)
+        np.random.seed(0)
+        # simulate the randomize() of transform
+        np.random.random()
+        channel_num = self.imt.shape[0]
+        factor = [np.random.uniform(low=-0.5, high=0.5) for _ in range(channel_num)]
+        expected = p(
+            np.stack([np.asarray((self.imt[i]) * (1 + factor[i])) for i in range(channel_num)]).astype(np.float32)
+        )
+        assert_allclose(result, expected, atol=0, rtol=1e-5, type_test=False)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_scale_intensityd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_std_shift_intensityd.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
 
-from monai.transforms import RandScaleIntensityd
+from monai.transforms import RandStdShiftIntensityd
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
 
-class TestRandScaleIntensityd(NumpyImageTestCase2D):
+class TestRandStdShiftIntensityd(NumpyImageTestCase2D):
     def test_value(self):
-        key = "img"
         for p in TEST_NDARRAYS:
-            scaler = RandScaleIntensityd(keys=[key], factors=0.5, prob=1.0)
-            scaler.set_random_state(seed=0)
-            result = scaler({key: p(self.imt)})
+            key = "img"
             np.random.seed(0)
-            # simulate the randomize function of transform
+            # simulate the randomize() of transform
             np.random.random()
-            expected = (self.imt * (1 + np.random.uniform(low=-0.5, high=0.5))).astype(np.float32)
-            assert_allclose(result[key], p(expected), type_test="tensor")
+            factor = np.random.uniform(low=-1.0, high=1.0)
+            expected = self.imt + factor * np.std(self.imt)
+            shifter = RandStdShiftIntensityd(keys=[key], factors=1.0, prob=1.0)
+            shifter.set_random_state(seed=0)
+            result = shifter({key: p(self.imt)})[key]
+            assert_allclose(result, expected, rtol=1e-5, type_test="tensor")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_shift_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_shift_intensityd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_spatial_crop.py` & `monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_spatial_crop_samples.py` & `monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_spatial_crop_samplesd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_spatial_cropd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_std_shift_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_weighted_crop.py` & `monai-weekly-1.3.dev2331/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_weighted_cropd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_zoom.py` & `monai-weekly-1.3.dev2331/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rand_zoomd.py` & `monai-weekly-1.3.dev2331/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_randidentity.py` & `monai-weekly-1.3.dev2331/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_random_order.py` & `monai-weekly-1.3.dev2331/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_randomizable.py` & `monai-weekly-1.3.dev2331/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_randomizable_transform_type.py` & `monai-weekly-1.3.dev2331/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_randtorchvisiond.py` & `monai-weekly-1.3.dev2331/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rankfilter_dist.py` & `monai-weekly-1.3.dev2331/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_recon_net_utils.py` & `monai-weekly-1.3.dev2331/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_reference_based_normalize_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_reference_based_spatial_cropd.py` & `monai-weekly-1.3.dev2331/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_reference_resolver.py` & `monai-weekly-1.3.dev2331/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_reg_loss_integration.py` & `monai-weekly-1.3.dev2331/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_regunet.py` & `monai-weekly-1.3.dev2331/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_regunet_block.py` & `monai-weekly-1.3.dev2331/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_remove_repeated_channel.py` & `monai-weekly-1.3.dev2331/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_remove_repeated_channeld.py` & `monai-weekly-1.3.dev2331/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_remove_small_objects.py` & `monai-weekly-1.3.dev2331/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_repeat_channel.py` & `monai-weekly-1.3.dev2331/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_repeat_channeld.py` & `monai-weekly-1.3.dev2331/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_replace_module.py` & `monai-weekly-1.3.dev2331/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_require_pkg.py` & `monai-weekly-1.3.dev2331/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resample.py` & `monai-weekly-1.3.dev2331/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resample_backends.py` & `monai-weekly-1.3.dev2331/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resample_datalist.py` & `monai-weekly-1.3.dev2331/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resample_to_match.py` & `monai-weekly-1.3.dev2331/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resample_to_matchd.py` & `monai-weekly-1.3.dev2331/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resampler.py` & `monai-weekly-1.3.dev2331/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resize.py` & `monai-weekly-1.3.dev2331/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resize_with_pad_or_crop.py` & `monai-weekly-1.3.dev2331/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resize_with_pad_or_cropd.py` & `monai-weekly-1.3.dev2331/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resized.py` & `monai-weekly-1.3.dev2331/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_resnet.py` & `monai-weekly-1.3.dev2331/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_retinanet.py` & `monai-weekly-1.3.dev2331/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_retinanet_detector.py` & `monai-weekly-1.3.dev2331/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_retinanet_predict_utils.py` & `monai-weekly-1.3.dev2331/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rotate.py` & `monai-weekly-1.3.dev2331/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rotate90.py` & `monai-weekly-1.3.dev2331/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rotate90d.py` & `monai-weekly-1.3.dev2331/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_rotated.py` & `monai-weekly-1.3.dev2331/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_safe_dtype_range.py` & `monai-weekly-1.3.dev2331/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_saliency_inferer.py` & `monai-weekly-1.3.dev2331/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_sample_slices.py` & `monai-weekly-1.3.dev2331/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_sampler_dist.py` & `monai-weekly-1.3.dev2331/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_save_classificationd.py` & `monai-weekly-1.3.dev2331/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_save_image.py` & `monai-weekly-1.3.dev2331/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_save_imaged.py` & `monai-weekly-1.3.dev2331/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_save_state.py` & `monai-weekly-1.3.dev2331/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_savitzky_golay_filter.py` & `monai-weekly-1.3.dev2331/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_savitzky_golay_smooth.py` & `monai-weekly-1.3.dev2331/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_savitzky_golay_smoothd.py` & `monai-weekly-1.3.dev2331/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_scale_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_scale_intensity_fixed_mean.py` & `monai-weekly-1.3.dev2331/tests/test_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_scale_intensity_range.py` & `monai-weekly-1.3.dev2331/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_scale_intensity_range_percentiles.py` & `monai-weekly-1.3.dev2331/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_scale_intensity_range_percentilesd.py` & `monai-weekly-1.3.dev2331/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_scale_intensity_ranged.py` & `monai-weekly-1.3.dev2331/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_scale_intensityd.py` & `monai-weekly-1.3.dev2331/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_se_block.py` & `monai-weekly-1.3.dev2331/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_se_blocks.py` & `monai-weekly-1.3.dev2331/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_seg_loss_integration.py` & `monai-weekly-1.3.dev2331/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_segresnet.py` & `monai-weekly-1.3.dev2331/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_segresnet_block.py` & `monai-weekly-1.3.dev2331/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_segresnet_ds.py` & `monai-weekly-1.3.dev2331/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_select_cross_validation_folds.py` & `monai-weekly-1.3.dev2331/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_select_itemsd.py` & `monai-weekly-1.3.dev2331/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_selfattention.py` & `monai-weekly-1.3.dev2331/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_senet.py` & `monai-weekly-1.3.dev2331/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_separable_filter.py` & `monai-weekly-1.3.dev2331/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_set_determinism.py` & `monai-weekly-1.3.dev2331/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_set_visible_devices.py` & `monai-weekly-1.3.dev2331/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_shift_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_shift_intensityd.py` & `monai-weekly-1.3.dev2331/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_shuffle_buffer.py` & `monai-weekly-1.3.dev2331/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_continuouswavelet.py` & `monai-weekly-1.3.dev2331/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_fillempty.py` & `monai-weekly-1.3.dev2331/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_rand_add_gaussiannoise.py` & `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_rand_add_sine.py` & `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_rand_add_sine_partial.py` & `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_rand_add_squarepulse.py` & `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_rand_add_squarepulse_partial.py` & `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_rand_drop.py` & `monai-weekly-1.3.dev2331/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_rand_scale.py` & `monai-weekly-1.3.dev2331/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_rand_shift.py` & `monai-weekly-1.3.dev2331/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_signal_remove_frequency.py` & `monai-weekly-1.3.dev2331/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_simple_aspp.py` & `monai-weekly-1.3.dev2331/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_simulatedelay.py` & `monai-weekly-1.3.dev2331/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_simulatedelayd.py` & `monai-weekly-1.3.dev2331/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_skip_connection.py` & `monai-weekly-1.3.dev2331/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_slice_inferer.py` & `monai-weekly-1.3.dev2331/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_sliding_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2331/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_sliding_window_hovernet_inference.py` & `monai-weekly-1.3.dev2331/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_sliding_window_inference.py` & `monai-weekly-1.3.dev2331/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_sliding_window_splitter.py` & `monai-weekly-1.3.dev2331/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_smartcachedataset.py` & `monai-weekly-1.3.dev2331/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_smooth_field.py` & `monai-weekly-1.3.dev2331/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_sobel_gradient.py` & `monai-weekly-1.3.dev2331/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_sobel_gradientd.py` & `monai-weekly-1.3.dev2331/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_some_of.py` & `monai-weekly-1.3.dev2331/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spacing.py` & `monai-weekly-1.3.dev2331/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spacingd.py` & `monai-weekly-1.3.dev2331/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spatial_combine_transforms.py` & `monai-weekly-1.3.dev2331/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spatial_crop.py` & `monai-weekly-1.3.dev2331/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spatial_cropd.py` & `monai-weekly-1.3.dev2331/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spatial_pad.py` & `monai-weekly-1.3.dev2331/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spatial_padd.py` & `monai-weekly-1.3.dev2331/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spatial_resample.py` & `monai-weekly-1.3.dev2331/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_spatial_resampled.py` & `monai-weekly-1.3.dev2331/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_split_channel.py` & `monai-weekly-1.3.dev2331/tests/test_split_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_split_channeld.py` & `monai-weekly-1.3.dev2331/tests/test_split_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_splitdim.py` & `monai-weekly-1.3.dev2331/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_splitdimd.py` & `monai-weekly-1.3.dev2331/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_squeezedim.py` & `monai-weekly-1.3.dev2331/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_squeezedimd.py` & `monai-weekly-1.3.dev2331/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ssim_loss.py` & `monai-weekly-1.3.dev2331/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_ssim_metric.py` & `monai-weekly-1.3.dev2331/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_state_cacher.py` & `monai-weekly-1.3.dev2331/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_std_shift_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_std_shift_intensityd.py` & `monai-weekly-1.3.dev2331/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_str2bool.py` & `monai-weekly-1.3.dev2331/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_str2list.py` & `monai-weekly-1.3.dev2331/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_subpixel_upsample.py` & `monai-weekly-1.3.dev2331/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_surface_dice.py` & `monai-weekly-1.3.dev2331/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_surface_distance.py` & `monai-weekly-1.3.dev2331/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_swin_unetr.py` & `monai-weekly-1.3.dev2331/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_synthetic.py` & `monai-weekly-1.3.dev2331/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_tciadataset.py` & `monai-weekly-1.3.dev2331/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_testtimeaugmentation.py` & `monai-weekly-1.3.dev2331/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_text_encoding.py` & `monai-weekly-1.3.dev2331/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_thread_buffer.py` & `monai-weekly-1.3.dev2331/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_threadcontainer.py` & `monai-weekly-1.3.dev2331/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_threshold_intensity.py` & `monai-weekly-1.3.dev2331/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_threshold_intensityd.py` & `monai-weekly-1.3.dev2331/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_timedcall_dist.py` & `monai-weekly-1.3.dev2331/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_contiguous.py` & `monai-weekly-1.3.dev2331/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_cupy.py` & `monai-weekly-1.3.dev2331/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_cupyd.py` & `monai-weekly-1.3.dev2331/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_device.py` & `monai-weekly-1.3.dev2331/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_deviced.py` & `monai-weekly-1.3.dev2331/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_from_meta_tensord.py` & `monai-weekly-1.3.dev2331/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_numpy.py` & `monai-weekly-1.3.dev2331/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_numpyd.py` & `monai-weekly-1.3.dev2331/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_onehot.py` & `monai-weekly-1.3.dev2331/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_pil.py` & `monai-weekly-1.3.dev2331/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_pild.py` & `monai-weekly-1.3.dev2331/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_tensor.py` & `monai-weekly-1.3.dev2331/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_to_tensord.py` & `monai-weekly-1.3.dev2331/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_torchscript_utils.py` & `monai-weekly-1.3.dev2331/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_torchvision.py` & `monai-weekly-1.3.dev2331/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_torchvision_fc_model.py` & `monai-weekly-1.3.dev2331/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_torchvisiond.py` & `monai-weekly-1.3.dev2331/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_traceable_transform.py` & `monai-weekly-1.3.dev2331/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_train_mode.py` & `monai-weekly-1.3.dev2331/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_trainable_bilateral.py` & `monai-weekly-1.3.dev2331/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_trainable_joint_bilateral.py` & `monai-weekly-1.3.dev2331/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_transchex.py` & `monai-weekly-1.3.dev2331/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_transform.py` & `monai-weekly-1.3.dev2331/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_transformerblock.py` & `monai-weekly-1.3.dev2331/tests/test_transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_transpose.py` & `monai-weekly-1.3.dev2331/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_transposed.py` & `monai-weekly-1.3.dev2331/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_tversky_loss.py` & `monai-weekly-1.3.dev2331/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_unet.py` & `monai-weekly-1.3.dev2331/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_unetr.py` & `monai-weekly-1.3.dev2331/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_unetr_block.py` & `monai-weekly-1.3.dev2331/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_unified_focal_loss.py` & `monai-weekly-1.3.dev2331/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_upsample_block.py` & `monai-weekly-1.3.dev2331/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_utils_pytorch_numpy_unification.py` & `monai-weekly-1.3.dev2331/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_varautoencoder.py` & `monai-weekly-1.3.dev2331/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_varnet.py` & `monai-weekly-1.3.dev2331/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_version_leq.py` & `monai-weekly-1.3.dev2331/tests/test_version_leq.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_video_datasets.py` & `monai-weekly-1.3.dev2331/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_vis_cam.py` & `monai-weekly-1.3.dev2331/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_vis_gradbased.py` & `monai-weekly-1.3.dev2331/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_vis_gradcam.py` & `monai-weekly-1.3.dev2331/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_vit.py` & `monai-weekly-1.3.dev2331/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_vitautoenc.py` & `monai-weekly-1.3.dev2331/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_vnet.py` & `monai-weekly-1.3.dev2331/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_vote_ensemble.py` & `monai-weekly-1.3.dev2331/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_vote_ensembled.py` & `monai-weekly-1.3.dev2331/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_warp.py` & `monai-weekly-1.3.dev2331/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_watershed.py` & `monai-weekly-1.3.dev2331/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_watershedd.py` & `monai-weekly-1.3.dev2331/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_weight_init.py` & `monai-weekly-1.3.dev2331/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_weighted_random_sampler_dist.py` & `monai-weekly-1.3.dev2331/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_with_allow_missing_keys.py` & `monai-weekly-1.3.dev2331/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_write_metrics_reports.py` & `monai-weekly-1.3.dev2331/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_wsi_sliding_window_splitter.py` & `monai-weekly-1.3.dev2331/tests/test_wsi_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_wsireader.py` & `monai-weekly-1.3.dev2331/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_zarr_avg_merger.py` & `monai-weekly-1.3.dev2331/tests/test_zarr_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_zipdataset.py` & `monai-weekly-1.3.dev2331/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_zoom.py` & `monai-weekly-1.3.dev2331/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_zoom_affine.py` & `monai-weekly-1.3.dev2331/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/tests/test_zoomd.py` & `monai-weekly-1.3.dev2331/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2330/versioneer.py` & `monai-weekly-1.3.dev2331/versioneer.py`

 * *Files identical despite different names*


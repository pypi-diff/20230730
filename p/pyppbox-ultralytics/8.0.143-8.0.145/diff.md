# Comparing `tmp/pyppbox-ultralytics-8.0.143.tar.gz` & `tmp/pyppbox-ultralytics-8.0.145.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-ultralytics-8.0.143.tar", last modified: Sat Jul 29 13:22:51 2023, max compression
+gzip compressed data, was "pyppbox-ultralytics-8.0.145.tar", last modified: Sun Jul 30 10:05:54 2023, max compression
```

## Comparing `pyppbox-ultralytics-8.0.143.tar` & `pyppbox-ultralytics-8.0.145.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-29 13:22:51.000000 pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-29 13:22:51.000000 pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:22:51.000000 pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-29 13:22:51.000000 pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-29 13:22:51.000000 pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 13:22:51.000000 pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.325494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.333494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.337494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.337494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.337494 pyppbox-ultralytics-8.0.143/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.337494 pyppbox-ultralytics-8.0.143/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    37439 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.337494 pyppbox-ultralytics-8.0.143/ultralytics/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.337494 pyppbox-ultralytics-8.0.143/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46161 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31186 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.337494 pyppbox-ultralytics-8.0.143/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.341494 pyppbox-ultralytics-8.0.143/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.341494 pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.341494 pyppbox-ultralytics-8.0.143/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.341494 pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.341494 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.341494 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.341494 pyppbox-ultralytics-8.0.143/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.341494 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.345494 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.345494 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.345494 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.345494 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.345494 pyppbox-ultralytics-8.0.143/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26091 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.345494 pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.345494 pyppbox-ultralytics-8.0.143/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.349494 pyppbox-ultralytics-8.0.143/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.349494 pyppbox-ultralytics-8.0.143/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    30202 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19491 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    42325 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29013 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    23082 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/yolo/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/yolo/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/yolo/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/yolo/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:22:51.353494 pyppbox-ultralytics-8.0.143/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-29 13:22:39.000000 pyppbox-ultralytics-8.0.143/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.452288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37439 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16521 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46161 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31186 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26091 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    30232 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19491 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42325 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29013 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23082 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/v8/__init__.py
```

### Comparing `pyppbox-ultralytics-8.0.143/LICENSE` & `pyppbox-ultralytics-8.0.145/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/PKG-INFO` & `pyppbox-ultralytics-8.0.145/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox-ultralytics
-Version: 8.0.143
+Version: 8.0.145
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/rathaumons/ultralytics-for-pyppbox
 Author: rathaROG
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-pyppbox/issues
 Project-URL: Funding, https://ultralytics.com
@@ -33,16 +33,16 @@
 Provides-Extra: export
 License-File: LICENSE
 
 [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
 # Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **July 29, 2023**
-* Synced with: v8.0.143 -> [[1a0eb3f]](https://github.com/ultralytics/ultralytics/commit/1a0eb3f0999f4bfb8aad986c635f60eda3fe545f) + ... + [[62a0fb9]](https://github.com/ultralytics/ultralytics/commit/62a0fb986a6f2ebe654594ea2d30f25e2b713a46)
+* Updated: **July 30, 2023**
+* Synced with: v8.0.145 -> [[a02b7e6]](https://github.com/ultralytics/ultralytics/commit/a02b7e6273b53f99536f3cefafc159e05bec2428)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `pyppbox-ultralytics-8.0.143/README.md` & `pyppbox-ultralytics-8.0.145/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
 # Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **July 29, 2023**
-* Synced with: v8.0.143 -> [[1a0eb3f]](https://github.com/ultralytics/ultralytics/commit/1a0eb3f0999f4bfb8aad986c635f60eda3fe545f) + ... + [[62a0fb9]](https://github.com/ultralytics/ultralytics/commit/62a0fb986a6f2ebe654594ea2d30f25e2b713a46)
+* Updated: **July 30, 2023**
+* Synced with: v8.0.145 -> [[a02b7e6]](https://github.com/ultralytics/ultralytics/commit/a02b7e6273b53f99536f3cefafc159e05bec2428)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/PKG-INFO` & `pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox-ultralytics
-Version: 8.0.143
+Version: 8.0.145
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/rathaumons/ultralytics-for-pyppbox
 Author: rathaROG
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-pyppbox/issues
 Project-URL: Funding, https://ultralytics.com
@@ -33,16 +33,16 @@
 Provides-Extra: export
 License-File: LICENSE
 
 [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
 # Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **July 29, 2023**
-* Synced with: v8.0.143 -> [[1a0eb3f]](https://github.com/ultralytics/ultralytics/commit/1a0eb3f0999f4bfb8aad986c635f60eda3fe545f) + ... + [[62a0fb9]](https://github.com/ultralytics/ultralytics/commit/62a0fb986a6f2ebe654594ea2d30f25e2b713a46)
+* Updated: **July 30, 2023**
+* Synced with: v8.0.145 -> [[a02b7e6]](https://github.com/ultralytics/ultralytics/commit/a02b7e6273b53f99536f3cefafc159e05bec2428)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `pyppbox-ultralytics-8.0.143/pyppbox_ultralytics.egg-info/SOURCES.txt` & `pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/requirements.txt` & `pyppbox-ultralytics-8.0.145/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/setup.cfg` & `pyppbox-ultralytics-8.0.145/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/setup.py` & `pyppbox-ultralytics-8.0.145/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/tests/test_cli.py` & `pyppbox-ultralytics-8.0.145/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/tests/test_engine.py` & `pyppbox-ultralytics-8.0.145/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/tests/test_python.py` & `pyppbox-ultralytics-8.0.145/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/__init__.py` & `pyppbox-ultralytics-8.0.145/ultralytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = '8.0.143'
+__version__ = '8.0.145'
 
 from ultralytics.hub import start
 from ultralytics.models import RTDETR, SAM, YOLO
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import SETTINGS as settings
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/assets/bus.jpg` & `pyppbox-ultralytics-8.0.145/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/assets/zidane.jpg` & `pyppbox-ultralytics-8.0.145/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/__init__.py` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/Argoverse.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/ImageNet.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/Objects365.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/SKU-110K.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/VOC.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/VisDrone.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco-pose.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco128-seg.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco128.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco8-pose.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco8-seg.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/coco8.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/datasets/xView.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/default.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v3/yolov3.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v5/yolov5.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v6/yolov6.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/models/v8/yolov8.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/trackers/botsort.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/cfg/trackers/bytetrack.yaml` & `pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/data/annotator.py` & `pyppbox-ultralytics-8.0.145/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/data/augment.py` & `pyppbox-ultralytics-8.0.145/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/data/base.py` & `pyppbox-ultralytics-8.0.145/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/data/build.py` & `pyppbox-ultralytics-8.0.145/ultralytics/data/build.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/data/converter.py` & `pyppbox-ultralytics-8.0.145/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/data/dataset.py` & `pyppbox-ultralytics-8.0.145/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/data/loaders.py` & `pyppbox-ultralytics-8.0.145/ultralytics/data/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     def __next__(self):
         """mss screen capture: get raw pixels from the screen as np array."""
         im0 = np.array(self.sct.grab(self.monitor))[:, :, :3]  # [:, :, :3] BGRA to BGR
         s = f'screen {self.screen} (LTWH): {self.left},{self.top},{self.width},{self.height}: '
 
         self.frame += 1
-        return str(self.screen), im0, None, s  # screen, img, original img, im0s, s
+        return [str(self.screen)], [im0], None, s  # screen, img, vid_cap, string
 
 
 class LoadImages:
     """YOLOv8 image/video dataloader, i.e. `yolo predict source=image.jpg/vid.mp4`."""
 
     def __init__(self, path, imgsz=640, vid_stride=1):
         """Initialize the Dataloader and raise FileNotFoundError if file not found."""
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/data/utils.py` & `pyppbox-ultralytics-8.0.145/ultralytics/data/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
     # Parse yaml
     train, val, test, s = (data.get(x) for x in ('train', 'val', 'test', 'download'))
     if val:
         val = [Path(x).resolve() for x in (val if isinstance(val, list) else [val])]  # val path
         if not all(x.exists() for x in val):
             name = clean_url(dataset)  # dataset name with URL auth stripped
-            m = f"\nDataset '{name}' images not found ⚠️, missing paths %s" % [str(x) for x in val if not x.exists()]
+            m = f"\nDataset '{name}' images not found ⚠️, missing path '{[x for x in val if not x.exists()][0]}'"
             if s and autodownload:
                 LOGGER.warning(m)
             else:
                 m += f"\nNote dataset download directory is '{DATASETS_DIR}'. You can update this in '{SETTINGS_YAML}'"
                 raise FileNotFoundError(m)
             t = time.time()
             if s.startswith('http') and s.endswith('.zip'):  # URL
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/engine/exporter.py` & `pyppbox-ultralytics-8.0.145/ultralytics/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/engine/model.py` & `pyppbox-ultralytics-8.0.145/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/engine/predictor.py` & `pyppbox-ultralytics-8.0.145/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/engine/results.py` & `pyppbox-ultralytics-8.0.145/ultralytics/engine/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         path (str): The path to the image file.
         names (dict): A dictionary of class names.
         boxes (torch.tensor, optional): A 2D tensor of bounding box coordinates for each detection.
         masks (torch.tensor, optional): A 3D tensor of detection masks, where each mask is a binary image.
         probs (torch.tensor, optional): A 1D tensor of probabilities of each class for classification task.
         keypoints (List[List[float]], optional): A list of detected keypoints for each object.
 
-
     Attributes:
         orig_img (numpy.ndarray): The original image as a numpy array.
         orig_shape (tuple): The original image shape in (height, width) format.
         boxes (Boxes, optional): A Boxes object containing the detection bounding boxes.
         masks (Masks, optional): A Masks object containing the detection masks.
         probs (Probs, optional): A Probs object containing probabilities of each class for classification task.
         names (dict): A dictionary of class names.
@@ -168,14 +167,15 @@
             conf=True,
             line_width=None,
             font_size=None,
             font='Arial.ttf',
             pil=False,
             img=None,
             im_gpu=None,
+            kpt_radius=5,
             kpt_line=True,
             labels=True,
             boxes=True,
             masks=True,
             probs=True,
             **kwargs  # deprecated args TODO: remove support in 8.2
     ):
@@ -186,14 +186,15 @@
             conf (bool): Whether to plot the detection confidence score.
             line_width (float, optional): The line width of the bounding boxes. If None, it is scaled to the image size.
             font_size (float, optional): The font size of the text. If None, it is scaled to the image size.
             font (str): The font to use for the text.
             pil (bool): Whether to return the image as a PIL Image.
             img (numpy.ndarray): Plot to another image. if not, plot to original image.
             im_gpu (torch.Tensor): Normalized image in gpu with shape (1, 3, 640, 640), for faster mask plotting.
+            kpt_radius (int, optional): Radius of the drawn keypoints. Default is 5.
             kpt_line (bool): Whether to draw lines connecting keypoints.
             labels (bool): Whether to plot the label of bounding boxes.
             boxes (bool): Whether to plot the bounding boxes.
             masks (bool): Whether to plot the masks.
             probs (bool): Whether to plot classification probability
 
         Returns:
@@ -247,15 +248,15 @@
             text = ',\n'.join(f'{names[j] if names else j} {pred_probs.data[j]:.2f}' for j in pred_probs.top5)
             x = round(self.orig_shape[0] * 0.03)
             annotator.text([x, x], text, txt_color=(255, 255, 255))  # TODO: allow setting colors
 
         # Plot Pose results
         if self.keypoints is not None:
             for k in reversed(self.keypoints.data):
-                annotator.kpts(k, self.orig_shape, kpt_line=kpt_line)
+                annotator.kpts(k, self.orig_shape, radius=kpt_radius, kpt_line=kpt_line)
 
         return annotator.result()
 
     def verbose(self):
         """
         Return log string for each task.
         """
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/engine/trainer.py` & `pyppbox-ultralytics-8.0.145/ultralytics/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/engine/validator.py` & `pyppbox-ultralytics-8.0.145/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/hub/__init__.py` & `pyppbox-ultralytics-8.0.145/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/hub/auth.py` & `pyppbox-ultralytics-8.0.145/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/hub/session.py` & `pyppbox-ultralytics-8.0.145/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/hub/utils.py` & `pyppbox-ultralytics-8.0.145/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/model.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/predict.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/prompt.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/utils.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/fastsam/val.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/nas/model.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/nas/predict.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/nas/val.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/model.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/predict.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/train.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/rtdetr/val.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/amg.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/build.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/model.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.model = build_sam(weights)
 
     def predict(self, source, stream=False, bboxes=None, points=None, labels=None, **kwargs):
         """Predicts and returns segmentation masks for given image or video source."""
         overrides = dict(conf=0.25, task='segment', mode='predict', imgsz=1024)
         kwargs.update(overrides)
         prompts = dict(bboxes=bboxes, points=points, labels=labels)
-        super().predict(source, stream, prompts=prompts, **kwargs)
+        return super().predict(source, stream, prompts=prompts, **kwargs)
 
     def __call__(self, source=None, stream=False, bboxes=None, points=None, labels=None, **kwargs):
         """Calls the 'predict' function with given arguments to perform object detection."""
         return self.predict(source, stream, bboxes, points, labels, **kwargs)
 
     def info(self, detailed=False, verbose=True):
         """
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/decoders.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/encoders.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/sam.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/tiny_encoder.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/modules/transformer.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/sam/predict.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
             pred_bboxes = pred_bboxes[keep]
             pred_scores = pred_scores[keep]
 
         return pred_masks, pred_scores, pred_bboxes
 
     def setup_model(self, model, verbose=True):
         """Set up YOLO model with specified thresholds and device."""
-        device = select_device(self.args.device)
+        device = select_device(self.args.device, verbose=verbose)
         if model is None:
             model = build_sam(self.args.model)
         model.eval()
         self.model = model.to(device)
         self.device = device
         self.mean = torch.tensor([123.675, 116.28, 103.53]).view(-1, 1, 1).to(device)
         self.std = torch.tensor([58.395, 57.12, 57.375]).view(-1, 1, 1).to(device)
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/utils/loss.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/utils/ops.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/classify/predict.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/classify/train.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,19 +131,20 @@
                 #     self.metrics = self.validator(model=f)
                 #     self.metrics.pop('fitness', None)
                 #     self.run_callbacks('on_fit_epoch_end')
         LOGGER.info(f"Results saved to {colorstr('bold', self.save_dir)}")
 
     def plot_training_samples(self, batch, ni):
         """Plots training samples with their annotations."""
-        plot_images(images=batch['img'],
-                    batch_idx=torch.arange(len(batch['img'])),
-                    cls=batch['cls'].squeeze(-1),
-                    fname=self.save_dir / f'train_batch{ni}.jpg',
-                    on_plot=self.on_plot)
+        plot_images(
+            images=batch['img'],
+            batch_idx=torch.arange(len(batch['img'])),
+            cls=batch['cls'].view(-1),  # warning: use .view(), not .squeeze() for Classify models
+            fname=self.save_dir / f'train_batch{ni}.jpg',
+            on_plot=self.on_plot)
 
 
 def train(cfg=DEFAULT_CFG, use_python=False):
     """Train the YOLO classification model."""
     model = cfg.model or 'yolov8n-cls.pt'  # or "resnet18"
     data = cfg.data or 'mnist160'  # or yolo.ClassificationDataset("mnist")
     device = cfg.device if cfg.device is not None else ''
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/classify/val.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/val.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,20 +70,21 @@
     def print_results(self):
         """Prints evaluation metrics for YOLO object detection model."""
         pf = '%22s' + '%11.3g' * len(self.metrics.keys)  # print format
         LOGGER.info(pf % ('all', self.metrics.top1, self.metrics.top5))
 
     def plot_val_samples(self, batch, ni):
         """Plot validation image samples."""
-        plot_images(images=batch['img'],
-                    batch_idx=torch.arange(len(batch['img'])),
-                    cls=batch['cls'].squeeze(-1),
-                    fname=self.save_dir / f'val_batch{ni}_labels.jpg',
-                    names=self.names,
-                    on_plot=self.on_plot)
+        plot_images(
+            images=batch['img'],
+            batch_idx=torch.arange(len(batch['img'])),
+            cls=batch['cls'].view(-1),  # warning: use .view(), not .squeeze() for Classify models
+            fname=self.save_dir / f'val_batch{ni}_labels.jpg',
+            names=self.names,
+            on_plot=self.on_plot)
 
     def plot_predictions(self, batch, preds, ni):
         """Plots predicted bounding boxes on input images and saves the result."""
         plot_images(batch['img'],
                     batch_idx=torch.arange(len(batch['img'])),
                     cls=torch.argmax(preds, dim=1),
                     fname=self.save_dir / f'val_batch{ni}_pred.jpg',
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/detect/predict.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/detect/train.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/detect/val.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/model.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/pose/predict.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/predict.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 from ultralytics.engine.results import Results
 from ultralytics.models.yolo.detect.predict import DetectionPredictor
-from ultralytics.utils import DEFAULT_CFG, ROOT, ops
+from ultralytics.utils import DEFAULT_CFG, LOGGER, ROOT, ops
 
 
 class PosePredictor(DetectionPredictor):
 
     def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
         super().__init__(cfg, overrides, _callbacks)
         self.args.task = 'pose'
+        if isinstance(self.args.device, str) and self.args.device.lower() == 'mps':
+            LOGGER.warning("WARNING ⚠️ Apple MPS known Pose bug. Recommend 'device=cpu' for Pose models. "
+                           'See https://github.com/ultralytics/ultralytics/issues/4031.')
 
     def postprocess(self, preds, img, orig_imgs):
         """Return detection results for a given input image or list of images."""
         preds = ops.non_max_suppression(preds,
                                         self.args.conf,
                                         self.args.iou,
                                         agnostic=self.args.agnostic_nms,
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/pose/train.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 from copy import copy
 
 from ultralytics.models import yolo
 from ultralytics.nn.tasks import PoseModel
-from ultralytics.utils import DEFAULT_CFG
+from ultralytics.utils import DEFAULT_CFG, LOGGER
 from ultralytics.utils.plotting import plot_images, plot_results
 
 
 # BaseTrainer python usage
 class PoseTrainer(yolo.detect.DetectionTrainer):
 
     def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
         """Initialize a PoseTrainer object with specified configurations and overrides."""
         if overrides is None:
             overrides = {}
         overrides['task'] = 'pose'
         super().__init__(cfg, overrides, _callbacks)
 
+        if isinstance(self.args.device, str) and self.args.device.lower() == 'mps':
+            LOGGER.warning("WARNING ⚠️ Apple MPS known Pose bug. Recommend 'device=cpu' for Pose models. "
+                           'See https://github.com/ultralytics/ultralytics/issues/4031.')
+
     def get_model(self, cfg=None, weights=None, verbose=True):
         """Get pose estimation model with specified configuration and weights."""
         model = PoseModel(cfg, ch=3, nc=self.data['nc'], data_kpt_shape=self.data['kpt_shape'], verbose=verbose)
         if weights:
             model.load(weights)
 
         return model
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/pose/val.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/val.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 class PoseValidator(DetectionValidator):
 
     def __init__(self, dataloader=None, save_dir=None, pbar=None, args=None, _callbacks=None):
         """Initialize a 'PoseValidator' object with custom parameters and assigned attributes."""
         super().__init__(dataloader, save_dir, pbar, args, _callbacks)
         self.args.task = 'pose'
         self.metrics = PoseMetrics(save_dir=self.save_dir, on_plot=self.on_plot)
+        if isinstance(self.args.device, str) and self.args.device.lower() == 'mps':
+            LOGGER.warning("WARNING ⚠️ Apple MPS known Pose bug. Recommend 'device=cpu' for Pose models. "
+                           'See https://github.com/ultralytics/ultralytics/issues/4031.')
 
     def preprocess(self, batch):
         """Preprocesses the batch by converting the 'keypoints' data into a float and moving it to the device."""
         batch = super().preprocess(batch)
         batch['keypoints'] = batch['keypoints'].to(self.device).float()
         return batch
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/segment/predict.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/segment/train.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/models/yolo/segment/val.py` & `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/__init__.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/autobackend.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/__init__.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/block.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/conv.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/head.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/transformer.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/modules/utils.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/nn/tasks.py` & `pyppbox-ultralytics-8.0.145/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/trackers/basetrack.py` & `pyppbox-ultralytics-8.0.145/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/trackers/bot_sort.py` & `pyppbox-ultralytics-8.0.145/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/trackers/byte_tracker.py` & `pyppbox-ultralytics-8.0.145/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/trackers/track.py` & `pyppbox-ultralytics-8.0.145/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/trackers/utils/gmc.py` & `pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/trackers/utils/kalman_filter.py` & `pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/trackers/utils/matching.py` & `pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/__init__.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -820,15 +820,15 @@
         version = float(__version__[:3]) + 0.2  # deprecate after 2nd major release
     LOGGER.warning(f"WARNING ⚠️ '{arg}' is deprecated and will be removed in 'ultralytics {version}' in the future. "
                    f"Please use '{new_arg}' instead.")
 
 
 def clean_url(url):
     """Strip auth from URL, i.e. https://url.com/file.txt?auth -> https://url.com/file.txt."""
-    url = str(Path(url)).replace(':/', '://')  # Pathlib turns :// -> :/
+    url = Path(url).as_posix().replace(':/', '://')  # Pathlib turns :// -> :/, as_posix() for Windows
     return urllib.parse.unquote(url).split('?')[0]  # '%2F' to '/', split https://url.com/file.txt?auth
 
 
 def url2file(url):
     """Convert URL to filename, i.e. https://url.com/file.txt?auth -> file.txt."""
     return Path(clean_url(url)).name
```

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/autobatch.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/benchmarks.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/base.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/clearml.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/comet.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/dvc.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/hub.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/mlflow.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/neptune.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/raytune.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/tensorboard.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/callbacks/wb.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/checks.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/dist.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/downloads.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/files.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/instance.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/loss.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/metrics.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/ops.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/patches.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/plotting.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/tal.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/torch_utils.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/utils/tuner.py` & `pyppbox-ultralytics-8.0.145/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/yolo/data/__init__.py` & `pyppbox-ultralytics-8.0.145/ultralytics/yolo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.143/ultralytics/yolo/utils/__init__.py` & `pyppbox-ultralytics-8.0.145/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*


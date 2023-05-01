# Comparing `tmp/ultralytics-8.0.90.tar.gz` & `tmp/ultralytics-8.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.0.90.tar", last modified: Sat Apr 29 18:18:51 2023, max compression
+gzip compressed data, was "ultralytics-8.0.91.tar", last modified: Mon May  1 20:21:39 2023, max compression
```

## Comparing `ultralytics-8.0.90.tar` & `ultralytics-8.0.91.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.539567 ultralytics-8.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-29 18:17:10.000000 ultralytics-8.0.90/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-29 18:17:10.000000 ultralytics-8.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-29 18:17:10.000000 ultralytics-8.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-04-29 18:18:51.539567 ultralytics-8.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-04-29 18:17:10.000000 ultralytics-8.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-04-29 18:17:10.000000 ultralytics-8.0.90/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-29 18:17:10.000000 ultralytics-8.0.90/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-29 18:18:51.539567 ultralytics-8.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-29 18:17:10.000000 ultralytics-8.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.519567 ultralytics-8.0.90/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-29 18:17:10.000000 ultralytics-8.0.90/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-29 18:17:10.000000 ultralytics-8.0.90/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-29 18:17:10.000000 ultralytics-8.0.90/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.519567 ultralytics-8.0.90/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/xView.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.519567 ultralytics-8.0.90/ultralytics/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/autobackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/autoshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/tracker/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/cfg/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/cfg/bytetrack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/tracker/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/trackers/byte_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/tracker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/vit/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/vit/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/autosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/vit/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.535567 ultralytics-8.0.90/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    27960 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.535567 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.535567 ultralytics-8.0.90/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.535567 ultralytics-8.0.90/ultralytics/yolo/v8/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.539567 ultralytics-8.0.90/ultralytics/yolo/v8/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/detect/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.539567 ultralytics-8.0.90/ultralytics/yolo/v8/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.539567 ultralytics-8.0.90/ultralytics/yolo/v8/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-01 20:20:18.000000 ultralytics-8.0.91/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 20:20:18.000000 ultralytics-8.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 20:20:18.000000 ultralytics-8.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-01 20:21:39.531917 ultralytics-8.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-01 20:20:18.000000 ultralytics-8.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-01 20:20:18.000000 ultralytics-8.0.91/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 20:20:18.000000 ultralytics-8.0.91/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-01 20:21:39.531917 ultralytics-8.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-01 20:20:18.000000 ultralytics-8.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.511917 ultralytics-8.0.91/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-01 20:20:18.000000 ultralytics-8.0.91/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-01 20:20:18.000000 ultralytics-8.0.91/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-01 20:20:18.000000 ultralytics-8.0.91/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.511917 ultralytics-8.0.91/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.515917 ultralytics-8.0.91/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.515917 ultralytics-8.0.91/ultralytics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/xView.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.515917 ultralytics-8.0.91/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.507917 ultralytics-8.0.91/ultralytics/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/autobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/autoshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/tracker/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/cfg/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/tracker/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/trackers/byte_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/tracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/vit/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/autosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/vit/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.527917 ultralytics-8.0.91/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.527917 ultralytics-8.0.91/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    27960 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/detect/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.515917 ultralytics-8.0.91/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.0.90/CONTRIBUTING.md` & `ultralytics-8.0.91/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 If you spot a problem with YOLOv8 please submit a Bug Report!
 
 For us to start investigating a possible problem we need to be able to reproduce it ourselves first. We've created a few
 short guidelines below to help users provide what we need in order to get started.
 
 When asking a question, people will be better able to provide help if you provide **code** that they can easily
 understand and use to **reproduce** the problem. This is referred to by community members as creating
-a [minimum reproducible example](https://stackoverflow.com/help/minimal-reproducible-example). Your code that reproduces
+a [minimum reproducible example](https://docs.ultralytics.com/help/minimum_reproducible_example/). Your code that reproduces
 the problem should be:
 
 - ✅ **Minimal** – Use as little code as possible that still produces the same problem
 - ✅ **Complete** – Provide **all** parts someone else needs to reproduce your problem in the question itself
 - ✅ **Reproducible** – Test the code you're about to provide to make sure it reproduces the problem
 
 In addition to the above requirements, for [Ultralytics](https://ultralytics.com/) to provide assistance your code
@@ -102,14 +102,14 @@
   GitHub [main](https://github.com/ultralytics/ultralytics/tree/main) branch, and if necessary `git pull` or `git clone`
   a new copy to ensure your problem has not already been resolved by previous commits.
 - ✅ **Unmodified** – Your problem must be reproducible without any modifications to the codebase in this
   repository. [Ultralytics](https://ultralytics.com/) does not provide support for custom code ⚠️.
 
 If you believe your problem meets all of the above criteria, please close this issue and raise a new one using the 🐛
 **Bug Report** [template](https://github.com/ultralytics/ultralytics/issues/new/choose) and providing
-a [minimum reproducible example](https://stackoverflow.com/help/minimal-reproducible-example) to help us better
+a [minimum reproducible example](https://docs.ultralytics.com/help/minimum_reproducible_example/) to help us better
 understand and diagnose your problem.
 
 ## License
 
 By contributing, you agree that your contributions will be licensed under
 the [AGPL-3.0 license](https://choosealicense.com/licenses/agpl-3.0/)
```

### Comparing `ultralytics-8.0.90/LICENSE` & `ultralytics-8.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/PKG-INFO` & `ultralytics-8.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.90
+Version: 8.0.91
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.90 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.91 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
 Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
```

### Comparing `ultralytics-8.0.90/README.md` & `ultralytics-8.0.91/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/README.zh-CN.md` & `ultralytics-8.0.91/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/requirements.txt` & `ultralytics-8.0.91/requirements.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/setup.cfg` & `ultralytics-8.0.91/setup.cfg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/setup.py` & `ultralytics-8.0.91/setup.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/tests/test_cli.py` & `ultralytics-8.0.91/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/tests/test_engine.py` & `ultralytics-8.0.91/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/tests/test_python.py` & `ultralytics-8.0.91/tests/test_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,7 +232,17 @@
     model = YOLO('yolov8n-cls.pt')
     res = model(SOURCE)
     res[0].plot(probs=False)
     res[0].plot(pil=True)
     res[0].plot()
     res[0] = res[0].cpu().numpy()
     print(res[0].path)
+
+
+def test_track():
+    im = cv2.imread(str(SOURCE))
+    model = YOLO(MODEL)
+    seg_model = YOLO('yolov8n-seg.pt')
+    pose_model = YOLO('yolov8n-pose.pt')
+    model.track(source=im)
+    seg_model.track(source=im)
+    pose_model.track(source=im)
```

### Comparing `ultralytics-8.0.90/ultralytics/assets/bus.jpg` & `ultralytics-8.0.91/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/assets/zidane.jpg` & `ultralytics-8.0.91/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/Argoverse.yaml` & `ultralytics-8.0.91/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/GlobalWheat2020.yaml` & `ultralytics-8.0.91/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/ImageNet.yaml` & `ultralytics-8.0.91/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/Objects365.yaml` & `ultralytics-8.0.91/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/SKU-110K.yaml` & `ultralytics-8.0.91/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/VOC.yaml` & `ultralytics-8.0.91/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/VisDrone.yaml` & `ultralytics-8.0.91/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/coco-pose.yaml` & `ultralytics-8.0.91/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/coco.yaml` & `ultralytics-8.0.91/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/coco128-seg.yaml` & `ultralytics-8.0.91/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/coco128.yaml` & `ultralytics-8.0.91/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/coco8-pose.yaml` & `ultralytics-8.0.91/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/coco8-seg.yaml` & `ultralytics-8.0.91/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/coco8.yaml` & `ultralytics-8.0.91/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/datasets/xView.yaml` & `ultralytics-8.0.91/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/hub/__init__.py` & `ultralytics-8.0.91/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/hub/auth.py` & `ultralytics-8.0.91/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/hub/session.py` & `ultralytics-8.0.91/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/hub/utils.py` & `ultralytics-8.0.91/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics-8.0.91/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics-8.0.91/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v3/yolov3.yaml` & `ultralytics-8.0.91/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v5/yolov5-p6.yaml` & `ultralytics-8.0.91/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v5/yolov5.yaml` & `ultralytics-8.0.91/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v8/yolov8-cls.yaml` & `ultralytics-8.0.91/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v8/yolov8-p2.yaml` & `ultralytics-8.0.91/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v8/yolov8-p6.yaml` & `ultralytics-8.0.91/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.0.91/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v8/yolov8-pose.yaml` & `ultralytics-8.0.91/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v8/yolov8-seg.yaml` & `ultralytics-8.0.91/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/models/v8/yolov8.yaml` & `ultralytics-8.0.91/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/nn/autobackend.py` & `ultralytics-8.0.91/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/nn/autoshape.py` & `ultralytics-8.0.91/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/nn/modules.py` & `ultralytics-8.0.91/ultralytics/nn/modules.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/nn/tasks.py` & `ultralytics-8.0.91/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/tracker/cfg/botsort.yaml` & `ultralytics-8.0.91/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/tracker/cfg/bytetrack.yaml` & `ultralytics-8.0.91/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/tracker/track.py` & `ultralytics-8.0.91/ultralytics/tracker/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         trackers.append(tracker)
     predictor.trackers = trackers
 
 
 def on_predict_postprocess_end(predictor):
     """Postprocess detected boxes and update with object tracking."""
     bs = predictor.dataset.bs
-    im0s = predictor.batch[2]
-    im0s = im0s if isinstance(im0s, list) else [im0s]
+    im0s = predictor.batch[1]
     for i in range(bs):
         det = predictor.results[i].boxes.cpu().numpy()
         if len(det) == 0:
             continue
         tracks = predictor.trackers[i].update(det, im0s[i])
         if len(tracks) == 0:
             continue
```

### Comparing `ultralytics-8.0.90/ultralytics/tracker/trackers/basetrack.py` & `ultralytics-8.0.91/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/tracker/trackers/bot_sort.py` & `ultralytics-8.0.91/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/tracker/trackers/byte_tracker.py` & `ultralytics-8.0.91/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/tracker/utils/gmc.py` & `ultralytics-8.0.91/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/tracker/utils/kalman_filter.py` & `ultralytics-8.0.91/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/tracker/utils/matching.py` & `ultralytics-8.0.91/ultralytics/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/amg.py` & `ultralytics-8.0.91/ultralytics/vit/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/autosize.py` & `ultralytics-8.0.91/ultralytics/vit/sam/autosize.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/build.py` & `ultralytics-8.0.91/ultralytics/vit/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/model.py` & `ultralytics-8.0.91/ultralytics/vit/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/modules/decoders.py` & `ultralytics-8.0.91/ultralytics/vit/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/modules/encoders.py` & `ultralytics-8.0.91/ultralytics/vit/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/modules/mask_generator.py` & `ultralytics-8.0.91/ultralytics/vit/sam/modules/mask_generator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/modules/prompt_predictor.py` & `ultralytics-8.0.91/ultralytics/vit/sam/modules/prompt_predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/modules/sam.py` & `ultralytics-8.0.91/ultralytics/vit/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/modules/transformer.py` & `ultralytics-8.0.91/ultralytics/vit/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/vit/sam/predict.py` & `ultralytics-8.0.91/ultralytics/vit/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/cfg/__init__.py` & `ultralytics-8.0.91/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/cfg/default.yaml` & `ultralytics-8.0.91/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/annotator.py` & `ultralytics-8.0.91/ultralytics/yolo/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/augment.py` & `ultralytics-8.0.91/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/base.py` & `ultralytics-8.0.91/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/build.py` & `ultralytics-8.0.91/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/dataset.py` & `ultralytics-8.0.91/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics-8.0.91/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/data/utils.py` & `ultralytics-8.0.91/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/engine/exporter.py` & `ultralytics-8.0.91/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/engine/model.py` & `ultralytics-8.0.91/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/engine/predictor.py` & `ultralytics-8.0.91/ultralytics/yolo/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/engine/results.py` & `ultralytics-8.0.91/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/engine/trainer.py` & `ultralytics-8.0.91/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/engine/validator.py` & `ultralytics-8.0.91/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/__init__.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/autobatch.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/benchmarks.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/base.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/clearml.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/comet.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/hub.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/mlflow.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/neptune.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/tensorboard.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/wb.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/checks.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/dist.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/downloads.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/files.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/instance.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/loss.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/metrics.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/ops.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/plotting.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/tal.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/torch_utils.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/utils/tuner.py` & `ultralytics-8.0.91/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/classify/predict.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/classify/train.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/classify/val.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/detect/predict.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/detect/train.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/detect/val.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/pose/predict.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/pose/train.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/pose/val.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/segment/predict.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/segment/train.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics/yolo/v8/segment/val.py` & `ultralytics-8.0.91/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.90/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.0.91/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.90
+Version: 8.0.91
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.90 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.91 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
 Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
```

### Comparing `ultralytics-8.0.90/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.0.91/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


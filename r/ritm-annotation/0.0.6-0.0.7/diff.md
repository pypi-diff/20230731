# Comparing `tmp/ritm_annotation-0.0.6.tar.gz` & `tmp/ritm_annotation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ritm_annotation-0.0.6.tar", last modified: Mon Jul 31 01:37:08 2023, max compression
+gzip compressed data, was "ritm_annotation-0.0.7.tar", last modified: Mon Jul 31 21:36:15 2023, max compression
```

## Comparing `ritm_annotation-0.0.6.tar` & `ritm_annotation-0.0.7.tar`

### file list

```diff
@@ -1,143 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.165394 ritm_annotation-0.0.6/ritm_annotation/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.165394 ritm_annotation-0.0.6/ritm_annotation/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.165394 ritm_annotation-0.0.6/ritm_annotation/cli/annotate/
--rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/cli/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/cli/annotate/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/cli/annotate/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/cli/annotate/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.165394 ritm_annotation-0.0.6/ritm_annotation/cli/model_info/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/cli/model_info/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.165394 ritm_annotation-0.0.6/ritm_annotation/cli/train/
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/cli/train/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.165394 ritm_annotation-0.0.6/ritm_annotation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.169394 ritm_annotation-0.0.6/ritm_annotation/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/berkeley.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/coco_lvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/davis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/grabcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/images_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/lvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/openimages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/pascalvoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/datasets/sbd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.169394 ritm_annotation-0.0.6/ritm_annotation/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/engine/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.169394 ritm_annotation-0.0.6/ritm_annotation/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/clicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.169394 ritm_annotation-0.0.6/ritm_annotation/inference/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/predictors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/predictors/brs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/predictors/brs_functors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/predictors/brs_losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.169394 ritm_annotation-0.0.6/ritm_annotation/inference/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/transforms/crops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/transforms/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/transforms/limit_longest_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/transforms/zoom_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.169394 ritm_annotation-0.0.6/ritm_annotation/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/is_deeplab_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/is_hrnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/is_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.169394 ritm_annotation-0.0.6/ritm_annotation/model/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/modeling/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/modeling/deeplab_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/modeling/hrnet_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/modeling/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/modeling/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/modeling/resnetv1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/model/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.169394 ritm_annotation-0.0.6/ritm_annotation/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3109 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3107 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3124 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3161 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3156 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3146 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3141 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3300 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3024 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3020 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2988 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3019 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3004 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/ritm_annotation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/ritm_annotation/utils/cython/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/cython/_get_dist_maps.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/cython/_get_dist_maps.pyxbld
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/cython/dist_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/exp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/ritm_annotation/utils/exp_imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/exp_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/exp_imports/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/ritm_annotation/utils/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.165394 ritm_annotation-0.0.6/ritm_annotation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 01:37:08.000000 ritm_annotation-0.0.6/ritm_annotation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-31 01:37:08.000000 ritm_annotation-0.0.6/ritm_annotation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:37:08.000000 ritm_annotation-0.0.6/ritm_annotation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 01:37:08.000000 ritm_annotation-0.0.6/ritm_annotation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-31 01:37:08.000000 ritm_annotation-0.0.6/ritm_annotation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 01:37:08.000000 ritm_annotation-0.0.6/ritm_annotation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:37:08.173394 ritm_annotation-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 01:36:56.000000 ritm_annotation-0.0.6/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.762313 ritm_annotation-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 21:36:15.762313 ritm_annotation-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/cli/model_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/model_info/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/cli/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.746312 ritm_annotation-0.0.7/ritm_annotation/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/berkeley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/coco_lvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/davis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/grabcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/images_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/lvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/openimages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/pascalvoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/sbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.746312 ritm_annotation-0.0.7/ritm_annotation/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/engine/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.746312 ritm_annotation-0.0.7/ritm_annotation/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/clicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.750312 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs_functors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs_losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.750312 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/crops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/limit_longest_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/zoom_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.750312 ritm_annotation-0.0.7/ritm_annotation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/is_deeplab_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/is_hrnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/is_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.750312 ritm_annotation-0.0.7/ritm_annotation/model/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/deeplab_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/hrnet_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/resnetv1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.754312 ritm_annotation-0.0.7/ritm_annotation/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.754312 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3362 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3290 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3307 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3270 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.754312 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.758312 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3369 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3354 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3363 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3348 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3208 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3179 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3203 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3187 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3430 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/test_exposed_model_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.758312 ritm_annotation-0.0.7/ritm_annotation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.758312 ritm_annotation-0.0.7/ritm_annotation/utils/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/cython/_get_dist_maps.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/cython/_get_dist_maps.pyxbld
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/cython/dist_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/exp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.758312 ritm_annotation-0.0.7/ritm_annotation/utils/exp_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/exp_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/exp_imports/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:36:15.762313 ritm_annotation-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.762313 ritm_annotation-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/tests/test_base.py
```

### Comparing `ritm_annotation-0.0.6/LICENSE` & `ritm_annotation-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/PKG-INFO` & `ritm_annotation-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritm_annotation
-Version: 0.0.6
+Version: 0.0.7
 Summary: Awesome ritm_annotation created by lucasew
 Home-page: https://github.com/lucasew/ritm_annotation/
 Author: lucasew
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `ritm_annotation-0.0.6/README.md` & `ritm_annotation-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/cli/__init__.py` & `ritm_annotation-0.0.7/ritm_annotation/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 import logging
 import sys
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from pathlib import Path
 
 from ritm_annotation.cli.annotate import command as command_annotate
-from ritm_annotation.cli.train import command as command_train
 from ritm_annotation.cli.model_info import command as command_model_info
+from ritm_annotation.cli.train import command as command_train
 
 logger = logging.getLogger(__name__)
 
 
 def add_subcommand(subparsers, name: str, command_fn):
     subparser = subparsers.add_parser(name)
     common_flags(subparser)
@@ -77,12 +77,12 @@
     version = open(str(Path(__file__).parent.parent / "VERSION"), "r").read()
     if args.is_show_version:
         print(version)
         exit(0)
     logger.debug(f"Starting ritm_annotation v{version}")
 
     fn = args.__dict__.get("fn")
-    args.__dict__['fn'] = None
+    args.__dict__["fn"] = None
     if fn is not None:
         fn(args)
     else:
         parser.parse_args([*sys.argv[1:], "--help"])
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/cli/annotate/__init__.py` & `ritm_annotation-0.0.7/ritm_annotation/cli/annotate/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/cli/annotate/canvas.py` & `ritm_annotation-0.0.7/ritm_annotation/cli/annotate/canvas.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/cli/annotate/controller.py` & `ritm_annotation-0.0.7/ritm_annotation/cli/annotate/controller.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/cli/annotate/wrappers.py` & `ritm_annotation-0.0.7/ritm_annotation/cli/annotate/wrappers.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/cli/model_info/__init__.py` & `ritm_annotation-0.0.7/ritm_annotation/cli/model_info/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from pathlib import Path
 import logging
+from pathlib import Path
 
 import torch
 
-from ritm_annotation.inference.utils import find_checkpoint, load_is_model, load_single_is_model
+from ritm_annotation.inference.utils import (
+    find_checkpoint,
+    load_single_is_model,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def command(subparser):
     subparser.description = "Show information about a model pth"
-    subparser.add_argument('model', type=Path)
+    subparser.add_argument("model", type=Path)
 
     def handle(args):
-        logger.debug('Loading model')
-        assert args.model.exists() and args.model.is_file(), "Model must exist and be a file"
+        logger.debug("Loading model")
+        assert (
+            args.model.exists() and args.model.is_file()
+        ), "Model must exist and be a file"
         checkpoint_path = find_checkpoint(args.model.parent, args.model.name)
-        state_dict = torch.load(checkpoint_path, map_location='cpu')
-        model = load_single_is_model(state_dict, torch.device('cpu'))
+        state_dict = torch.load(checkpoint_path, map_location="cpu")
+        model = load_single_is_model(state_dict, torch.device("cpu"))
         print(state_dict)
         print(model)
+
     return handle
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/base.py` & `ritm_annotation-0.0.7/ritm_annotation/data/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,30 @@
         points_sampler=MultiPointSampler(max_num_points=12),
         min_object_area=0,
         keep_background_prob=0.0,
         with_image_info=False,
         samples_scores_path=None,
         samples_scores_gamma=1.0,
         epoch_len=-1,
+        dry_run=False,
     ):
         super(ISDataset, self).__init__()
         self.epoch_len = epoch_len
         self.augmentator = augmentator
         self.min_object_area = min_object_area
         self.keep_background_prob = keep_background_prob
         self.points_sampler = points_sampler
         self.with_image_info = with_image_info
         self.samples_precomputed_scores = self._load_samples_scores(
-            samples_scores_path, samples_scores_gamma
+            samples_scores_path, samples_scores_gamma, dry_run=dry_run
         )
         self.to_tensor = transforms.ToTensor()
 
         self.dataset_samples = None
+        self.dry_run = dry_run
 
     def __getitem__(self, index):
         if self.samples_precomputed_scores is not None:
             index = np.random.choice(
                 self.samples_precomputed_scores["indices"],
                 p=self.samples_precomputed_scores["probs"],
             )
@@ -88,18 +90,19 @@
         else:
             return self.get_samples_number()
 
     def get_samples_number(self):
         return len(self.dataset_samples)
 
     @staticmethod
-    def _load_samples_scores(samples_scores_path, samples_scores_gamma):
-        if samples_scores_path is None:
+    def _load_samples_scores(
+        samples_scores_path, samples_scores_gamma, dry_run=False
+    ):
+        if samples_scores_path is None or (not dry_run):
             return None
-
         with open(samples_scores_path, "rb") as f:
             images_scores = pickle.load(f)
 
         probs = np.array(
             [(1.0 - x[2]) ** samples_scores_gamma for x in images_scores]
         )
         probs /= probs.sum()
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/compose.py` & `ritm_annotation-0.0.7/ritm_annotation/data/compose.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/__init__.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/ade20k.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/ade20k.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 
 from ritm_annotation.data.base import ISDataset
 from ritm_annotation.data.sample import DSample
 from ritm_annotation.utils.misc import get_labels_with_sizes
 
 
 class ADE20kDataset(ISDataset):
-    def __init__(self, dataset_path, split="train", stuff_prob=0.0, **kwargs):
+    def __init__(
+        self,
+        dataset_path,
+        split="train",
+        stuff_prob=0.0,
+        dry_run=False,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
         assert split in {"train", "val"}
 
         self.dataset_path = Path(dataset_path)
         self.dataset_split = split
         self.dataset_split_folder = (
             "training" if split == "train" else "validation"
@@ -25,14 +32,16 @@
 
         anno_path = (
             self.dataset_path / f"{split}-annotations-object-segmentation.pkl"
         )
         if os.path.exists(anno_path):
             with anno_path.open("rb") as f:
                 annotations = pkl.load(f)
+        elif dry_run:
+            annotations = {}
         else:
             raise RuntimeError(f"Can't find annotations at {anno_path}")
         self.annotations = annotations
         self.dataset_samples = list(annotations.keys())
 
     def get_sample(self, index) -> DSample:
         image_id = self.dataset_samples[index]
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/coco.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/coco.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,33 +6,44 @@
 import numpy as np
 
 from ritm_annotation.data.base import ISDataset
 from ritm_annotation.data.sample import DSample
 
 
 class CocoDataset(ISDataset):
-    def __init__(self, dataset_path, split="train", stuff_prob=0.0, **kwargs):
+    def __init__(
+        self,
+        dataset_path,
+        split="train",
+        stuff_prob=0.0,
+        dry_run=False,
+        **kwargs,
+    ):
         super(CocoDataset, self).__init__(**kwargs)
         self.split = split
         self.dataset_path = Path(dataset_path)
         self.stuff_prob = stuff_prob
+        self.dry_run = dry_run
 
         self.load_samples()
 
     def load_samples(self):
         annotation_path = (
             self.dataset_path / "annotations" / f"panoptic_{self.split}.json"
         )
         self.labels_path = (
             self.dataset_path / "annotations" / f"panoptic_{self.split}"
         )
         self.images_path = self.dataset_path / self.split
 
-        with open(annotation_path, "r") as f:
-            annotation = json.load(f)
+        if not self.dry_run:
+            with open(annotation_path, "r") as f:
+                annotation = json.load(f)
+        else:
+            annotation = dict(annotations=[], categories=[])
 
         self.dataset_samples = annotation["annotations"]
 
         self._categories = annotation["categories"]
         self._stuff_labels = [
             x["id"] for x in self._categories if x["isthing"] == 0
         ]
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/coco_lvis.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/coco_lvis.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,30 @@
     def __init__(
         self,
         dataset_path,
         split="train",
         stuff_prob=0.0,
         allow_list_name=None,
         anno_file="hannotation.pickle",
+        dry_run=False,
         **kwargs,
     ):
         super(CocoLvisDataset, self).__init__(**kwargs)
         dataset_path = Path(dataset_path)
         self._split_path = dataset_path / split
         self.split = split
         self._images_path = self._split_path / "images"
         self._masks_path = self._split_path / "masks"
         self.stuff_prob = stuff_prob
 
-        with open(self._split_path / anno_file, "rb") as f:
-            self.dataset_samples = sorted(pickle.load(f).items())
+        if not dry_run:
+            with open(self._split_path / anno_file, "rb") as f:
+                self.dataset_samples = sorted(pickle.load(f).items())
+        else:
+            self.dataset_samples = []
 
         if allow_list_name is not None:
             allow_list_path = self._split_path / allow_list_name
             with open(allow_list_path, "r") as f:
                 allow_images_ids = json.load(f)
             allow_images_ids = set(allow_images_ids)
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/davis.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/davis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/grabcut.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/grabcut.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/images_dir.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/images_dir.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/lvis.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/lvis.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,46 @@
 
 from ritm_annotation.data.base import ISDataset
 from ritm_annotation.data.sample import DSample
 
 
 class LvisDataset(ISDataset):
     def __init__(
-        self, dataset_path, split="train", max_overlap_ratio=0.5, **kwargs
+        self,
+        dataset_path,
+        split="train",
+        max_overlap_ratio=0.5,
+        dry_run=False,
+        **kwargs,
     ):
         super(LvisDataset, self).__init__(**kwargs)
         dataset_path = Path(dataset_path)
         train_categories_path = dataset_path / "train_categories.json"
         self._train_path = dataset_path / "train"
         self._val_path = dataset_path / "val"
 
         self.split = split
         self.max_overlap_ratio = max_overlap_ratio
 
-        with open(dataset_path / split / f"lvis_{self.split}.json", "r") as f:
-            json_annotation = json.loads(f.read())
+        if not dry_run:
+            with open(
+                dataset_path / split / f"lvis_{self.split}.json", "r"
+            ) as f:
+                json_annotation = json.loads(f.read())
+        else:
+            json_annotation = dict(annotations=[], images=[])
 
         self.annotations = defaultdict(list)
         for x in json_annotation["annotations"]:
             self.annotations[x["image_id"]].append(x)
 
         if not train_categories_path.exists():
-            self.generate_train_categories(dataset_path, train_categories_path)
+            self.generate_train_categories(
+                dataset_path, train_categories_path, dry_run=dry_run
+            )
         self.dataset_samples = [
             x
             for x in json_annotation["images"]
             if len(self.annotations[x["id"]]) > 0
         ]
 
     def get_sample(self, index) -> DSample:
@@ -95,13 +107,18 @@
                 np.newaxis, :
             ]
             cv2.fillPoly(mask, contour_points, 1)
 
         return mask
 
     @staticmethod
-    def generate_train_categories(dataset_path, train_categories_path):
-        with open(dataset_path / "train/lvis_train.json", "r") as f:
-            annotation = json.load(f)
+    def generate_train_categories(
+        dataset_path, train_categories_path, dry_run=False
+    ):
+        if not dry_run:
+            with open(dataset_path / "train/lvis_train.json", "r") as f:
+                annotation = json.load(f)
+        else:
+            annotation = dict(categories=[])
 
         with open(train_categories_path, "w") as f:
             json.dump(annotation["categories"], f, indent=1)
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/openimages.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/openimages.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 
 from ritm_annotation.data.base import ISDataset
 from ritm_annotation.data.sample import DSample
 
 
 class OpenImagesDataset(ISDataset):
-    def __init__(self, dataset_path, split="train", **kwargs):
+    def __init__(self, dataset_path, split="train", dry_run=False, **kwargs):
         super().__init__(**kwargs)
         assert split in {"train", "val", "test"}
 
         self.dataset_path = Path(dataset_path)
         self._split_path = self.dataset_path / split
         self._images_path = self._split_path / "images"
         self._masks_path = self._split_path / "masks"
@@ -24,14 +24,16 @@
         clean_anno_path = (
             self._split_path
             / f"{split}-annotations-object-segmentation_clean.pkl"
         )
         if os.path.exists(clean_anno_path):
             with clean_anno_path.open("rb") as f:
                 annotations = pkl.load(f)
+        elif dry_run:
+            annotations = dict(image_id_to_masks=[], dataset_samples=[])
         else:
             raise RuntimeError(f"Can't find annotations at {clean_anno_path}")
         self.image_id_to_masks = annotations["image_id_to_masks"]
         self.dataset_samples = annotations["dataset_samples"]
 
     def get_sample(self, index) -> DSample:
         image_id = self.dataset_samples[index]
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/pascalvoc.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/pascalvoc.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,33 +5,39 @@
 import numpy as np
 
 from ritm_annotation.data.base import ISDataset
 from ritm_annotation.data.sample import DSample
 
 
 class PascalVocDataset(ISDataset):
-    def __init__(self, dataset_path, split="train", **kwargs):
+    def __init__(self, dataset_path, split="train", dry_run=False, **kwargs):
         super().__init__(**kwargs)
         assert split in {"train", "val", "trainval", "test"}
 
         self.dataset_path = Path(dataset_path)
         self._images_path = self.dataset_path / "JPEGImages"
         self._insts_path = self.dataset_path / "SegmentationObject"
         self.dataset_split = split
-
-        if split == "test":
-            with open(
-                self.dataset_path / "ImageSets/Segmentation/test.pickle", "rb"
-            ) as f:
-                self.dataset_samples, self.instance_ids = pkl.load(f)
+        if dry_run:
+            self.dataset_samples = []
         else:
-            with open(
-                self.dataset_path / f"ImageSets/Segmentation/{split}.txt", "r"
-            ) as f:
-                self.dataset_samples = [name.strip() for name in f.readlines()]
+            if split == "test":
+                with open(
+                    self.dataset_path / "ImageSets/Segmentation/test.pickle",
+                    "rb",
+                ) as f:
+                    self.dataset_samples, self.instance_ids = pkl.load(f)
+            else:
+                with open(
+                    self.dataset_path / f"ImageSets/Segmentation/{split}.txt",
+                    "r",
+                ) as f:
+                    self.dataset_samples = [
+                        name.strip() for name in f.readlines()
+                    ]
 
     def get_sample(self, index) -> DSample:
         sample_id = self.dataset_samples[index]
         image_path = str(self._images_path / f"{sample_id}.jpg")
         mask_path = str(self._insts_path / f"{sample_id}.png")
 
         image = cv2.imread(image_path)
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/datasets/sbd.py` & `ritm_annotation-0.0.7/ritm_annotation/data/datasets/sbd.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,36 @@
     get_bbox_from_mask,
     get_labels_with_sizes,
 )
 
 
 class SBDDataset(ISDataset):
     def __init__(
-        self, dataset_path, split="train", buggy_mask_thresh=0.08, **kwargs
+        self,
+        dataset_path,
+        split="train",
+        buggy_mask_thresh=0.08,
+        dry_run=False,
+        **kwargs,
     ):
         super(SBDDataset, self).__init__(**kwargs)
         assert split in {"train", "val"}
 
         self.dataset_path = Path(dataset_path)
         self.dataset_split = split
         self._images_path = self.dataset_path / "img"
         self._insts_path = self.dataset_path / "inst"
         self._buggy_objects = dict()
         self._buggy_mask_thresh = buggy_mask_thresh
 
-        with open(self.dataset_path / f"{split}.txt", "r") as f:
-            self.dataset_samples = [x.strip() for x in f.readlines()]
+        if dry_run:
+            self.dataset_samples = []
+        else:
+            with open(self.dataset_path / f"{split}.txt", "r") as f:
+                self.dataset_samples = [x.strip() for x in f.readlines()]
 
     def get_sample(self, index):
         image_name = self.dataset_samples[index]
         image_path = str(self._images_path / f"{image_name}.jpg")
         inst_info_path = str(self._insts_path / f"{image_name}.mat")
 
         image = cv2.imread(image_path)
@@ -68,27 +76,28 @@
             for obj_id in buggy_image_objects:
                 instances_mask[instances_mask == obj_id] = 0
 
         return instances_mask
 
 
 class SBDEvaluationDataset(ISDataset):
-    def __init__(self, dataset_path, split="val", **kwargs):
+    def __init__(self, dataset_path, split="val", dry_run=False, **kwargs):
         super(SBDEvaluationDataset, self).__init__(**kwargs)
         assert split in {"train", "val"}
 
         self.dataset_path = Path(dataset_path)
         self.dataset_split = split
         self._images_path = self.dataset_path / "img"
         self._insts_path = self.dataset_path / "inst"
-
-        with open(self.dataset_path / f"{split}.txt", "r") as f:
-            self.dataset_samples = [x.strip() for x in f.readlines()]
-
-        self.dataset_samples = self.get_sbd_images_and_ids_list()
+        if dry_run:
+            self.dataset_samples = []
+        else:
+            with open(self.dataset_path / f"{split}.txt", "r") as f:
+                self.dataset_samples = [x.strip() for x in f.readlines()]
+            self.dataset_samples = self.get_sbd_images_and_ids_list()
 
     def get_sample(self, index) -> DSample:
         image_name, instance_id = self.dataset_samples[index]
         image_path = str(self._images_path / f"{image_name}.jpg")
         inst_info_path = str(self._insts_path / f"{image_name}.mat")
 
         image = cv2.imread(image_path)
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/points_sampler.py` & `ritm_annotation-0.0.7/ritm_annotation/data/points_sampler.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/sample.py` & `ritm_annotation-0.0.7/ritm_annotation/data/sample.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/data/transforms.py` & `ritm_annotation-0.0.7/ritm_annotation/data/transforms.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/engine/optimizer.py` & `ritm_annotation-0.0.7/ritm_annotation/engine/optimizer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/engine/trainer.py` & `ritm_annotation-0.0.7/ritm_annotation/engine/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
+import pprint
 import random
 from collections import defaultdict
 from copy import deepcopy
-import pprint
 
 import cv2
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
@@ -44,15 +44,17 @@
         lr_scheduler=None,
         metrics=None,
         additional_val_metrics=None,
         net_inputs=("images", "points"),
         max_num_next_clicks=0,
         click_models=None,
         prev_mask_drop_prob=0.0,
+        dry_run=False,
     ):
+        self._ran_before_needed = False
         self.cfg = cfg
         self.model_cfg = model_cfg
         self.max_interactive_points = max_interactive_points
         self.loss_cfg = loss_cfg
         self.val_loss_cfg = deepcopy(loss_cfg)
         self.tb_dump_period = tb_dump_period
         self.net_inputs = net_inputs
@@ -88,34 +90,36 @@
         )
 
         self.train_data = DataLoader(
             trainset,
             cfg.batch_size,
             sampler=get_sampler(
                 trainset, shuffle=True, distributed=cfg.distributed
-            ),
+            )
+            if not dry_run
+            else None,
             drop_last=True,
             pin_memory=True,
             num_workers=cfg.workers,
-            persistent_workers=True
+            persistent_workers=cfg.workers > 0,
         )
 
         self.val_data = DataLoader(
             valset,
             cfg.val_batch_size,
             sampler=get_sampler(
                 valset, shuffle=False, distributed=cfg.distributed
-            ),
+            )
+            if not dry_run
+            else None,
             drop_last=True,
             pin_memory=True,
             num_workers=cfg.workers,
-            persistent_workers=True
+            persistent_workers=cfg.workers > 0,
         )
-        logger.debug(f'First train batch: {repr(next(iter(self.train_data)))}')
-        logger.debug(f'First evaluation batch: {repr(next(iter(self.val_data)))}')
 
         self.optim = get_optimizer(model, optimizer, optimizer_params)
         model = self._load_weights(model)
 
         if cfg.multi_gpu:
             model = get_dp_wrapper(cfg.distributed)(
                 model, device_ids=cfg.gpu_ids, output_device=cfg.gpu_ids[0]
@@ -142,26 +146,37 @@
                 for param in click_model.parameters():
                     param.requires_grad = False
                 click_model.to(self.device)
                 click_model.eval()
         logger.info("Run experiment with config:")
         logger.info(pprint.pformat(cfg, indent=4))
 
+    def _before_needed_hook(self):
+        if self._ran_before_needed:
+            return
+        self._ran_before_needed = True
+        logger.debug(f"First train batch: {repr(next(iter(self.train_data)))}")
+        logger.debug(
+            f"First evaluation batch: {repr(next(iter(self.val_data)))}"
+        )
+
     def run(self, num_epochs, start_epoch=None, validation=True):
+        self._before_needed_hook()
         if start_epoch is None:
             start_epoch = self.cfg.start_epoch
 
         logger.info(f"Starting Epoch: {start_epoch}")
         logger.info(f"Total Epochs: {num_epochs}")
         for epoch in range(start_epoch, num_epochs):
             self.training(epoch)
             if validation:
                 self.validation(epoch)
 
     def training(self, epoch):
+        self._before_needed_hook()
         if self.sw is None and self.is_master:
             self.sw = SummaryWriterAvg(
                 log_dir=str(self.cfg.LOGS_PATH),
                 flush_secs=10,
                 dump_period=self.tb_dump_period,
             )
 
@@ -279,14 +294,15 @@
                     multi_gpu=self.cfg.multi_gpu,
                 )
 
         if hasattr(self, "lr_scheduler"):
             self.lr_scheduler.step()
 
     def validation(self, epoch):
+        self._before_needed_hook()
         if self.sw is None and self.is_master:
             self.sw = SummaryWriterAvg(
                 log_dir=str(self.cfg.LOGS_PATH),
                 flush_secs=10,
                 dump_period=self.tb_dump_period,
             )
 
@@ -347,14 +363,15 @@
                     tag=f"{log_prefix}Metrics/{metric.name}",
                     value=metric.get_epoch_value(),
                     global_step=epoch,
                     disable_avg=True,
                 )
 
     def batch_forward(self, batch_data, validation=False):
+        self._before_needed_hook()
         metrics = self.val_metrics if validation else self.train_metrics
         losses_logging = dict()
 
         with torch.set_grad_enabled(not validation):
             batch_data = {k: v.to(self.device) for k, v in batch_data.items()}
             image, gt_mask, points = (
                 batch_data["images"],
@@ -533,18 +550,18 @@
                 self.cfg.weights = None
             else:
                 raise RuntimeError(
                     f"=> no checkpoint found at '{self.cfg.weights}'"
                 )
         elif self.cfg.resume_exp is not None:
             checkpoint_glob = f"{self.cfg.resume_prefix}*.pth"
-            checkpoints = list(
-                self.cfg.CHECKPOINTS_PATH.glob(checkpoint_glob)
-            )
-            assert len(checkpoints) == 1, f"'{self.cfg.CHECKPOINTS_PATH}/{checkpoint_glob}' didn't match anything"
+            checkpoints = list(self.cfg.CHECKPOINTS_PATH.glob(checkpoint_glob))
+            assert (
+                len(checkpoints) == 1
+            ), f"'{self.cfg.CHECKPOINTS_PATH}/{checkpoint_glob}' didn't match anything"  # noqa: E501
 
             checkpoint_path = checkpoints[0]
             load_weights(net, str(checkpoint_path))
         return net
 
     @property
     def is_master(self):
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/clicker.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/clicker.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/evaluation.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/evaluation.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/predictors/__init__.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/predictors/base.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/predictors/brs.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/predictors/brs_functors.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs_functors.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/predictors/brs_losses.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs_losses.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/transforms/base.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/transforms/crops.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/crops.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/transforms/flip.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/flip.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/transforms/limit_longest_side.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/limit_longest_side.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/transforms/zoom_in.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/zoom_in.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/inference/utils.py` & `ritm_annotation-0.0.7/ritm_annotation/inference/utils.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/initializer.py` & `ritm_annotation-0.0.7/ritm_annotation/model/initializer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/is_deeplab_model.py` & `ritm_annotation-0.0.7/ritm_annotation/model/is_deeplab_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/is_hrnet_model.py` & `ritm_annotation-0.0.7/ritm_annotation/model/is_hrnet_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/is_model.py` & `ritm_annotation-0.0.7/ritm_annotation/model/is_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/losses.py` & `ritm_annotation-0.0.7/ritm_annotation/model/losses.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/metrics.py` & `ritm_annotation-0.0.7/ritm_annotation/model/metrics.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/modeling/basic_blocks.py` & `ritm_annotation-0.0.7/ritm_annotation/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/modeling/deeplab_v3.py` & `ritm_annotation-0.0.7/ritm_annotation/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/modeling/hrnet_ocr.py` & `ritm_annotation-0.0.7/ritm_annotation/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/modeling/ocr.py` & `ritm_annotation-0.0.7/ritm_annotation/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/modeling/resnet.py` & `ritm_annotation-0.0.7/ritm_annotation/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/modeling/resnetv1b.py` & `ritm_annotation-0.0.7/ritm_annotation/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/model/ops.py` & `ritm_annotation-0.0.7/ritm_annotation/model/ops.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py` & `ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,123 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
+    model_cfg.default_num_epochs = 160
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = SigmoidBinaryCrossEntropyLoss()
+    loss_cfg.instance_loss = SoftIoU()
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = CocoLvisDataset(
         cfg.LVIS_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
         keep_background_prob=0.0,
         points_sampler=points_sampler,
         epoch_len=30000,
-        stuff_prob=0.30
+        stuff_prob=0.30,
+        dry_run=dry_run,
     )
 
     valset = CocoLvisDataset(
         cfg.LVIS_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=80,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[140, 155], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=160)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py` & `ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,125 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
+from ritm_annotation.utils.misc import load_module
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 160
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = FocalLoss(alpha=0.5, gamma=2)
+    loss_cfg.instance_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = CocoLvisDataset(
         cfg.LVIS_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
         keep_background_prob=0.0,
         points_sampler=points_sampler,
         epoch_len=30000,
-        stuff_prob=0.30
+        stuff_prob=0.30,
+        dry_run=dry_run,
     )
 
     valset = CocoLvisDataset(
         cfg.LVIS_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=80,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[140, 155], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=160)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+    )
+    return trainer
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,124 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 230
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = CocoLvisDataset(
         cfg.LVIS_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
+        min_object_area=1000,
+        keep_background_prob=0.05,
         points_sampler=points_sampler,
         epoch_len=30000,
-        stuff_prob=0.30
+        stuff_prob=0.30,
+        dry_run=dry_run,
     )
 
     valset = CocoLvisDataset(
         cfg.LVIS_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
-        min_object_area=80,
+        min_object_area=1000,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[140, 155], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=160)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=[(0, 5), (200, 1)],
+        image_dump_interval=3000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py` & `ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,123 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
+    model_cfg.default_num_epochs = 160
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = SoftIoU()
+    loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = CocoLvisDataset(
         cfg.LVIS_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
         keep_background_prob=0.0,
         points_sampler=points_sampler,
         epoch_len=30000,
-        stuff_prob=0.30
+        stuff_prob=0.30,
+        dry_run=dry_run,
     )
 
     valset = CocoLvisDataset(
         cfg.LVIS_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=80,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[140, 155], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=160)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,94 +1,127 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'cocolvis_hrnet18'
+MODEL_NAME = "cocolvis_hrnet18s"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 230
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5,
-                       with_prev_mask=True)
+    model = HRNetModel(
+        width=18,
+        ocr_width=48,
+        small=True,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+        with_prev_mask=True,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18_SMALL
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
-    cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
+def get_trainer(model, cfg, model_cfg, dry_run=False):
+    cfg.batch_size = 32 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.80,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.80,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = CocoLvisDataset(
         cfg.LVIS_v1_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
         epoch_len=30000,
-        stuff_prob=0.30
+        stuff_prob=0.30,
+        dry_run=dry_run,
     )
 
     valset = CocoLvisDataset(
         cfg.LVIS_v1_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[200, 220], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=[(0, 5), (200, 1)],
-                        image_dump_interval=3000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points,
-                        max_num_next_clicks=3)
-    trainer.run(num_epochs=230)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=[(0, 5), (200, 1)],
+        image_dump_interval=3000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        max_num_next_clicks=3,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py` & `ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,97 +1,123 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'sbd_hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5, with_prev_mask=True)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
+    model_cfg.default_num_epochs = 160
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
+    loss_cfg.instance_loss = FocalLoss(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.25)),
-        Flip(),
-        RandomRotate90(),
-        ShiftScaleRotate(shift_limit=0.03, scale_limit=0,
-                         rotate_limit=(-3, 3), border_mode=0, p=0.75),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.25)),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.80,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = SBDDataset(
-        cfg.SBD_PATH,
-        split='train',
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = CocoLvisDataset(
+        cfg.LVIS_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
-        keep_background_prob=0.01,
+        keep_background_prob=0.0,
         points_sampler=points_sampler,
-        samples_scores_path='./assets/sbd_samples_weights.pkl',
-        samples_scores_gamma=1.25
+        epoch_len=30000,
+        stuff_prob=0.30,
+        dry_run=dry_run,
     )
 
-    valset = SBDDataset(
-        cfg.SBD_PATH,
-        split='val',
+    valset = CocoLvisDataset(
+        cfg.LVIS_PATH,
+        split="val",
         augmentator=val_augmentator,
         min_object_area=80,
         points_sampler=points_sampler,
-        epoch_len=500
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[200, 215], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=[(0, 5), (100, 1)],
-                        image_dump_interval=3000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points,
-                        max_num_next_clicks=3)
-    trainer.run(num_epochs=220)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,119 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'cocolvis_hrnet18s'
+MODEL_NAME = "resnet34"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 120
 
-    model = HRNetModel(width=18, ocr_width=48, small=True, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5,
-                       with_prev_mask=True)
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18_SMALL)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
-    cfg.batch_size = 32 if cfg.batch_size < 1 else cfg.batch_size
+def get_trainer(model, cfg, model_cfg, dry_run=False):
+    cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
-    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
-    loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.80,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = CocoLvisDataset(
-        cfg.LVIS_v1_PATH,
-        split='train',
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = SBDDataset(
+        cfg.SBD_PATH,
+        split="train",
         augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
+        min_object_area=80,
+        keep_background_prob=0.0,
         points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30
+        samples_scores_path="./assets/sbd_samples_weights.pkl",
+        samples_scores_gamma=1.25,
+        dry_run=dry_run,
     )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_v1_PATH,
-        split='val',
+    valset = SBDDataset(
+        cfg.SBD_PATH,
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
         points_sampler=points_sampler,
-        epoch_len=2000
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[200, 220], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=[(0, 5), (200, 1)],
-                        image_dump_interval=3000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points,
-                        max_num_next_clicks=3)
-    trainer.run(num_epochs=230)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,126 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'cocolvis_hrnet32'
+MODEL_NAME = "cocolvis_hrnet32"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 230
 
-    model = HRNetModel(width=32, ocr_width=128, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5, with_prev_mask=True)
+    model = HRNetModel(
+        width=32,
+        ocr_width=128,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+        with_prev_mask=True,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W32)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W32
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 32 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.80,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.80,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = CocoLvisDataset(
         cfg.LVIS_v1_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
         epoch_len=30000,
-        stuff_prob=0.30
+        stuff_prob=0.30,
+        dry_run=dry_run,
     )
 
     valset = CocoLvisDataset(
         cfg.LVIS_v1_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[200, 220], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=[(0, 5), (200, 1)],
-                        image_dump_interval=3000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points,
-                        max_num_next_clicks=3)
-    trainer.run(num_epochs=230)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=[(0, 5), (200, 1)],
+        image_dump_interval=3000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        max_num_next_clicks=3,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,93 +1,121 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "resnet34"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 120
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
-    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
-    loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.80,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = ADE20kDataset(
         cfg.ADE20K_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
         stuff_prob=0.30,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=30000
+        epoch_len=30000,
+        dry_run=dry_run,
     )
 
     valset = ADE20kDataset(
         cfg.ADE20K_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=80,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[100, 115], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=120)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,120 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "resnet34"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights()
 
+    model_cfg.default_num_epochs = 140
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
-    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
-    loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = CocoDataset(
         cfg.COCO_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
         stuff_prob=0.30,
-        epoch_len=30000
+        epoch_len=30000,
+        dry_run=dry_run,
     )
 
     valset = CocoDataset(
         cfg.COCO_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[120, 135], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=140)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,124 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 140
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split='train',
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = OpenImagesDataset(
+        cfg.OPENIMAGES_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
         epoch_len=30000,
-        stuff_prob=0.30
+        dry_run=dry_run,
     )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split='val',
+    valset = OpenImagesDataset(
+        cfg.OPENIMAGES_PATH,
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
+        keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[200, 220], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=[(0, 5), (200, 1)],
-                        image_dump_interval=3000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=230)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,123 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 160
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
     trainset = LvisDataset(
         cfg.LVIS_PATH,
-        split='train',
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=30000
+        epoch_len=30000,
+        dry_run=dry_run,
     )
 
     valset = LvisDataset(
         cfg.LVIS_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[140, 155], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=160)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,119 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "resnet34"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 160
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
-    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
-    loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = OpenImagesDataset(
-        cfg.OPENIMAGES_PATH,
-        split='train',
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = LvisDataset(
+        cfg.LVIS_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=30000
+        epoch_len=30000,
+        dry_run=dry_run,
     )
 
-    valset = OpenImagesDataset(
-        cfg.OPENIMAGES_PATH,
-        split='val',
+    valset = LvisDataset(
+        cfg.LVIS_PATH,
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
-        keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[120, 135], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=140)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,125 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 120
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.80,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = SBDDataset(
-        cfg.SBD_PATH,
-        split='train',
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.80,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = ADE20kDataset(
+        cfg.ADE20K_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
-        keep_background_prob=0.0,
+        stuff_prob=0.30,
+        keep_background_prob=0.05,
         points_sampler=points_sampler,
-        samples_scores_path='./assets/sbd_samples_weights.pkl',
-        samples_scores_gamma=1.25
+        epoch_len=30000,
+        dry_run=dry_run,
     )
 
-    valset = SBDDataset(
-        cfg.SBD_PATH,
-        split='val',
+    valset = ADE20kDataset(
+        cfg.ADE20K_PATH,
+        split="val",
         augmentator=val_augmentator,
-        min_object_area=1000,
+        min_object_area=80,
+        keep_background_prob=0.05,
         points_sampler=points_sampler,
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[100, 115], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=120)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,123 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'hrnet18'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 120
 
-    model = HRNetModel(width=18, ocr_width=64, with_aux_output=True, use_leaky_relu=True,
-                       use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights(cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18)
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.80,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
 
-    trainset = ComposeDataset(
+    val_augmentator = Compose(
         [
-            PascalVocDataset(cfg.PASCALVOC_PATH, split='train'),
-            SBDDataset(
-                cfg.SBD_PATH,
-                split='train',
-                samples_scores_path='./assets/sbd_samples_weights.pkl',
-                samples_scores_gamma=1.25
-            )
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
         ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.80,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = SBDDataset(
+        cfg.SBD_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
         keep_background_prob=0.0,
-        points_sampler=points_sampler
+        points_sampler=points_sampler,
+        samples_scores_path="./assets/sbd_samples_weights.pkl",
+        samples_scores_gamma=1.25,
+        dry_run=dry_run,
     )
 
     valset = SBDDataset(
         cfg.SBD_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
         points_sampler=points_sampler,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[100, 115], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=120)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,120 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'resnet34'
+MODEL_NAME = "resnet34"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 160
 
-    model = DeeplabModel(backbone='resnet34', deeplab_ch=128, aspp_dropout=0.20, use_leaky_relu=True,
-                         use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights()
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = ADE20kDataset(
-        cfg.ADE20K_PATH,
-        split='train',
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = CocoLvisDataset(
+        cfg.LVIS_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
-        stuff_prob=0.30,
-        keep_background_prob=0.05,
+        keep_background_prob=0.0,
         points_sampler=points_sampler,
-        epoch_len=30000
+        epoch_len=30000,
+        stuff_prob=0.30,
+        dry_run=dry_run,
     )
 
-    valset = ADE20kDataset(
-        cfg.ADE20K_PATH,
-        split='val',
+    valset = CocoLvisDataset(
+        cfg.LVIS_PATH,
+        split="val",
         augmentator=val_augmentator,
         min_object_area=80,
-        keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[100, 115], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=120)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py` & `ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,126 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'resnet34'
+MODEL_NAME = "cocolvis_hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 230
 
-    model = DeeplabModel(backbone='resnet34', deeplab_ch=128, aspp_dropout=0.20, use_leaky_relu=True,
-                         use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+        with_prev_mask=True,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights()
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
+    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
+    loss_cfg.instance_aux_loss_weight = 0.4
+
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = CocoDataset(
-        cfg.COCO_PATH,
-        split='train',
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.80,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = CocoLvisDataset(
+        cfg.LVIS_v1_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
+        epoch_len=30000,
         stuff_prob=0.30,
-        epoch_len=30000
+        dry_run=dry_run,
     )
 
-    valset = CocoDataset(
-        cfg.COCO_PATH,
-        split='val',
+    valset = CocoLvisDataset(
+        cfg.LVIS_v1_PATH,
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
-        keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[120, 135], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=140)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=[(0, 5), (200, 1)],
+        image_dump_interval=3000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        max_num_next_clicks=3,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,126 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'resnet34'
+MODEL_NAME = "resnet34"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 120
 
-    model = DeeplabModel(backbone='resnet34', deeplab_ch=128, aspp_dropout=0.20, use_leaky_relu=True,
-                         use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
+        use_leaky_relu=True,  # noqa: E501
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights()
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split='train',
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,  # noqa:E501
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = ComposeDataset(
+        [
+            PascalVocDataset(
+                cfg.PASCALVOC_PATH, split="train", dry_run=dry_run
+            ),
+            SBDDataset(
+                cfg.SBD_PATH,
+                split="train",
+                samples_scores_path="./assets/sbd_samples_weights.pkl",
+                samples_scores_gamma=1.25,
+                dry_run=dry_run,
+            ),
+        ],
         augmentator=train_augmentator,
         min_object_area=80,
         keep_background_prob=0.0,
         points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30
     )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split='val',
+    valset = SBDDataset(
+        cfg.SBD_PATH,
+        split="val",
         augmentator=val_augmentator,
-        min_object_area=80,
+        min_object_area=1000,
         points_sampler=points_sampler,
-        epoch_len=2000
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[140, 155], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=160)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,120 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'resnet34'
+MODEL_NAME = "resnet34"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 140
 
-    model = DeeplabModel(backbone='resnet34', deeplab_ch=128, aspp_dropout=0.20, use_leaky_relu=True,
-                         use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights()
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = LvisDataset(
-        cfg.LVIS_PATH,
-        split='train',
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = OpenImagesDataset(
+        cfg.OPENIMAGES_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=30000
+        epoch_len=30000,
+        dry_run=dry_run,
     )
 
-    valset = LvisDataset(
-        cfg.LVIS_PATH,
-        split='val',
+    valset = OpenImagesDataset(
+        cfg.OPENIMAGES_PATH,
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
+        keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[140, 155], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=160)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,125 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'resnet34'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 140
 
-    model = DeeplabModel(backbone='resnet34', deeplab_ch=128, aspp_dropout=0.20, use_leaky_relu=True,
-                         use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights()
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
+    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
+    loss_cfg.instance_aux_loss_weight = 0.4
+
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
+
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.8,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
-
-    trainset = OpenImagesDataset(
-        cfg.OPENIMAGES_PATH,
-        split='train',
+    trainset = CocoDataset(
+        cfg.COCO_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=30000
+        stuff_prob=0.30,
+        epoch_len=30000,
+        dry_run=dry_run,
     )
 
-    valset = OpenImagesDataset(
-        cfg.OPENIMAGES_PATH,
-        split='val',
+    valset = CocoDataset(
+        cfg.COCO_PATH,
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
         keep_background_prob=0.05,
         points_sampler=points_sampler,
-        epoch_len=2000
+        epoch_len=2000,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[120, 135], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=140)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py` & `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,130 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'resnet34'
+MODEL_NAME = "hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 120
 
-    model = DeeplabModel(backbone='resnet34', deeplab_ch=128, aspp_dropout=0.20, use_leaky_relu=True,
-                         use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights()
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
+    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
+    loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.40)),
+            HorizontalFlip(),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
 
-    trainset = SBDDataset(
-        cfg.SBD_PATH,
-        split='train',
+    val_augmentator = Compose(
+        [
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+        ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.80,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = ComposeDataset(
+        [
+            PascalVocDataset(
+                cfg.PASCALVOC_PATH, split="train", dry_run=dry_run
+            ),
+            SBDDataset(
+                cfg.SBD_PATH,
+                split="train",
+                samples_scores_path="./assets/sbd_samples_weights.pkl",
+                samples_scores_gamma=1.25,
+                dry_run=dry_run,
+            ),
+        ],
         augmentator=train_augmentator,
         min_object_area=80,
         keep_background_prob=0.0,
         points_sampler=points_sampler,
-        samples_scores_path='./assets/sbd_samples_weights.pkl',
-        samples_scores_gamma=1.25
     )
 
     valset = SBDDataset(
         cfg.SBD_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
         min_object_area=1000,
         points_sampler=points_sampler,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[100, 115], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=120)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py` & `ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,135 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = 'resnet34'
+MODEL_NAME = "sbd_hrnet18"
 
 
-def main(cfg):
-    model, model_cfg = init_model(cfg)
-    train(model, cfg, model_cfg)
-
-
-def init_model(cfg):
+def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 220
 
-    model = DeeplabModel(backbone='resnet34', deeplab_ch=128, aspp_dropout=0.20, use_leaky_relu=True,  # noqa: E501
-                         use_rgb_conv=False, use_disks=True, norm_radius=5)
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
+        use_rgb_conv=False,
+        use_disks=True,
+        norm_radius=5,
+        with_prev_mask=True,
+    )
 
     model.to(cfg.device)
-    model.apply(initializer.XavierGluon(rnd_type='gaussian', magnitude=2.0))
-    model.feature_extractor.load_pretrained_weights()
+    model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
+    if not dry_run:
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def train(model, cfg, model_cfg):
+def get_trainer(model, cfg, model_cfg, dry_run=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
+    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
+    loss_cfg.instance_aux_loss_weight = 0.4
 
-    train_augmentator = Compose([
-        UniformRandomResize(scale_range=(0.75, 1.40)),
-        HorizontalFlip(),
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size),
-        RandomBrightnessContrast(brightness_limit=(-0.25, 0.25), contrast_limit=(-0.15, 0.4), p=0.75),
-        RGBShift(r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75)
-    ], p=1.0)
-
-    val_augmentator = Compose([
-        PadIfNeeded(min_height=crop_size[0], min_width=crop_size[1], border_mode=0),
-        RandomCrop(*crop_size)
-    ], p=1.0)
-
-    points_sampler = MultiPointSampler(model_cfg.num_max_points, prob_gamma=0.8,  # noqa:E501
-                                       merge_objects_prob=0.15,
-                                       max_num_merged_objects=2)
+    train_augmentator = Compose(
+        [
+            UniformRandomResize(scale_range=(0.75, 1.25)),
+            Flip(),
+            RandomRotate90(),
+            ShiftScaleRotate(
+                shift_limit=0.03,
+                scale_limit=0,
+                rotate_limit=(-3, 3),
+                border_mode=0,
+                p=0.75,
+            ),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
+            RandomBrightnessContrast(
+                brightness_limit=(-0.25, 0.25),
+                contrast_limit=(-0.15, 0.4),
+                p=0.75,
+            ),
+            RGBShift(
+                r_shift_limit=10, g_shift_limit=10, b_shift_limit=10, p=0.75
+            ),
+        ],
+        p=1.0,
+    )
 
-    trainset = ComposeDataset(
+    val_augmentator = Compose(
         [
-            PascalVocDataset(cfg.PASCALVOC_PATH, split='train'),
-            SBDDataset(
-                cfg.SBD_PATH,
-                split='train',
-                samples_scores_path='./assets/sbd_samples_weights.pkl',
-                samples_scores_gamma=1.25
-            )
+            UniformRandomResize(scale_range=(0.75, 1.25)),
+            PadIfNeeded(
+                min_height=crop_size[0], min_width=crop_size[1], border_mode=0
+            ),
+            RandomCrop(*crop_size),
         ],
+        p=1.0,
+    )
+
+    points_sampler = MultiPointSampler(
+        model_cfg.num_max_points,
+        prob_gamma=0.80,
+        merge_objects_prob=0.15,
+        max_num_merged_objects=2,
+    )
+
+    trainset = SBDDataset(
+        cfg.SBD_PATH,
+        split="train",
         augmentator=train_augmentator,
         min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler
+        keep_background_prob=0.01,
+        points_sampler=points_sampler,
+        samples_scores_path="./assets/sbd_samples_weights.pkl",
+        samples_scores_gamma=1.25,
+        dry_run=dry_run,
     )
 
     valset = SBDDataset(
         cfg.SBD_PATH,
-        split='val',
+        split="val",
         augmentator=val_augmentator,
-        min_object_area=1000,
+        min_object_area=80,
         points_sampler=points_sampler,
+        epoch_len=500,
+        dry_run=dry_run,
     )
 
-    optimizer_params = {
-        'lr': 5e-4, 'betas': (0.9, 0.999), 'eps': 1e-8
-    }
-
-    lr_scheduler = partial(torch.optim.lr_scheduler.MultiStepLR,
-                           milestones=[100, 115], gamma=0.1)
-    trainer = ISTrainer(model, cfg, model_cfg, loss_cfg,
-                        trainset, valset,
-                        optimizer='adam',
-                        optimizer_params=optimizer_params,
-                        lr_scheduler=lr_scheduler,
-                        checkpoint_interval=5,
-                        image_dump_interval=2000,
-                        metrics=[AdaptiveIoU()],
-                        max_interactive_points=model_cfg.num_max_points)
-    trainer.run(num_epochs=120)
+    optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
+
+    lr_scheduler = partial(
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 215], gamma=0.1
+    )
+    return ISTrainer(
+        model,
+        cfg,
+        model_cfg,
+        loss_cfg,
+        trainset,
+        valset,
+        optimizer="adam",
+        optimizer_params=optimizer_params,
+        lr_scheduler=lr_scheduler,
+        checkpoint_interval=[(0, 5), (100, 1)],
+        image_dump_interval=3000,
+        metrics=[AdaptiveIoU()],
+        max_interactive_points=model_cfg.num_max_points,
+        max_num_next_clicks=3,
+        dry_run=dry_run,
+    )
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/utils/cython/_get_dist_maps.pyx` & `ritm_annotation-0.0.7/ritm_annotation/utils/cython/_get_dist_maps.pyx`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/utils/distributed.py` & `ritm_annotation-0.0.7/ritm_annotation/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/utils/exp.py` & `ritm_annotation-0.0.7/ritm_annotation/utils/exp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import os
-import pprint
 import shutil
 import sys
 from datetime import datetime
 from pathlib import Path
 
 import torch
 import yaml  # type: ignore
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation/utils/exp_imports/default.py` & `ritm_annotation-0.0.7/ritm_annotation/utils/exp_imports/default.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/utils/log.py` & `ritm_annotation-0.0.7/ritm_annotation/utils/log.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/utils/serialization.py` & `ritm_annotation-0.0.7/ritm_annotation/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation/utils/vis.py` & `ritm_annotation-0.0.7/ritm_annotation/utils/vis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.6/ritm_annotation.egg-info/PKG-INFO` & `ritm_annotation-0.0.7/ritm_annotation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritm-annotation
-Version: 0.0.6
+Version: 0.0.7
 Summary: Awesome ritm_annotation created by lucasew
 Home-page: https://github.com/lucasew/ritm_annotation/
 Author: lucasew
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `ritm_annotation-0.0.6/ritm_annotation.egg-info/SOURCES.txt` & `ritm_annotation-0.0.7/ritm_annotation.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ritm_annotation/base.py
 ritm_annotation.egg-info/PKG-INFO
 ritm_annotation.egg-info/SOURCES.txt
 ritm_annotation.egg-info/dependency_links.txt
 ritm_annotation.egg-info/entry_points.txt
 ritm_annotation.egg-info/requires.txt
 ritm_annotation.egg-info/top_level.txt
+ritm_annotation/cli/README.md
 ritm_annotation/cli/__init__.py
 ritm_annotation/cli/annotate/__init__.py
 ritm_annotation/cli/annotate/canvas.py
 ritm_annotation/cli/annotate/controller.py
 ritm_annotation/cli/annotate/wrappers.py
 ritm_annotation/cli/model_info/__init__.py
 ritm_annotation/cli/train/__init__.py
@@ -70,15 +71,17 @@
 ritm_annotation/model/modeling/__init__.py
 ritm_annotation/model/modeling/basic_blocks.py
 ritm_annotation/model/modeling/deeplab_v3.py
 ritm_annotation/model/modeling/hrnet_ocr.py
 ritm_annotation/model/modeling/ocr.py
 ritm_annotation/model/modeling/resnet.py
 ritm_annotation/model/modeling/resnetv1b.py
+ritm_annotation/models/README.md
 ritm_annotation/models/__init__.py
+ritm_annotation/models/test_exposed_model_stuff.py
 ritm_annotation/models/cocolvis_loss_ablation/__init__.py
 ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py
 ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py
 ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py
 ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py
 ritm_annotation/models/iter_mask/__init__.py
 ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py
@@ -96,14 +99,15 @@
 ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py
+ritm_annotation/utils/README.md
 ritm_annotation/utils/__init__.py
 ritm_annotation/utils/distributed.py
 ritm_annotation/utils/exp.py
 ritm_annotation/utils/log.py
 ritm_annotation/utils/misc.py
 ritm_annotation/utils/serialization.py
 ritm_annotation/utils/vis.py
```

### Comparing `ritm_annotation-0.0.6/setup.py` & `ritm_annotation-0.0.7/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/dronevis-1.0.0.tar.gz` & `tmp/dronevis-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronevis-1.0.0.tar", last modified: Sat Mar  4 22:13:48 2023, max compression
+gzip compressed data, was "dronevis-1.1.0.tar", last modified: Mon Jul 31 01:56:56 2023, max compression
```

## Comparing `dronevis-1.0.0.tar` & `dronevis-1.1.0.tar`

### file list

```diff
@@ -1,72 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.534342 dronevis-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-04 22:11:41.000000 dronevis-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-04 22:11:41.000000 dronevis-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-03-04 22:13:48.534342 dronevis-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-03-04 22:11:41.000000 dronevis-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-04 22:11:41.000000 dronevis-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-04 22:11:41.000000 dronevis-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 22:13:48.534342 dronevis-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-04 22:11:41.000000 dronevis-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.526341 dronevis-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.526341 dronevis-1.0.0/src/dronevis/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.526341 dronevis-1.0.0/src/dronevis/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/abstract/abstract_gluoncv_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/abstract/abstract_torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/abstract/base_drone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/abstract/base_video_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/abstract/noop_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.530341 dronevis-1.0.0/src/dronevis/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/backward.png
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/connect.png
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/down.png
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/forward.png
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/left.png
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/right.png
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/rotate_ccw.png
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/rotate_cw.png
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/assets/up.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.530341 dronevis-1.0.0/src/dronevis/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/config/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/config/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.530341 dronevis-1.0.0/src/dronevis/drone_connect/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/drone_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/drone_connect/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/drone_connect/demo_drone.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/drone_connect/drone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/drone_connect/navdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/drone_connect/navdata_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/drone_connect/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/main_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.530341 dronevis-1.0.0/src/dronevis/models/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/models/faster_rcnn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/models/human_tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/models/mediapipe_face_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/models/pose_mediapipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/models/ssd_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/models/yolov5_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.534342 dronevis-1.0.0/src/dronevis/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/ui/circular_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/ui/drone_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/ui/drone_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/ui/image_bw_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/ui/main_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/ui/navdata_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.534342 dronevis-1.0.0/src/dronevis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/utils/control_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-03-04 22:11:41.000000 dronevis-1.0.0/src/dronevis/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 22:13:48.526341 dronevis-1.0.0/src/dronevis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-03-04 22:13:48.000000 dronevis-1.0.0/src/dronevis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-04 22:13:48.000000 dronevis-1.0.0/src/dronevis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 22:13:48.000000 dronevis-1.0.0/src/dronevis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-04 22:13:48.000000 dronevis-1.0.0/src/dronevis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-04 22:13:48.000000 dronevis-1.0.0/src/dronevis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-04 22:13:48.000000 dronevis-1.0.0/src/dronevis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.354909 dronevis-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-31 01:54:01.000000 dronevis-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 01:54:01.000000 dronevis-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-31 01:56:56.354909 dronevis-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-31 01:54:01.000000 dronevis-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-31 01:54:01.000000 dronevis-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 01:54:01.000000 dronevis-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 01:56:56.354909 dronevis-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 01:54:01.000000 dronevis-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.346909 dronevis-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.346909 dronevis-1.1.0/src/dronevis/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.350909 dronevis-1.1.0/src/dronevis/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/abstract/abstract_torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/abstract/base_drone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/abstract/base_video_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/abstract/noop_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.350909 dronevis-1.1.0/src/dronevis/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/backward.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/connect.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/down.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/forward.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/left.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/right.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/rotate_ccw.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/rotate_cw.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/assets/up.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.354909 dronevis-1.1.0/src/dronevis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/config/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/config/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.354909 dronevis-1.1.0/src/dronevis/drone_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/drone_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/drone_connect/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/drone_connect/demo_drone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/drone_connect/drone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/drone_connect/navdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/drone_connect/navdata_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/drone_connect/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/main_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.354909 dronevis-1.1.0/src/dronevis/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/faster_rcnn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/gesture_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/human_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/pose_mediapipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/ssd_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/yolov5_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/models/yolov8.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.354909 dronevis-1.1.0/src/dronevis/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/ui/drone_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/ui/drone_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/ui/gui_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.354909 dronevis-1.1.0/src/dronevis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/utils/control_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-31 01:54:01.000000 dronevis-1.1.0/src/dronevis/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:56:56.346909 dronevis-1.1.0/src/dronevis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-31 01:56:56.000000 dronevis-1.1.0/src/dronevis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-31 01:56:56.000000 dronevis-1.1.0/src/dronevis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:56:56.000000 dronevis-1.1.0/src/dronevis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 01:56:56.000000 dronevis-1.1.0/src/dronevis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 01:56:56.000000 dronevis-1.1.0/src/dronevis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 01:56:56.000000 dronevis-1.1.0/src/dronevis.egg-info/top_level.txt
```

### Comparing `dronevis-1.0.0/LICENSE` & `dronevis-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/PKG-INFO` & `dronevis-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,32 @@
 Metadata-Version: 2.1
 Name: dronevis
-Version: 1.0.0
+Version: 1.1.0
 Summary: Full compatible drone library to automate computer vision algorithms on parrot drones.
 Author-email: Ahmed Heakl <ahmed.heakl@ejust.edu.eg>
 Project-URL: repository, https://github.com/ahmedheakl/drone-vis
 Keywords: drone,computer vision,human tracking,object recognition,YOLO,human counting,face detection,mediapipe,pytorch,sockets,thread
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
-<p><img src="https://badge.fury.io/py/dronevis.svg">
-<img src="https://readthedocs.org/projects/drone-vis/badge/?version=latest">
-<img src="https://github.com/ahmedheakl/drone-vis/workflows/build/badge.svg">
-<img src="https://img.shields.io/badge/code%20style-black-000000.svg">
-<img src="https://codecov.io/github/ahmedheakl/drone-vis/branch/master/graph/badge.svg">
-<img src="https://github.com/ahmedheakl/drone-vis/workflows/test/badge.svg">
-</p>
-
-<p>
-<img src="https://img.shields.io/badge/gitlab%20ci-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" height=20>
-<img src="https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge" height=20>
-</p>
-
-**`Documentation`** |
-------------------- |
-[![Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://drone-vis.readthedocs.io/en/latest) |
+<img src="https://user-images.githubusercontent.com/52796111/235324370-646b53c8-7540-4555-8097-63b4ead2d4fc.png" align="right" width="30%"/>
 
+![CI](https://github.com/ahmedheakl/drone-vis/workflows/test/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/drone-vis/badge/?version=latest)](https://drone-vis.readthedocs.io/) ![coverage report](https://codecov.io/github/ahmedheakl/drone-vis/branch/master/graph/badge.svg)
+[![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Version](https://badge.fury.io/py/dronevis.svg)
+# DroneVision
 
-# DroneVis: Full compatible drone library to automate computer vision algorithms on parrot drones.
+Drone Vision (DroneVis) is a full compatible drone library to automate computer vision algorithms on parrot drones. You can read a detailed documentation of Drone Vision [docs](https://drone-vis.readthedocs.io/en/latest).
 
 **DroneVis** is a cutting-edge drone software library that has been specifically designed for use with the AR. Drone 2.0. It has been extensively tested both indoors and outdoors, and offers a wide range of features including adaptability in connecting to the drone, advanced computer vision algorithms, and a user-friendly interface. This makes it easy for users to take full advantage of the drone's capabilities and control it with simple commands.All of the implemented real-time data, inference, and detection achieve a minimum ``fps >= 4.5`` on an Intel core 8 CPU.
 
 ## Features
 - Unified state-of-the art computer vision algoritms
 - Full control over the drone
 - PEP8 compliant (unified code style)
@@ -130,14 +114,14 @@
 
 ## Citing the Project
 
 To cite this repository:
 
 ```bibtex
 @software{drone-vis,
-  author  = {Ahmed Heakl, Abdallah-Elbarkokry, Fatma Youssef},
+  author  = {Ahmed Heakl, Abdallah-Elbarkokry, Fatma Youssef, Youssief Anas},
   title   = {Dronevis: Full compatible drone library to automate computer vision algorithms on parrot drones},
-  year    = {2022},
+  year    = {2023},
   url     = {github.com/ahmedheakl/drone-vis},
-  version = {0.2.2}
+  version = {1.0.0}
 }
 ```
```

### Comparing `dronevis-1.0.0/README.md` & `dronevis-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,16 @@
-<p><img src="https://badge.fury.io/py/dronevis.svg">
-<img src="https://readthedocs.org/projects/drone-vis/badge/?version=latest">
-<img src="https://github.com/ahmedheakl/drone-vis/workflows/build/badge.svg">
-<img src="https://img.shields.io/badge/code%20style-black-000000.svg">
-<img src="https://codecov.io/github/ahmedheakl/drone-vis/branch/master/graph/badge.svg">
-<img src="https://github.com/ahmedheakl/drone-vis/workflows/test/badge.svg">
-</p>
-
-<p>
-<img src="https://img.shields.io/badge/gitlab%20ci-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" height=20>
-<img src="https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge" height=20>
-</p>
-
-**`Documentation`** |
-------------------- |
-[![Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://drone-vis.readthedocs.io/en/latest) |
+<img src="https://user-images.githubusercontent.com/52796111/235324370-646b53c8-7540-4555-8097-63b4ead2d4fc.png" align="right" width="30%"/>
 
+![CI](https://github.com/ahmedheakl/drone-vis/workflows/test/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/drone-vis/badge/?version=latest)](https://drone-vis.readthedocs.io/) ![coverage report](https://codecov.io/github/ahmedheakl/drone-vis/branch/master/graph/badge.svg)
+[![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Version](https://badge.fury.io/py/dronevis.svg)
+# DroneVision
 
-# DroneVis: Full compatible drone library to automate computer vision algorithms on parrot drones.
+Drone Vision (DroneVis) is a full compatible drone library to automate computer vision algorithms on parrot drones. You can read a detailed documentation of Drone Vision [docs](https://drone-vis.readthedocs.io/en/latest).
 
 **DroneVis** is a cutting-edge drone software library that has been specifically designed for use with the AR. Drone 2.0. It has been extensively tested both indoors and outdoors, and offers a wide range of features including adaptability in connecting to the drone, advanced computer vision algorithms, and a user-friendly interface. This makes it easy for users to take full advantage of the drone's capabilities and control it with simple commands.All of the implemented real-time data, inference, and detection achieve a minimum ``fps >= 4.5`` on an Intel core 8 CPU.
 
 ## Features
 - Unified state-of-the art computer vision algoritms
 - Full control over the drone
 - PEP8 compliant (unified code style)
@@ -114,14 +98,14 @@
 
 ## Citing the Project
 
 To cite this repository:
 
 ```bibtex
 @software{drone-vis,
-  author  = {Ahmed Heakl, Abdallah-Elbarkokry, Fatma Youssef},
+  author  = {Ahmed Heakl, Abdallah-Elbarkokry, Fatma Youssef, Youssief Anas},
   title   = {Dronevis: Full compatible drone library to automate computer vision algorithms on parrot drones},
-  year    = {2022},
+  year    = {2023},
   url     = {github.com/ahmedheakl/drone-vis},
-  version = {0.2.2}
+  version = {1.0.0}
 }
 ```
```

### Comparing `dronevis-1.0.0/pyproject.toml` & `dronevis-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dronevis"
-version = "1.0.0"
+version = "1.1.0"
 description = "Full compatible drone library to automate computer vision algorithms on parrot drones."
 readme = "README.md"
 authors = [{ name = "Ahmed Heakl", email = "ahmed.heakl@ejust.edu.eg" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -31,15 +31,15 @@
     dronevis-gui = "dronevis.main_gui:main"
 
     [project.urls]
     repository = "https://github.com/ahmedheakl/drone-vis"
 
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "bump version {old_version} -> {new_version}"
 
     [tool.bumpver.file_patterns]
     "pyproject.toml" = [
         'current_version = "{version}"',
         'version = "{version}"',
```

### Comparing `dronevis-1.0.0/src/dronevis/__main__.py` & `dronevis-1.1.0/src/dronevis/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,33 +10,33 @@
     $ dronevis --help
 
 Or just run the following to the default
     $ dronevis
 
 Version
 ------------------
- - dronevis v1.0.0
+ - dronevis v1.1.0
 """
-import sys
+from typing import Optional, Sequence
 import logging
 
 from dronevis.drone_connect import DemoDrone, Drone
 from dronevis.ui.drone_cli import DroneCli
 from dronevis.utils.general import library_ontro, init_logger
 from dronevis.abstract.base_drone import BaseDrone
 
 _LOG = logging.getLogger(__name__)
 
 
-def main() -> None:
+def main(arguments: Optional[Sequence[str]] = None) -> None:
     """Running CLI script and CLI main loop"""
 
     # parse user arguments
     cli = DroneCli()
-    args = cli.parse()
+    args = cli.parse(arguments)
     init_logger(level=args.logger_level)
 
     # initialize drone instance
     if args.drone == "demo":
         drone: BaseDrone = DemoDrone()
     else:
         drone = Drone()
@@ -48,22 +48,23 @@
     try:
         cli(args, drone)
 
     except KeyboardInterrupt:
         print("")
         _LOG.warning("Keyinterrupt: closing CLI ...")
         drone.stop()
-        sys.exit()
 
     except NotImplementedError:
         _LOG.error("Drone tests are NOT yet implemented")
 
     except ConnectionError:
-        _LOG.error("Couldn't connect to the drone")
-        _LOG.error("Make sure you are connected to the drone network")
+        _LOG.error(
+            "Couldn't connect to the drone\n%s",
+            "Make sure you are connected to the drone network",
+        )
 
     except (ValueError, AssertionError) as error:
-        _LOG.error(error)
+        _LOG.error("An error occured: %s", error)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dronevis-1.0.0/src/dronevis/abstract/abstract_gluoncv_model.py` & `dronevis-1.1.0/src/dronevis/ui/gui_components.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,201 +1,227 @@
-"""Interface for models implemented with GluonCV"""
-from abc import abstractmethod
-from typing import List, Union
-import time
-import logging
-import matplotlib.pyplot as plt
-import numpy as np
-import cv2
-from gluoncv import utils, model_zoo
+"""Implementation of a tkinter circular progress bar for the GUI"""
+import os
+import inspect
+from typing import Tuple
+from tkinter import Canvas, Button, messagebox
+from tkinter.ttk import Label, Frame
+from PIL import Image, ImageTk, ImageOps
 
-from dronevis.utils.general import write_fps
-from dronevis.abstract.abstract_model import CVModel
+import dronevis
+from dronevis.config.gui import GREEN_COLOR, WHITE_COLOR, MAIN_COLOR, MAIN_FONT
 
-_LOG = logging.getLogger(__name__)
 
+class CircularProgressbar:
+    """Circular progress bar implementation for presenting drone navigation data"""
 
-class GluonCVModel(CVModel):
-    """Base class (inherits from CV abstract model) for creating custom gluoncv models.
-    To use the abstract class just inherit it, and override the following abstract methods:
-
-    - ``transform_img``: transform input image to be fed into model for inference
-    - ``load_and_transform_img``: load image from given path and transform it
-    """
-
-    def __init__(self, model_name: str, short_size: int = 512) -> None:
-        """Initialize Base model
+    start_ang: float = 0.0
 
+    def __init__(
+        self,
+        canvas: Canvas,
+        bottom_coord: Tuple[int, int],
+        top_coord: Tuple[int, int],
+        width: int = 2,
+    ) -> None:
+        """Contruct circular progressbar
         Args:
-            model_name (str): name of the implemented model
-            short_size (int, optional): Resize image short side to this short and keep aspect ratio.
-                                        Defaults to 512.
-        """
-        self.short_size = short_size
-        self.net = None
-        self.class_ids = None
-        self.scores = None
-        self.bounding_boxes = None
-        self.model_name = model_name
-
-    def load_model(self, model_path: str = "ssd_512_mobilenet1.0_voc_int8") -> None:
-        """Load the model from model zoo.
-        Run ``get_model_options`` to get model options.
+            canvas (tkinter.Canvas): a tkinter canvas to render the progressbar
+            x0 (int): x pos for bottom oval
+            y0 (int): y pos for bottom oval
+            x1 (int): x pos for top oval
+            y1 (int): y pos for top oval
+            width (int, optional): width of circular bar. Defaults to 2.
+            start_ang (float, optional): starting angle. Defaults to 0.0.
+        """
+        self.canvas = canvas
+
+        x0_coords, y0_coords, x1_coords, y1_coords = (
+            bottom_coord[0] + width,
+            bottom_coord[1] + width,
+            top_coord[0] - width,
+            top_coord[1] - width,
+        )
+        self.text_x = (top_coord[0] - bottom_coord[0]) / 2 + 10
+        self.text_y = (top_coord[1] - bottom_coord[1]) / 2 + width * 3
+        self.width = width
+        # draw static bar outline
+        mid_width = width / 2
+        self.canvas.create_oval(
+            x0_coords - mid_width,
+            y0_coords - mid_width,
+            x1_coords + mid_width,
+            y1_coords + mid_width,
+            outline=GREEN_COLOR,
+        )
+        self.canvas.create_oval(
+            x0_coords + mid_width,
+            y0_coords + mid_width,
+            x1_coords - mid_width,
+            y1_coords - mid_width,
+            outline=GREEN_COLOR,
+        )
+        self.extent = 0
+        self.arc_id = self.canvas.create_arc(
+            x0_coords,
+            y0_coords,
+            x1_coords,
+            y1_coords,
+            start=self.start_ang,
+            extent=0,
+            width=self.width,
+            style="arc",
+            outline="green",
+        )
+        percent = "0%"
+        self.label_id = self.canvas.create_text(
+            self.text_x, self.text_y, text=percent, fill="white"
+        )
 
+    def change(self, extent: float, text: str) -> None:
+        """Change data in the progress bar
         Args:
-            model_name (str): name of the pretrained model
+            extent (float): angle of the progressbar
+            text (str): text to be displayed in the middle
         """
-        self.net = model_zoo.get_model(model_path, pretrained=True)
-
-    def predict(self, image: np.ndarray, img_data=None) -> np.ndarray:
-        """Generate predictions along with a labelled img
-
-        Args:
-            img_data (mxnet.NDArray): input to the network
-            img (numpy.ndarray): normal img with un-normalized colors
+        self.canvas.itemconfigure(self.arc_id, extent=extent)
+        self.canvas.itemconfigure(self.label_id, text=text)
 
-        Returns:
-            numpy.ndarray: output image with boxes drawn around detected objects
-        """
+    def change_canvas(self, canvas: Canvas) -> None:
+        """Changed canvas object"""
+        self.canvas = canvas
 
-        assert (
-            self.net
-        ), "You need to load the model first. Please run load_model method."
 
-        self.class_ids, self.scores, self.bounding_boxes = self.net(img_data)
-        labelled_img = utils.viz.cv_plot_bbox(
-            image,
-            self.bounding_boxes[0],
-            self.scores[0],
-            self.class_ids[0],
-            class_names=self.net.classes,
-        )
-        return labelled_img
+class ImageBWButton(Button):
+    """Image button with alternating black/white image"""
 
-    def plot_bounding_box(self, img: np.ndarray) -> None:
-        """Show bounding boxes on input on ``matplotlib`` window
+    # pylint: disable=too-many-arguments
+    def __init__(
+        self,
+        master,
+        title: str,
+        message: str,
+        img: str,
+        size: Tuple[int, ...],
+        *args,
+        **kw,
+    ) -> None:
+        """Initialize image button
+        The button deals with two images ``passive`` and ``active``.
+        Each image is used in case of hover/no-hover.
 
-        .. note::
+        The active image is an __inverted__ version of the passive.
 
-            You must run the inference in the input image first
+        Image path is defaulted to be in the assets folder.
 
         Args:
-            img (numpy.ndarray): input_image
+            master (tkiner.widget): master widget
+            title (str): title of info box
+            message (str): message to be displayed in info box
+            img (str): image path
+            size (Tuple[int, ...]): size for image to be resized
+            is_inverted (bool): whether to invert the colors
         """
-        assert (
-            self.net
-        ), "You need to load the model first. Please run load_model method."
-
-        assert (
-            self.bounding_boxes is not None
-        ), "You need to inference the model first. Run predict func."
-        assert (
-            self.scores is not None
-        ), "You need to inference the model first. Run predict func."
-        assert (
-            self.class_ids is not None
-        ), "You need to inference the model first. Run predict func."
+        super().__init__(master, *args, **kw)
+        self["background"] = MAIN_COLOR
+        self["activebackground"] = WHITE_COLOR
+        package_path = os.path.dirname(inspect.getfile(dronevis))
+        passive_img_path = f"{package_path}/assets/{img}"
+        passive_img = Image.open(passive_img_path)
+        passive_img = passive_img.resize(size, Image.Resampling.HAMMING)
+        active_img = ImageOps.invert(passive_img.convert("1"))
+        self.passive_img = ImageTk.PhotoImage(passive_img)
+        self.active_img = ImageTk.PhotoImage(active_img)
+        self["image"] = self.passive_img
 
-        utils.viz.plot_bbox(
-            img,
-            self.bounding_boxes[0],
-            self.scores[0],
-            self.class_ids[0],
-            class_names=self.net.classes,
-        )
+        self.message = message
+        self.title = title
 
-        plt.show()
+        self.bind("<Button-3>", self.on_info)
+        self.bind("<Enter>", self.on_enter)
+        self.bind("<Leave>", self.on_leave)
 
-    @abstractmethod
-    def transform_img(self, image: np.ndarray) -> np.ndarray:
-        """Run transformations on input image
+    def on_info(self, _) -> None:
+        """Show information about the button
 
         Args:
-            image (np.ndarray): Input image as array
-
-        Returns:
-            np.ndarray: Image after transformation
+            e (tkinter.Event): event information
         """
+        messagebox.showinfo(title=self.title, message=self.message)
 
-    @abstractmethod
-    def load_and_transform_img(self, img_path: str):
-        """Load image from disk and run transformation
+    def on_enter(self, _) -> None:
+        """Event handler for entering hover
 
         Args:
-            img_path (str): Relative/absolute image path on disk
+            e (tkinter.Event): event information
         """
+        self["image"] = self.active_img
 
-    def add_bounding_box(self, img: np.ndarray) -> np.ndarray:
-        """Add bouding boxes along with their scores to input image
+    def on_leave(self, _) -> None:
+        """Event handler for leaving hover
 
         Args:
-            img (numpy.ndarray): input image
-
-        Returns:
-            numpy.ndarray: labelled image
+            e (tkinter.Event): Event handler for hover
         """
+        self["image"] = self.passive_img
 
-        assert (
-            self.net
-        ), "You need to load the model first. Please run load_model method."
-        assert (
-            self.bounding_boxes is not None
-        ), "You need to inference the model first. Run predict func."
-        assert (
-            self.scores is not None
-        ), "You need to inference the model first. Run predict func."
-        assert (
-            self.class_ids is not None
-        ), "You need to inference the model first. Run predict func."
 
-        return utils.viz.cv_plot_bbox(
-            img,
-            self.bounding_boxes[0],
-            self.scores[0],
-            self.class_ids[0],
-            class_names=self.net.classes,
-        )
+class MainButton(Button):
+    """Main tkinter button for GUI"""
 
-    def get_model_options(self) -> List[str]:
-        """Get options for model name
+    def __init__(self, master, message: str, *args, **kw) -> None:
+        """Contruct main button style
 
-        Returns:
-            List[str]: model name options
+        Args:
+            master (tkiner.Widget): parent of the button
+            message (str): message to be displayed in message box
         """
-        assert self.model_name is not None, "Use a model name."
-        options_for_center_net = []
-        for model_name in model_zoo.get_model_list():
-            if self.model_name in model_name.lower():
-                options_for_center_net.append(model_name)
-        return options_for_center_net
+        super().__init__(master, *args, **kw)
+        self["foreground"] = WHITE_COLOR
+        self["background"] = MAIN_COLOR
+        self["activebackground"] = WHITE_COLOR
+        self["font"] = MAIN_FONT
+        self["borderwidth"] = 0
 
-    def detect_webcam(
-        self,
-        video_index: Union[str, int] = 0,
-        window_name: str = "Cam Detection",
-    ) -> None:
-        """Detecting objects with a webcam using current model
-        *(to quit running this function press 'q')*
+        self.message = message
+        self.bind("<Button-3>", self.on_info)
+
+    def on_info(self, _) -> None:
+        """Contruct message box"""
+        messagebox.showinfo(title=self["text"], message=self.message)
+
+
+class DataFrame(Frame):
+    """Implementation of Frame for view navigation data"""
+
+    def __init__(self, master: Frame, title: str, *args, **kw) -> None:
+        """Contruct a data frame designed for ploting navdata in progressbar style
 
         Args:
-            video_index (Union[str, int], optional): index of cam, can be a `url`. Defaults to 0.
-            window_name (str, optional): name of video window. Defaults to "Cam Detection".
+            master (tkinter.ttk.Frame): master frame
+            title (str): title to be displayed on top of progressbar
         """
+        super().__init__(master, *args, **kw)
+
+        self.rowconfigure(0, weight=1)
+        self.rowconfigure(1, weight=3)
+        self.columnconfigure(0, weight=1)
 
-        cap = cv2.VideoCapture(video_index)
-        if not cap.isOpened():
-            _LOG.warning("Error while trying to read video. Please check path again")
-
-        while cap.isOpened():
-            _, frame = cap.read()
-            start_time = time.time()
-            image_frames, img = self.transform_img(frame)
-            image = self.predict(img, image_frames)
-            end_time = time.time()
-            fps = 1 / (end_time - start_time)
-            wait_time = max(1, int(fps / 4))
-            cv2.imshow(window_name, write_fps(image, fps))
-            if cv2.waitKey(wait_time) & 0xFF == ord("q"):
-                break
+        self.title = title
+        self.lbl_title = Label(self, text=self.title)
+        self.canvas = Canvas(
+            self,
+            width=70,
+            height=65,
+            bd=2,
+            bg=MAIN_COLOR,
+            highlightthickness=1,
+            highlightbackground=MAIN_COLOR,
+        )
+        self.cpb = CircularProgressbar(
+            self.canvas,
+            bottom_coord=(10, 0),
+            top_coord=(60, 50),
+            width=10,
+        )
 
-        cap.release()
-        cv2.destroyAllWindows()
+        self.lbl_title.grid(row=0, column=0)
+        self.canvas.grid(row=1, column=0)
```

### Comparing `dronevis-1.0.0/src/dronevis/abstract/abstract_model.py` & `dronevis-1.1.0/src/dronevis/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/abstract/abstract_torch_model.py` & `dronevis-1.1.0/src/dronevis/abstract/abstract_torch_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """Interface for models implemented with PyTorch"""
 from typing import Union, Tuple, List, Optional
 import time
 import logging
+
 import numpy as np
 import torch
 import torchvision
 from torchvision.transforms.functional import to_pil_image
 import cv2
-from PIL import Image
 
 from dronevis.config.general import COCO_NAMES
 from dronevis.abstract.abstract_model import CVModel
 from dronevis.utils.general import write_fps
 
 _LOG = logging.getLogger(__name__)
 
 
 class TorchDetectionModel(CVModel):
     """Base class (inherits from CV abstract model) for creating custom PyTorch models.
     To use the abstract class just inherit it, and override the abstract method.
+
+    For each prediction, the model output 300 labels, and their corresponding 300 scores.
+    Labels are picked if they surpass the threshold accuracy.
     """
 
     coco_names = COCO_NAMES
     colors = np.random.uniform(0, 255, size=(len(COCO_NAMES), 3))
 
     def __init__(self) -> None:
         """Construct torch models, and detect device for inference (cuda or cpu).
@@ -32,17 +35,16 @@
         you have an available GPU. The property ``device``, contains the device that
         will be used for inference. You can change the device by changing the ``device`` property.
         """
 
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.transform: Optional[torchvision.transforms.Compose] = None
         self.net: Optional[torch.nn.Module] = None
-        self.pred_classes: Optional[List[np.ndarray]] = None
+        self.pred_classes: Optional[List[str]] = None
         self.pred_scores: Optional[np.ndarray] = None
-        self.pred_bboxes: Optional[np.ndarray] = None
         self.boxes: Optional[np.ndarray] = None
 
     def predict(
         self,
         image: np.ndarray,
         detection_threshold: float = 0.7,
     ) -> np.ndarray:
@@ -57,17 +59,14 @@
         """
         assert (
             self.net
         ), "Model not initialized! You need to load the model first. Please run `load_model`."
         assert (
             0.0 <= detection_threshold <= 1.0
         ), "Threshold must be a float between 0 and 1."
-        assert (
-            self.transform
-        ), "Model not initialized. You need to load the model first. Please run `load_model`."
 
         input_image = image
         with torch.no_grad():
             transformed_image = self.transform_img(image).to(self.device)
             transformed_image = transformed_image.unsqueeze(0)  # add a batch dimension
             outputs = self.net(transformed_image)[0]  # get outputs array
             self.pred_classes = [
@@ -100,29 +99,33 @@
             self.transform is not None
         ), "Model not initialized. You need to load the model first. Please run `load_model`."
         pil_image = to_pil_image(image)
         transformed_image = self.transform(pil_image).to(self.device)
         return transformed_image
 
     def draw_boxes(
-        self, boxes: np.ndarray, classes: List, labels: torch.Tensor, image: np.ndarray
+        self,
+        boxes: np.ndarray,
+        classes: List[str],
+        labels: torch.Tensor,
+        image: np.ndarray,
     ) -> np.ndarray:
         """Draw boxes for the predicted classes in an image using torch model
 
         Args:
             boxes(numpy.ndarray): predicted boxes returned by predict function
             classes(List): predicted classes in an image returned by predict function
             labels(torch.Tensor): class labels in an image returned by predict function
             image(numpy.ndarray): an image to draw boxes on.
 
         Returns:
             numpy.ndarray: cv2 image after drawing boxes of the predicted classes on
             it with their labels
         """
-        image = cv2.cvtColor(np.asarray(image), cv2.COLOR_BGR2RGB)
+        image = cv2.cvtColor(np.asarray(image, dtype=np.float32), cv2.COLOR_BGR2RGB)
         for i, box in enumerate(boxes):
             color = self.colors[labels[i]]
             cv2.rectangle(
                 img=image,
                 pt1=(int(box[0]), int(box[1])),
                 pt2=(int(box[2]), int(box[3])),
                 color=color,
@@ -136,31 +139,14 @@
                 fontScale=0.8,
                 color=color,
                 thickness=2,
                 lineType=cv2.LINE_AA,
             )
         return cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
 
-    def transform_and_load_img(self, img_path: str, output_path: str) -> None:
-        """Detecting objects in a given image using torch model
-
-        *(to quit running this function press 'q')*
-
-        Args:
-            img_path (str): path of the image to load
-        """
-        image = Image.open(img_path)
-        image = np.asarray(image)
-        boxes, classes, labels = self.predict(image)
-        image = self.draw_boxes(boxes, classes, labels, image)
-        cv2.imshow("Predicted Image", image)
-        if output_path is not None:
-            cv2.imwrite(output_path, image)
-        cv2.waitKey(0)
-
     def detect_webcam(
         self,
         video_index: Union[int, str] = 0,
         window_name: str = "Cam Detection",
     ) -> None:
         """Detecting objects with a webcam using torch model
         *(to quit running this function press 'q')*
@@ -170,44 +156,22 @@
         Args:
             video_index (int, optional): device index used to retrieve video stream, it
             can be an index or an IP. Defaults to 0.
             window_name (str, optional): name of video stream window. Defaults to "Cam Detection".
         """
 
         cap = cv2.VideoCapture(video_index)
-        if not cap.isOpened():
-            _LOG.warning("Error while trying to read video. Please check path again")
-        prev_time = 0.0
+
         while cap.isOpened():
+            prev_time = time.time()
             _, frame = cap.read()
             with torch.no_grad():
                 image = self.predict(frame, 0.7)
-            cur_time = time.time()
-            fps = 1 / (cur_time - prev_time)
+            fps = 1 / (time.time() - prev_time)
             wait_time = max(1, int(fps / 4))
             image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
             cv2.imshow(window_name, write_fps(image, fps))
-            prev_time = cur_time
             if cv2.waitKey(wait_time) & 0xFF == ord("q"):
                 break
 
         cap.release()
         cv2.destroyAllWindows()
-
-    def frame_detection(self, frame: np.ndarray) -> Tuple[np.ndarray, float, float]:
-        """Detect a single frame of a video stream
-
-        Args:
-            frame (numpy.ndarray): input frame
-
-        Returns:
-            Tuple[numpy.ndarray, float, fps]: image with detection results and wait
-            time between frames
-        """
-        start_time = time.time()
-        with torch.no_grad():
-            image = self.predict(frame, 0.7)
-        end_time = time.time()
-        fps = 1 / (end_time - start_time)
-        wait_time = max(1, int(fps / 4))
-        image = cv2.cvtColor(write_fps(image, fps), cv2.COLOR_BGR2RGB)
-        return image, wait_time, fps
```

### Comparing `dronevis-1.0.0/src/dronevis/abstract/base_drone.py` & `dronevis-1.1.0/src/dronevis/abstract/base_drone.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 """Inteface for drone classes"""
 from typing import Callable, Optional
 import logging
+import socket
 from inspect import getmro
 
 from dronevis.abstract import CVModel
 from dronevis.abstract.base_video_thread import BaseVideoThread
 
 _LOG = logging.getLogger(__name__)
 
 
 class BaseDrone:
     """Interface and base class for real and demo drone"""
 
     def __init__(self, ip_address: str = "192.168.1.1") -> None:
+        if not self._validate_ip(ip_address):
+            raise ValueError(f"Invalid IP address {ip_address}")
+
         self.ip_address = ip_address
         self.is_connected = False
         self.video_thread: Optional[BaseVideoThread] = None
 
+    def _validate_ip(self, ip_address) -> bool:
+        """Validate input IP address"""
+        try:
+            socket.inet_aton(ip_address)
+            return True
+        except OSError:
+            return False
+
     def connect_video(self, callback: Callable, model: CVModel) -> None:
         """Initialize and start video thread
 
         Args:
             callback (Callable): Callback to be invoked after closing the video thread
             model (CVModel): Computer vision to run over the video stream
```

### Comparing `dronevis-1.0.0/src/dronevis/abstract/noop_model.py` & `dronevis-1.1.0/src/dronevis/abstract/noop_model.py`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/backward.png` & `dronevis-1.1.0/src/dronevis/assets/backward.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/connect.png` & `dronevis-1.1.0/src/dronevis/assets/connect.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/down.png` & `dronevis-1.1.0/src/dronevis/assets/down.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/forward.png` & `dronevis-1.1.0/src/dronevis/assets/forward.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/left.png` & `dronevis-1.1.0/src/dronevis/assets/left.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/right.png` & `dronevis-1.1.0/src/dronevis/assets/right.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/rotate_ccw.png` & `dronevis-1.1.0/src/dronevis/assets/rotate_ccw.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/rotate_cw.png` & `dronevis-1.1.0/src/dronevis/assets/rotate_cw.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/assets/up.png` & `dronevis-1.1.0/src/dronevis/assets/up.png`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/config/general.py` & `dronevis-1.1.0/src/dronevis/config/general.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 """Configurations for dronevis"""
+from typing import Dict, Any, Callable, Tuple, List
+
 from dronevis.utils.control_utils import (
     detect_tag,
     activate_gps,
     activate_navdata,
     indoor,
     outdoor,
     nervosity_level,
     max_altitude,
     goto_gps_point,
     flip,
 )
 
-SUPPORTED_CONFIG = {
+SUPPORTED_CONFIG: Dict[str, Callable[[Any], List[Tuple[str, str]]]] = {
     "detect_tag": detect_tag,
     "activate_navdata": activate_navdata,
     "activate_gps": activate_gps,  # Data activation
     "indoor": indoor,
     "outdoor": outdoor,
     "nervosity_level": nervosity_level,
     "max_altitude": max_altitude,  # One-time config
 }
+
 AUTONOMOUS_FLIGHT = {"gps": goto_gps_point}
 ANIMATIONS = {"flip": flip}
 ANIMATIONS_INFOS = {"flip": "(side)"}
-# Check if animations corelate
-if ANIMATIONS.keys() != ANIMATIONS_INFOS.keys():
-    raise ImportError("Animations differs")
+
+MODELS_URLS = {
+    "gesture_recognition": [
+        "https://drive.google.com/uc?export=download&id=1FTJWeavbHwmu9Vkr_M5k5mV4Lt8sWGFo",
+        "gesture_recognition.pth",
+    ],
+}
+
+GESTURES_LABELS = {
+    "Down": 0,
+    "Forward": 1,
+    "Left": 2,
+    "Right": 3,
+    "Stop": 4,
+    "Up": 5,
+}
 
 
 COCO_NAMES = [
     "__background__",
     "person",
     "bicycle",
     "car",
```

### Comparing `dronevis-1.0.0/src/dronevis/config/gui.py` & `dronevis-1.1.0/src/dronevis/config/gui.py`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/drone_connect/command.py` & `dronevis-1.1.0/src/dronevis/drone_connect/command.py`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/drone_connect/demo_drone.py` & `dronevis-1.1.0/src/dronevis/drone_connect/demo_drone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Implementation for demo drone for testing purposes"""
-from typing import Optional, Callable
+from typing import Optional, Callable, Union
 import logging
 import random
 import time
 from threading import Thread
 
 from dronevis.abstract import CVModel
 from dronevis.abstract.base_drone import BaseDrone
@@ -16,15 +16,14 @@
     """Demo class for running ``demo GUI``."""
 
     def __init__(self, ip_address: str = "192.168.1.1") -> None:
         """Construct demo object"""
         super().__init__(ip_address)
         self.nav_thread: Optional[DemoNavThread] = None
         self.video_thread: Optional[DemoVideoThread] = None
-        self.ip_address = ip_address
 
     def connect_video(self, callback: Callable, model: CVModel) -> None:
         """Retrieve video stream by connecting to the video port
 
         Args:
             callback (Callable): Callback after closing the video thread
             model (CVModel): Computer vision model to run on the video stream
@@ -34,15 +33,15 @@
             TypeError: The computer vision provided should implement the `CVModel`
             interface
         """
 
         super().connect_video(callback, model)
 
         self.video_thread = DemoVideoThread(callback, model)
-        self.video_thread.start()
+        self.video_thread.resume()
 
     def disconnect_video(self):
         """Disconnect video stream, and close the correspoding
         thread
 
         Raises:
             ValueError: Cannot close a stream that is not openned in the
@@ -50,16 +49,14 @@
         """
         if self.video_thread is None:
             err_message = "Video stream is not initialized"
             _LOG.error(err_message)
             raise ValueError(err_message)
 
         self.video_thread.stop()
-        time.sleep(0.2)
-        self.video_thread = None
         _LOG.debug("Video thread stopped")
 
     def connect(self) -> None:
         """Connect to drone
         Note that it is an idle method in this case
         """
         _LOG.info("drone connected")
@@ -73,26 +70,25 @@
 
         Raises:
             TypeError: Provided callback should be a function or None.
         """
         if callback is None:
             callback = self._print_navdata
 
-        if not hasattr(callable, "__call__"):
+        if not hasattr(callback, "__call__"):
             err_message = "Please provide a function as a callback or None."
             _LOG.error(err_message)
             raise TypeError(err_message)
 
         if self.nav_thread is None:
             self.nav_thread = DemoNavThread(callback)
             self.nav_thread.start()
             _LOG.debug("Nav thread started")
         else:
             self.nav_thread.change_callback(callback)
-            self.nav_thread.start()
             _LOG.debug("Changed callback")
 
     def set_config(self, **kwargs) -> bool:
         """Setter for configurations (gps, navdata)
 
         Args:
             activate_gps (bool, optional): Flag for starting gps. Defaults to True.
@@ -170,44 +166,48 @@
         return True
 
     def emergency(self) -> bool:
         """Simulate emergency"""
         _LOG.info("Emergency")
         return True
 
-    def stop(self):
+    def stop(self) -> None:
         """Simulate stopping"""
         self.is_connected = False
         if self.video_thread is not None:
-            self.video_thread.stop()
+            self.video_thread.close_thread()
             self.video_thread.join()
             _LOG.debug("Video thread stopped")
+            self.video_thread = None
 
         if self.nav_thread is not None:
             self.nav_thread.stop()
             self.nav_thread.join()
             _LOG.debug("Nav thread stopped")
+            self.nav_thread = None
 
         _LOG.warning("Drone disconnected")
 
-    def reset(self):
+    def reset(self) -> bool:
         """Simulate resting"""
         _LOG.info("Reseting")
+        return True
 
 
 class DemoVideoThread(BaseVideoThread):
     """Demo for video thread implementing `BaseVideoThread` interface"""
 
     def __init__(
         self,
         closing_callback: Callable,
         model: CVModel,
         ip_address: str = "192.168.1.1",
+        video_index: Union[int, str] = 0,
     ) -> None:
-        super().__init__(closing_callback, model, ip_address)
+        super().__init__(closing_callback, model, ip_address, video_index)
         self.frame = "Demo Video Capture"
 
 
 class DemoNavThread(Thread):
     """Demo for navigation data thread"""
 
     def __init__(
```

### Comparing `dronevis-1.0.0/src/dronevis/drone_connect/drone.py` & `dronevis-1.1.0/src/dronevis/drone_connect/drone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Implementation for real drone control"""
-from typing import Callable, Optional, List
+from typing import Callable, Optional, List, Tuple
 import logging
 import struct
 import time
 import socket
 
 from dronevis.abstract import CVModel
 from dronevis.abstract.base_drone import BaseDrone
@@ -44,25 +44,24 @@
         Raises:
             TypeError: Provided callback should be callable
         """
 
         super().connect_video(callback=callback, model=model)
 
         self.video_thread = VideoThread(callback, model, self.ip_address)
-        self.video_thread.start()
+        self.video_thread.resume()
         _LOG.debug("Initialized video thread")
 
     def disconnect_video(self) -> None:
         """Disconnect video stream"""
         if self.video_thread is None:
             _LOG.warning("Video thread is not initialized")
             return
 
         self.video_thread.stop()
-        self.video_thread = None
         _LOG.debug("Disconnected video thread")
 
     def connect(self) -> None:
         """Start communication thread to send control commands
 
         Raises:
             ConnectionError: Lost connection to drone
@@ -108,19 +107,18 @@
         for key_arg in kwargs:
             _LOG.debug(key_arg)
             if key_arg.lower() not in list(cfg.SUPPORTED_CONFIG):
                 err_message = f"The configuration key {key_arg} can't be found!"
                 _LOG.critical(err_message)
                 raise AttributeError(err_message)
         # Then set each config
-        at_commands: List[str] = []
+        at_commands: List[Tuple[str, str]] = []
         for key_arg in kwargs:
-            at_commands = at_commands + cfg.SUPPORTED_CONFIG[key_arg.lower()](
-                kwargs[key_arg.lower()]
-            )
+            config_out = cfg.SUPPORTED_CONFIG[key_arg.lower()](kwargs[key_arg.lower()])
+            at_commands.extend(config_out)
         for at_command in at_commands:
             self.com_thread.configure(at_command[0], at_command[1])
         return True
 
     def list_config(self) -> list:
         """List all possible configuration
 
@@ -320,15 +318,15 @@
             self.com_thread.stop()
 
         if self.nav_thread is not None:
             self.nav_thread.stop()
             self.nav_thread.join()
 
         if self.video_thread is not None:
-            self.video_thread.stop()
+            self.video_thread.close_thread()
             self.video_thread.join()
 
     def set_callback(self, callback=None):
         "Set the callback function"
         # Check if the argument is a function
         if callback is None:
             callback = self._print_navdata
```

### Comparing `dronevis-1.0.0/src/dronevis/drone_connect/navdata.py` & `dronevis-1.1.0/src/dronevis/drone_connect/navdata.py`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/drone_connect/navdata_decode.py` & `dronevis-1.1.0/src/dronevis/drone_connect/navdata_decode.py`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/drone_connect/video.py` & `dronevis-1.1.0/src/dronevis/drone_connect/video.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,10 +21,10 @@
         """Initialize drone instance
 
         Args:
             closing_callback (Callable): Callback to be invoked after closing thread
             model (CVModel): Computer vision model to run inference on the video stream
             ip_address (str, optional): IP address of the drone. Defaults to "192.168.1.1".
         """
-        super().__init__(closing_callback, model, ip_address)
+        video_index = f"{self.protocol}://{ip_address}:{self.video_port}"
+        super().__init__(closing_callback, model, ip_address, video_index=video_index)
         self.socket_lock = threading.Lock()
-        self.video_index = f"{self.protocol}://{ip_address}:{self.video_port}"
```

### Comparing `dronevis-1.0.0/src/dronevis/main_gui.py` & `dronevis-1.1.0/src/dronevis/main_gui.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,50 +11,51 @@
     $ dronevis-gui --help
 
 Or just run the following to the default
     $ dronevis-gui
 
 Version
 ------------------
- - dronevis-gui v0.2.1
+ - dronevis-gui v1.1.0
 """
+from typing import Optional, Sequence
 import logging
-import sys
 
 from dronevis.utils.general import library_ontro, gui_parse, init_logger
 from dronevis.drone_connect import DemoDrone, Drone
 from dronevis.abstract.base_drone import BaseDrone
 from dronevis.ui.drone_gui import DroneVisGui
 
 
 _LOG = logging.getLogger(__name__)
 
 
-def main() -> None:
+def main(argv: Optional[Sequence[str]] = None) -> None:
     """Running CLI script and CLI main loop"""
 
-    args = gui_parse()
+    args = gui_parse(argv)
     init_logger(level=args.logger_level)
 
     if args.drone == "demo":
         drone: BaseDrone = DemoDrone()
     else:
         drone = Drone()
 
     gui = DroneVisGui(drone=drone)
     library_ontro()
     try:
         gui()
 
-    except KeyboardInterrupt:
+    except KeyboardInterrupt as exec_info:
         print("")
         _LOG.warning("Closing GUI ...")
         gui.on_close_window()
-        sys.exit()
+        raise SystemExit(1) from exec_info
 
-    except (ConnectionError, AssertionError, ValueError, AttributeError) as error:
-        _LOG.error(error)
+    except (ConnectionError, AssertionError, ValueError, AttributeError) as exec_info:
+        _LOG.error(exec_info)
         gui.on_close_window()
+        raise SystemExit(1) from exec_info
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dronevis-1.0.0/src/dronevis/models/faster_rcnn_torch.py` & `dronevis-1.1.0/src/dronevis/models/faster_rcnn_torch.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,27 +8,23 @@
 
 _LOG = logging.getLogger(__name__)
 
 
 class FasterRCNN(TorchDetectionModel):
     """FasterRCNN model implementation for object detection/recognition"""
 
-    def __init__(self) -> None:
-        """Initialize faster R-CNN model"""
-        super().__init__()
-        self.weights = FasterRCNN_MobileNet_V3_Large_320_FPN_Weights.DEFAULT
-        self.transform = self.weights.transforms()
-
     def load_model(self) -> None:
         """Load model from PyTorchHub
 
         .. note::
 
             Default weights used are ``fasterrcnn_mobilenet_v3_large_320_fpn``.
         """
         _LOG.info("Loading Faster R-CNN model ...")
+        weights = FasterRCNN_MobileNet_V3_Large_320_FPN_Weights.DEFAULT
+        self.transform = weights.transforms()
         self.net = (
-            fasterrcnn_mobilenet_v3_large_320_fpn(weights=self.weights)
+            fasterrcnn_mobilenet_v3_large_320_fpn(weights=weights)
             .eval()
             .to(self.device)
         )
         _LOG.info("Loadded Faster R-CNN model")
```

### Comparing `dronevis-1.0.0/src/dronevis/models/human_tracking.py` & `dronevis-1.1.0/src/dronevis/models/human_tracking.py`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/models/mediapipe_face_detection.py` & `dronevis-1.1.0/src/dronevis/models/face_detection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Implementation for face detection from mediapipe"""
 from typing import Union
 import time
+
 import cv2
 import mediapipe as mp
 import numpy as np
 
 from dronevis.abstract import CVModel
 from dronevis.utils.general import write_fps
 
@@ -20,18 +21,20 @@
         """Construct model instance
 
         Args:
             confidence (float, optional): threshold for detection,
             **input is a probability [0, 1]**.
             Defaults to 0.5.
         """
-        assert 0.0 <= confidence <= 1, "Confidence must be a score between 0 and 1"
-        assert isinstance(confidence, (int, float)), "Confidence must be a number"
-        self.face_detection = mp.solutions.face_detection.FaceDetection(confidence)  # type: ignore
-        self.mp_drawing = mp.solutions.drawing_utils  # type: ignore
+        if not isinstance(confidence, (int, float)):
+            raise TypeError("Confidence must be a float or int")
+
+        assert 0.0 <= confidence <= 1.0, "Confidence must be a score between 0 and 1"
+        self.face_detection = mp.solutions.face_detection.FaceDetection(confidence)
+        self.mp_drawing = mp.solutions.drawing_utils
 
     def load_model(self) -> None:
         """Load model from memory"""
 
     def transform_img(self, image: np.ndarray) -> np.ndarray:
         """Idle transformation of the image"""
         return image
```

### Comparing `dronevis-1.0.0/src/dronevis/models/pose_mediapipe.py` & `dronevis-1.1.0/src/dronevis/models/pose_mediapipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Module for pose estimation and single-instance human segmentation"""
-
 import time
 from typing import Union
 import mediapipe as mp
 import numpy as np
 import cv2
 
 from dronevis.utils.general import write_fps
@@ -141,13 +140,7 @@
             cv2.imshow("Segmented Pose", write_fps(seg_pose, fps))
 
             if cv2.waitKey(1) & 0xFF == ord("q"):
                 break
 
         cv2.destroyAllWindows()
         cap.release()
-
-
-if __name__ == "__main__":
-    model = PoseSegEstimation()
-    model.load_model()
-    model.detect_webcam()
```

### Comparing `dronevis-1.0.0/src/dronevis/models/ssd_torch.py` & `dronevis-1.1.0/src/dronevis/models/ssd_torch.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,24 +9,20 @@
 _LOG = logging.getLogger(__name__)
 
 
 class SSD(TorchDetectionModel):
     """Single shot detector model implementation for object
     detection/recognition using torchvision pre-trained models"""
 
-    def __init__(self) -> None:
-        """Initialize SSD model and load weights"""
-        super().__init__()
-        self.weights = SSDLite320_MobileNet_V3_Large_Weights.DEFAULT
-        self.transform = self.weights.transforms()
-
     def load_model(self):
         """Load model from PyTorchHub
 
         .. note::
 
             Default weights used are ``ssdlite320_mobilenet_v3_large``.
         """
         _LOG.info("Loading SSD Torch model ...")
-        self.net = ssdlite320_mobilenet_v3_large(weights=self.weights)
+        weights = SSDLite320_MobileNet_V3_Large_Weights.DEFAULT
+        self.transform = weights.transforms()
+        self.net = ssdlite320_mobilenet_v3_large(weights=weights)
         self.net = self.net.eval().to(self.device)
         _LOG.info("Loaded SSD Torch model")
```

### Comparing `dronevis-1.0.0/src/dronevis/models/yolov5_torch.py` & `dronevis-1.1.0/src/dronevis/models/yolov5_torch.py`

 * *Files identical despite different names*

### Comparing `dronevis-1.0.0/src/dronevis/ui/drone_cli.py` & `dronevis-1.1.0/src/dronevis/ui/drone_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """implementation for dronevis CLI"""
 import argparse
 import logging
-from typing import Callable, Dict
+from typing import Callable, Dict, Optional, Sequence
 import sys
+
 from rich_argparse import RichHelpFormatter
 from rich.console import Console
 from rich.table import Table
 from rich import print as rprint
 
 from dronevis import __version__
 from dronevis.abstract.base_drone import BaseDrone
@@ -14,15 +15,15 @@
 
 _LOG = logging.getLogger(__name__)
 
 
 class DroneCli:
     """Encapsulate all CLI needed methods"""
 
-    def parse(self) -> argparse.Namespace:
+    def parse(self, arguments: Optional[Sequence[str]] = None) -> argparse.Namespace:
         """Argument parser to get user inputs
 
         Returns:
             argparse.Namespace: namespace with all user input arguments
         """
         parser = argparse.ArgumentParser(
             prog="DroneVis",
@@ -57,15 +58,15 @@
             dest="logger_level",
             type=str,
             choices=["debug", "info", "warning", "error", "critical"],
             default="info",
             help="Level for logger",
         )
 
-        args = parser.parse_args()
+        args = parser.parse_args(arguments)
         return args
 
     def print_available_control(self) -> None:
         """Print all drone available control, and mark them
         as either implemented with a green check mark or not implemented
         with a red X.
         """
@@ -95,31 +96,31 @@
         for i, control in enumerate(controls, start=1):
             valid = "✅" if i < 14 else "❌"
             table.add_row(f"{i}", control, valid)
 
         console = Console()
         console.print(table)
 
-    def not_implemeneted(self) -> None:
+    def _not_implemeneted(self) -> None:
         """Dummy method from not implemented methods
 
         Raises:
             NotImplementedError: main exception error
         """
         raise NotImplementedError("Not implemented yet")
 
     def index_to_control(self, drone: BaseDrone) -> Dict[str, Callable]:
         """Get a list a with keys as commands index and values
         as commands methods
 
         Args:
-            drone (BaseDrone): drone instance
+            drone (BaseDrone): Drone instance
 
         Returns:
-            Dict[str, Callable]: a dictionary mapping from index to control methods
+            Dict[str, Callable]: A dictionary mapping from index to control methods
         """
         assert isinstance(drone, BaseDrone), "Please provide a valid drone instance"
 
         def cli_exit():
             drone.stop()
             sys.exit()
 
@@ -134,32 +135,32 @@
             "7": drone.rotate_left,
             "8": drone.rotate_right,
             "9": drone.takeoff,
             "10": drone.land,
             "11": drone.hover,
             "12": drone.reset,
             "13": drone.emergency,
-            "14": self.not_implemeneted,
+            "14": self._not_implemeneted,
         }
 
         return available_commands
 
     def __call__(
         self,
         args: argparse.Namespace,
         drone: BaseDrone,
     ) -> None:
         """Main loop for drone connection and control
 
         Args:
-            args (argparse.NameSpace): args from user input
-            drone (BaseDrone): drone instance
+            args (argparse.NameSpace): Args from user input
+            drone (BaseDrone): Drone instance
 
         Raises:
-            NotImplementedError: drone testing is not implemented
+            NotImplementedError: Drone testing is not implemented
         """
         assert isinstance(
             drone, BaseDrone
         ), "Provided drone must implement the base drone interface"
 
         # get commands
         available_commands = self.index_to_control(drone)
@@ -190,8 +191,8 @@
 
                 command = available_commands[index]
                 command()
 
                 print("")
 
         else:
-            raise NotImplementedError()
+            raise NotImplementedError("Drone tests are not implemented yet")
```

### Comparing `dronevis-1.0.0/src/dronevis/ui/drone_gui.py` & `dronevis-1.1.0/src/dronevis/ui/drone_gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,67 @@
 """GUI implmentation"""
-from typing import Optional
+from typing import Optional, List
+
 from tkinter import Tk, StringVar, HORIZONTAL, LEFT
 from tkinter.ttk import Style, Frame, Label, Progressbar, OptionMenu
 import logging
+from dataclasses import dataclass, field
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
 from dronevis.models import FaceDetectModel, FasterRCNN, YOLOv5, PoseSegEstimation
 from dronevis.drone_connect import DemoDrone
 from dronevis.abstract.base_drone import BaseDrone
 from dronevis.utils.general import axis_config
 from dronevis.abstract.noop_model import NOOPModel
-
 from dronevis.config import gui as cfg
-from dronevis.ui.image_bw_button import ImageBWButton
-from dronevis.ui.main_button import MainButton
-from dronevis.ui.navdata_frame import DataFrame
+from dronevis.ui.gui_components import ImageBWButton, MainButton, DataFrame
 
 _LOG = logging.getLogger(__name__)
 
 
+@dataclass
+class GUIOpt:
+    """GUI attributes"""
+
+    axis: Optional[plt.Axes] = None
+    navdata: Optional[dict] = None
+    plot_job: Optional[str] = None
+    is_stream: bool = False
+    data: List[int] = field(default_factory=lambda: [0])
+    index: List[float] = field(default_factory=lambda: [0.0])
+    scatter: Optional[FigureCanvasTkAgg] = None
+
+
+@dataclass
+class GUIFrames:
+    """GUI Frames"""
+
+    pb_battery: Progressbar
+    lbl_battery_percentage: Label
+    frm_nav_vx: DataFrame
+    frm_nav_vy: DataFrame
+    frm_nav_vz: DataFrame
+    btn_connect: MainButton
+    btn_video_stream: MainButton
+
+
 class DroneVisGui:
     """Implementation for the library GUI using Tkinter"""
 
     models = {
         "none": NOOPModel,
         "face": FaceDetectModel,
         "yolov5": YOLOv5,
         "faster r-cnn": FasterRCNN,
         "pose": PoseSegEstimation,
         "seg": PoseSegEstimation,
         "pose+seg": PoseSegEstimation,
     }
+    mid_point = int((cfg.GUI_X_LIMIT / cfg.INDEX_STEP) // 2)
 
     def __init__(
         self,
         drone: Optional[BaseDrone] = None,
     ) -> None:
         """Contruct a GUI window
 
@@ -66,112 +92,104 @@
         )
         self.window.title("Drone Vision")
         self.window.rowconfigure(0, weight=1)
         self.window.columnconfigure(0, minsize=600, weight=1)
         self.window.columnconfigure(1, minsize=330, weight=1)
 
         # attributes initializations
-        self.ax = None
-        self.navdata = None
-        self.is_stream = False
-        self.data = [0]
-        self.index = [0]
-        self.mid_point = int((cfg.GUI_X_LIMIT / cfg.INDEX_STEP) // 2)
+        self.opt = GUIOpt()
+        self.init_frames()
+        _LOG.debug("Main frames initialized")
 
     def handle_navdata(self) -> None:
         """Handle incomming navdata and convert them to suitable format"""
-        if self.navdata is None:
+        if self.opt.navdata is None:
             return
 
-        navdata = self.navdata
+        navdata = self.opt.navdata
 
         # Battery comes in percentage format
         battery_percentage = int(navdata["navdata_demo"]["battery_percentage"])
-        self.pb_battery["value"] = battery_percentage
+        self.frms.pb_battery["value"] = battery_percentage
         self.lbl_battery_percentage["text"] = f"{battery_percentage}%"
 
-        ### velocity handling ###
-        # velocity comes in mm/s format
-        vx = navdata["navdata_demo"]["vx"] * cfg.MILLI_TO_METER_FACTOR
-        vx_text = f"{abs(vx):0.2f} m\\s"
-        self.frm_nav_vx.cpb.change(to_angle(abs(vx), cfg.MAX_VELOCITY), vx_text)
-
-        vy = navdata["navdata_demo"]["vy"] * cfg.MILLI_TO_METER_FACTOR
-        vy_text = f"{abs(vy):0.2f} m\\s"
-        self.frm_nav_vy.cpb.change(to_angle(abs(vy), cfg.MAX_VELOCITY), vy_text)
-
-        vz = navdata["navdata_demo"]["vz"] * cfg.MILLI_TO_METER_FACTOR
-        vz_text = f"{abs(vz):0.2f} m\\s"
-        self.frm_nav_vz.cpb.change(to_angle(abs(vz), cfg.MAX_VELOCITY), vz_text)
-
-        ### elevation handling ###
-        # elevation comes in mm format
-        h = int(navdata["navdata_demo"]["altitude"] * cfg.MILLI_TO_METER_FACTOR)
-        self.data.append(h)
-        last_index = self.index[-1]
-        self.index.append(last_index + cfg.INDEX_STEP)  # type: ignore
+        # Velocity comes in mm/s format
+        vel_x = navdata["navdata_demo"]["vx"] * cfg.MILLI_TO_METER_FACTOR
+        vx_text = f"{abs(vel_x):0.2f} m\\s"
+        self.frms.frm_nav_vx.cpb.change(to_angle(abs(vel_x), cfg.MAX_VELOCITY), vx_text)
+
+        vel_y = navdata["navdata_demo"]["vy"] * cfg.MILLI_TO_METER_FACTOR
+        vy_text = f"{abs(vel_y):0.2f} m\\s"
+        self.frms.frm_nav_vy.cpb.change(to_angle(abs(vel_y), cfg.MAX_VELOCITY), vy_text)
+
+        vel_z = navdata["navdata_demo"]["vz"] * cfg.MILLI_TO_METER_FACTOR
+        vz_text = f"{abs(vel_z):0.2f} m\\s"
+        self.frms.frm_nav_vz.cpb.change(to_angle(abs(vel_z), cfg.MAX_VELOCITY), vz_text)
+
+        # Elevation comes in mm format
+        elevation = int(navdata["navdata_demo"]["altitude"] * cfg.MILLI_TO_METER_FACTOR)
+        self.opt.data.append(elevation)
+        last_index = self.opt.index[-1]
+        self.opt.index.append(last_index + cfg.INDEX_STEP)
 
     def on_plot(self) -> None:
         """Handles heights points and graph them"""
 
-        # convert incoming navdata to suitable format
+        # Convert incoming navdata to suitable format
         self.handle_navdata()
 
-        # initialize axis if not exist
-        if self.ax is None:
-
-            # initialize a figure instance
+        # Initialize axis if not exist
+        if self.opt.axis is None or self.opt.scatter is None:
+            # Initialize a figure instance
             figure3 = plt.figure(figsize=(5, 4), dpi=90)
 
-            # set background color to MAIN COLOR
+            # Set background color to MAIN COLOR
             figure3.set_facecolor(cfg.MAIN_COLOR)
 
-            # create a subplot instance stored in self.ax
-            self.ax = figure3.add_subplot(111)
+            # Create a subplot instance stored in self.axis
+            self.opt.axis = figure3.add_subplot(111)
 
-            # plot data on created axis
-            self.ax.plot(self.index, self.data, color="g", linewidth=2)
+            # Plot data on created axis
+            self.opt.axis.plot(self.opt.index, self.opt.data, color="g", linewidth=2)
 
-            # create a tkinter widget with axis object
-            self.scatter3 = FigureCanvasTkAgg(figure3, self.frm_nav_h)
+            # Create a tkinter widget with axis object
+            self.opt.scatter = FigureCanvasTkAgg(figure3, self.frm_nav_h)
 
-            # place the plotting-tkiner widget
-            self.scatter3.get_tk_widget().grid(
+            # Place the plotting-tkiner widget
+            self.opt.scatter.get_tk_widget().grid(
                 row=0,
                 column=0,
                 sticky="nsew",
                 pady=5,
                 padx=5,
             )
 
-            # set configurations for the axis
-            axis_config(self.ax)
+            # Set configurations for the axis
+            axis_config(self.opt.axis)
 
         else:
-
             # if number of points exceeded the width of the graph
-            if len(self.index) > self.mid_point * 2:
-
+            if len(self.opt.index) > self.mid_point * 2:
                 # shifting data to left
-                first_point = self.index[self.mid_point]
-                self.index = self.index[self.mid_point :]
-                self.index = [i - first_point for i in self.index]
-                self.data = self.data[self.mid_point :]
-                self.cnt = len(self.index)
-                self.ax.clear()
-                self.scatter3.draw()
+                first_point = self.opt.index[self.mid_point]
+                self.opt.index = self.opt.index[self.mid_point :]
+                self.opt.index = [i - first_point for i in self.opt.index]
+                self.opt.data = self.opt.data[self.mid_point :]
+                self.opt.axis.clear()
+                self.opt.scatter.draw()
 
             # plot updated data and reset configs
-            self.ax.plot(self.index, self.data, color="g", linewidth=2)
-            axis_config(self.ax)
-            self.scatter3.draw()
+            self.opt.axis.plot(self.opt.index, self.opt.data, color="g", linewidth=2)
+            axis_config(self.opt.axis)
+            self.opt.scatter.draw()
 
         # recursive call to the plot function to run each 51 ms
-        self._plot_job = self.window.after(ms=51, func=self.on_plot)
+        self.opt.plot_job = self.window.after(ms=51, func=self.on_plot)
 
+    # pylint: disable=too-many-statements
     def init_frames(self):
         """Initialize main frames for the GUI"""
         frm_left = Frame(master=self.window)
         frm_right = Frame(master=self.window)
 
         # Left Configs
         frm_left.rowconfigure(0, minsize=480, weight=1)
@@ -192,15 +210,15 @@
 
         ######################## Battary Data ###################################
         frm_battary = Frame(frm_info, style="MainFrame.TFrame")
         lbl_battary = Label(
             frm_battary, text="Battery Percentage", font=cfg.HEADER_FONT
         )
         frm_progress = Frame(frm_battary)
-        self.pb_battery = Progressbar(
+        pb_battery = Progressbar(
             frm_progress,
             mode="determinate",
             length=300,
             maximum=100,
             orient=HORIZONTAL,
             value=0,
             style="Custom.Horizontal.TProgressbar",
@@ -222,22 +240,22 @@
         self.on_plot()
 
         frm_navdata = Frame(frm_nav_h)
         frm_navdata.rowconfigure(0, weight=1)
         frm_navdata.rowconfigure(1, weight=1)
         frm_navdata.rowconfigure(2, weight=1)
 
-        self.frm_nav_vx = DataFrame(frm_navdata, title="vx")
-        self.frm_nav_vx.grid(row=0, column=0, sticky="ew")
+        frm_nav_vx = DataFrame(frm_navdata, title="vx")
+        frm_nav_vx.grid(row=0, column=0, sticky="ew")
 
-        self.frm_nav_vy = DataFrame(frm_navdata, title="vy")
-        self.frm_nav_vy.grid(row=1, column=0, sticky="ew")
+        frm_nav_vy = DataFrame(frm_navdata, title="vy")
+        frm_nav_vy.grid(row=1, column=0, sticky="ew")
 
-        self.frm_nav_vz = DataFrame(frm_navdata, title="vz")
-        self.frm_nav_vz.grid(row=2, column=0, sticky="ew")
+        frm_nav_vz = DataFrame(frm_navdata, title="vz")
+        frm_nav_vz.grid(row=2, column=0, sticky="ew")
 
         ######################## Basic Control ##################################
         frm_basic_control = Frame(master=frm_right, style="MainFrame.TFrame")
         lbl_basic_control = Label(
             frm_basic_control, text="Basic Control", font=cfg.HEADER_FONT
         )
 
@@ -302,21 +320,21 @@
             title="DOWN",
             message="Move the drone down",
             img="down.png",
             size=cfg.VERTICAL_ARROW_SIZE,
             command=self.drone.downward,
         )
 
-        self.btn_connect = MainButton(
+        btn_connect = MainButton(
             frm_basic_control,
             message="Start drone connection",
             text="START",
         )
 
-        self.btn_connect.bind("<Button-1>", self.on_drone_connect)
+        btn_connect.bind("<Button-1>", self.on_drone_connect)
 
         for i in range(4):
             frm_basic_control.rowconfigure(i, weight=1)
             frm_basic_control.columnconfigure(i % 3, minsize=70, weight=1)
 
         ######################## Special Control #################################
         frm_special_control = Frame(master=frm_right, style="MainFrame.TFrame")
@@ -393,15 +411,15 @@
         )
         self.models_choice = StringVar()
         self.models_choice.set("none")
         btn_detection = OptionMenu(
             frm_vision_control, self.models_choice, *self.models.keys()
         )
 
-        self.btn_video_stream = MainButton(
+        btn_video_stream = MainButton(
             frm_vision_control,
             text="Stream",
             message="Initiate video stream from drone",
             command=self.on_stream,
         )
 
         for i in range(3):
@@ -415,15 +433,15 @@
         btn_backward.grid(row=3, column=1, sticky="ew", padx=2)
         btn_right.grid(row=2, column=2, sticky="ew", padx=5)
         btn_left.grid(row=2, column=0, sticky="ew", padx=2)
         btn_up.grid(row=3, column=2, sticky="ew", padx=5)
         btn_down.grid(row=3, column=0, sticky="ew", padx=5)
         btn_rotate_l.grid(row=1, column=0, sticky="ew", padx=5)
         btn_rotate_r.grid(row=1, column=2, sticky="ew", padx=2)
-        self.btn_connect.grid(row=2, column=1, sticky="ew", padx=5, pady=5)
+        btn_connect.grid(row=2, column=1, sticky="ew", padx=5, pady=5)
 
         # special control
         lbl_special_control.grid(row=0, columnspan=2, pady=5, padx=5)
         btn_take_off.grid(row=1, column=0, sticky="ew", padx=5)
         btn_land.grid(row=1, column=1, sticky="ew", padx=5)
         btn_hover.grid(row=2, column=0, sticky="ew", padx=5)
         btn_flip.grid(row=2, column=1, sticky="ew", padx=5)
@@ -432,85 +450,88 @@
         lbl_reset_control.grid(row=0, columnspan=3, padx=5)
         btn_reset.grid(row=1, column=0, sticky="ew", padx=5, ipady=2)
         btn_calib.grid(row=1, column=1, sticky="ew", padx=5, ipady=2)
         btn_emerg.grid(row=1, column=2, sticky="ew", padx=5, ipady=2)
 
         # battary info
         lbl_battary.grid(row=0, column=0)
-        self.pb_battery.pack(side=LEFT)
+        pb_battery.pack(side=LEFT)
         self.lbl_battery_percentage.pack(side=LEFT, padx=5)
         frm_progress.grid(row=2, column=0)
 
         # height graph
         frm_nav_h.grid(row=1, column=0, sticky="nsew")
         frm_navdata.grid(row=0, column=1, padx=5, pady=5, sticky="ns")
 
         # vision control
         lbl_vision_control.grid(row=0, column=1, pady=10)
         btn_record_video.grid(row=1, column=0, sticky="ew", padx=10, pady=10, ipady=2)
         btn_detection.grid(row=1, column=1, sticky="ew", padx=10, pady=10, ipady=2)
-        self.btn_video_stream.grid(
-            row=1, column=2, sticky="ew", padx=10, pady=10, ipady=2
-        )
+        btn_video_stream.grid(row=1, column=2, sticky="ew", padx=10, pady=10, ipady=2)
 
         # Left Frame
         frm_vision_control.grid(row=1, column=0, sticky="nsew")
         frm_info.grid(row=0, column=0, sticky="nsew")
         frm_battary.grid(row=0, column=0, sticky="nsew")
 
         # Right Frame
         frm_basic_control.grid(row=0, column=0, sticky="nsew")
         frm_special_control.grid(row=1, column=0, sticky="nsew")
         frm_reset_control.grid(row=2, column=0, sticky="nsew")
 
         frm_left.grid(row=0, column=0, sticky="nsew")
         frm_right.grid(row=0, column=1, sticky="nsew")
+        self.frms = GUIFrames(
+            pb_battery=pb_battery,
+            lbl_battery_percentage=self.lbl_battery_percentage,
+            frm_nav_vx=frm_nav_vx,
+            frm_nav_vy=frm_nav_vy,
+            frm_nav_vz=frm_nav_vz,
+            btn_connect=btn_connect,
+            btn_video_stream=btn_video_stream,
+        )
 
     def on_drone_connect(self, _):
-        """Event handler for drone connection
-
-        Args:
-            e (tkiner.Event): event for pressing on start button
-        """
+        """Event handler for drone connection"""
         self.drone.connect()  # connect drone
         self.drone.set_config(activate_gps=True, activate_navdata=True)
 
         # change connect button color
-        self.btn_connect["text"] = "Connected"
-        self.btn_connect["background"] = cfg.GREEN_COLOR
-        self.btn_connect["foreground"] = cfg.WHITE_COLOR
-        self.btn_connect["activebackground"] = cfg.RED_COLOR
-        self.btn_connect["activeforeground"] = cfg.WHITE_COLOR
+        self.frms.btn_connect["text"] = "Connected"
+        self.frms.btn_connect["background"] = cfg.GREEN_COLOR
+        self.frms.btn_connect["foreground"] = cfg.WHITE_COLOR
+        self.frms.btn_connect["activebackground"] = cfg.RED_COLOR
+        self.frms.btn_connect["activeforeground"] = cfg.WHITE_COLOR
 
         # set navdata handler as callback
         self.drone.set_callback(self.on_navdata)
 
-    def on_navdata(self, navdata):
+    def on_navdata(self, navdata: dict):
         """Callback handler to retrieve navdata from drone instance
 
         Args:
             navdata (dict): navigation data dictionary
         """
         if not self.drone.is_connected:
             return
 
-        self.navdata = navdata
+        self.opt.navdata = navdata
 
     def on_stream(self):
         """Event handler for pressing on stream button"""
         if self.drone.video_thread is not None:
             self.on_change_stream_model()
             return
 
         _LOG.info("Current Model: %s", self.models_choice.get())
-        self.is_stream = True
+        self.opt.is_stream = True
         model = self.get_and_load_model()
         close_stream_callback = idle
         self.drone.connect_video(close_stream_callback, model)
-        self.btn_video_stream["text"] = "change"
+        self.frms.btn_video_stream["text"] = "change"
 
     def get_and_load_model(self):
         """Retrieve chosen model and load its weights"""
         model_class = self.models[self.models_choice.get()]
         if self.models_choice.get() == "seg":
             model = model_class(is_seg=True)  # type: ignore
 
@@ -531,31 +552,29 @@
             raise ValueError(err_message)
 
         _LOG.info("Current Model: %s", self.models_choice.get())
         model = self.get_and_load_model()
         self.drone.video_thread.change_model(model)
 
     def __call__(self) -> None:
-        self.init_frames()
-        _LOG.debug("Main frames initialized")
         self.window.mainloop()
 
     def on_close_window(self):
         """Event handler for closing the GUI window
 
         It stop the drone connection and destroyes and GUI window
         """
-        if self._plot_job is None:
+        if self.opt.plot_job is None:
             err_message = "GUI closed before initialized"
             _LOG.critical(err_message)
             raise AssertionError(err_message)
 
         self.drone.stop()
-        self.window.after_cancel(self._plot_job)
-        self._plot_job = None
+        self.window.after_cancel(self.opt.plot_job)
+        self.opt.plot_job = None
         plt.close()
         self.window.destroy()
         _LOG.info("GUI closed")
 
 
 def idle() -> None:
     """Idle function"""
```

### Comparing `dronevis-1.0.0/src/dronevis/utils/control_utils.py` & `dronevis-1.1.0/src/dronevis/utils/control_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Utilities for controling the drone"""
 from typing import List, Tuple
 
 
-def activate_navdata(activate: bool = True) -> List[Tuple[str, ...]]:
+def activate_navdata(activate: bool = True) -> List[Tuple[str, str]]:
     "Prepare the drone so he can send navdata back to us"
     if activate:
         return [("general:navdata_demo", "FALSE")]  # Activate navdata
     return [("general:navdata_demo", "TRUE")]
 
 
-def activate_gps(activate: bool = True) -> List[Tuple[str, ...]]:
+def activate_gps(activate: bool = True) -> List[Tuple[str, str]]:
     "Prepare the drone to receive GPS command"
     if activate:
         return [("control:flying_mode", "0"), ("control:autonomous_flight", "FALSE")]
     return []
 
 
 def detect_tag(color: int = 0) -> List[Tuple[str, str]]:
@@ -109,17 +109,14 @@
         + str(longi)
         + ","
         + str(alt)
         + ",0,0,0,"
         + str(cap)
         + ",0"
     )
-    # Let's go !
     com = []
-    # if not continuous:  com.append(("control:flying_mode","0")) # To Check
-    # if not continuous:  com.append(("control:autonomous_flight","FALSE")) # To Check
     if not continuous:
         com.append(("control:flying_camera_enable", "FALSE"))
     com.append(("control:flying_camera_mode", param1))
     if not continuous:
         com.append(("control:flying_camera_enable", "TRUE"))
     return com
```

### Comparing `dronevis-1.0.0/src/dronevis/utils/general.py` & `dronevis-1.1.0/src/dronevis/utils/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Utilities for dronevis library including image processing and parser"""
-from typing import Union
+from typing import Union, Optional, Sequence
 import logging
 import os
 import argparse
+
 from pyfiglet import Figlet
 from rich import print as rprint
 from termcolor import colored
 from rich_argparse import RichHelpFormatter
 import cv2
 import numpy as np
 import coloredlogs
+import wget
+import torch
 
 from dronevis import __version__
 import dronevis.config.gui as cfg
 
 
 def write_fps(image: np.ndarray, fps: Union[str, int, float]) -> np.ndarray:
     """Write fps on input image
@@ -23,15 +26,15 @@
         fps (Union[str, int, float]): frame per second
 
     Returns:
         np.array: processed image with fps written
     """
     assert isinstance(fps, (str, int, float)), "Please enter a valid fps value"
     if not isinstance(fps, int):
-        fps = str(int(fps))
+        fps = str(int(float(fps)))
 
     cv2.putText(
         img=image,
         text=f"{fps} FPS",
         org=(15, 30),
         fontFace=cv2.FONT_HERSHEY_SIMPLEX,
         fontScale=1,
@@ -49,15 +52,15 @@
     rprint(
         "DroneVis is a full-compatible library for [green]controlling your drone [white]and"
         + "\nrunning your favourite [green]computer vision algorithms in real-time[white]"
     )
     print("----------------------------------------------------------")
 
 
-def gui_parse() -> argparse.Namespace:
+def gui_parse(arguments: Optional[Sequence[str]] = None) -> argparse.Namespace:
     """Parse arguments for the GUI script
 
     Returns:
         argparse.Namespace: parsed arguments of user input
     """
     parser = argparse.ArgumentParser(
         prog="DroneVisGUI",
@@ -84,15 +87,15 @@
         dest="logger_level",
         type=str,
         choices=["debug", "info", "warning", "error", "critical"],
         default="info",
         help="Level for logger",
     )
 
-    args = parser.parse_args()
+    args = parser.parse_args(arguments)
     return args
 
 
 def axis_config(axis) -> None:
     """Set the axis paramets for height graph in the GUI
 
     Args:
@@ -172,7 +175,35 @@
     logging.basicConfig(handlers=[f_handler])
 
     # initialize colored logs
     coloredlogs.install(
         fmt="%(asctime)s - %(message)s",
         level=log_level,
     )
+
+
+def download_file(file_url: str, file_name: str) -> str:
+    """Download file from url"""
+
+    # Define the path to the .cache directory for each operating system
+    if os.name == "nt":  # Windows
+        cache_dir = os.path.join(os.environ["LOCALAPPDATA"], ".cache/dronevis")
+    elif os.name == "posix":  # Linux or Mac
+        cache_dir = os.path.join(os.environ["HOME"], ".cache/dronevis")
+    else:
+        raise OSError("Unsupported operating system")
+
+    os.makedirs(cache_dir, exist_ok=True)
+    model_weights_path = os.path.join(cache_dir, file_name)
+
+    if os.path.exists(model_weights_path):
+        return model_weights_path
+
+    wget.download(file_url, model_weights_path)
+
+    return model_weights_path
+
+
+def device() -> str:
+    """Returns the device to be used for inference"""
+    device_name = os.getenv("DEVICE", "cuda" if torch.cuda.is_available() else "cpu")
+    return device_name
```

### Comparing `dronevis-1.0.0/src/dronevis.egg-info/PKG-INFO` & `dronevis-1.1.0/src/dronevis.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,32 @@
 Metadata-Version: 2.1
 Name: dronevis
-Version: 1.0.0
+Version: 1.1.0
 Summary: Full compatible drone library to automate computer vision algorithms on parrot drones.
 Author-email: Ahmed Heakl <ahmed.heakl@ejust.edu.eg>
 Project-URL: repository, https://github.com/ahmedheakl/drone-vis
 Keywords: drone,computer vision,human tracking,object recognition,YOLO,human counting,face detection,mediapipe,pytorch,sockets,thread
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
-<p><img src="https://badge.fury.io/py/dronevis.svg">
-<img src="https://readthedocs.org/projects/drone-vis/badge/?version=latest">
-<img src="https://github.com/ahmedheakl/drone-vis/workflows/build/badge.svg">
-<img src="https://img.shields.io/badge/code%20style-black-000000.svg">
-<img src="https://codecov.io/github/ahmedheakl/drone-vis/branch/master/graph/badge.svg">
-<img src="https://github.com/ahmedheakl/drone-vis/workflows/test/badge.svg">
-</p>
-
-<p>
-<img src="https://img.shields.io/badge/gitlab%20ci-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" height=20>
-
-<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" height=20>
-<img src="https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge" height=20>
-</p>
-
-**`Documentation`** |
-------------------- |
-[![Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://drone-vis.readthedocs.io/en/latest) |
+<img src="https://user-images.githubusercontent.com/52796111/235324370-646b53c8-7540-4555-8097-63b4ead2d4fc.png" align="right" width="30%"/>
 
+![CI](https://github.com/ahmedheakl/drone-vis/workflows/test/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/drone-vis/badge/?version=latest)](https://drone-vis.readthedocs.io/) ![coverage report](https://codecov.io/github/ahmedheakl/drone-vis/branch/master/graph/badge.svg)
+[![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Version](https://badge.fury.io/py/dronevis.svg)
+# DroneVision
 
-# DroneVis: Full compatible drone library to automate computer vision algorithms on parrot drones.
+Drone Vision (DroneVis) is a full compatible drone library to automate computer vision algorithms on parrot drones. You can read a detailed documentation of Drone Vision [docs](https://drone-vis.readthedocs.io/en/latest).
 
 **DroneVis** is a cutting-edge drone software library that has been specifically designed for use with the AR. Drone 2.0. It has been extensively tested both indoors and outdoors, and offers a wide range of features including adaptability in connecting to the drone, advanced computer vision algorithms, and a user-friendly interface. This makes it easy for users to take full advantage of the drone's capabilities and control it with simple commands.All of the implemented real-time data, inference, and detection achieve a minimum ``fps >= 4.5`` on an Intel core 8 CPU.
 
 ## Features
 - Unified state-of-the art computer vision algoritms
 - Full control over the drone
 - PEP8 compliant (unified code style)
@@ -130,14 +114,14 @@
 
 ## Citing the Project
 
 To cite this repository:
 
 ```bibtex
 @software{drone-vis,
-  author  = {Ahmed Heakl, Abdallah-Elbarkokry, Fatma Youssef},
+  author  = {Ahmed Heakl, Abdallah-Elbarkokry, Fatma Youssef, Youssief Anas},
   title   = {Dronevis: Full compatible drone library to automate computer vision algorithms on parrot drones},
-  year    = {2022},
+  year    = {2023},
   url     = {github.com/ahmedheakl/drone-vis},
-  version = {0.2.2}
+  version = {1.0.0}
 }
 ```
```

### Comparing `dronevis-1.0.0/src/dronevis.egg-info/SOURCES.txt` & `dronevis-1.1.0/src/dronevis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 src/dronevis.egg-info/PKG-INFO
 src/dronevis.egg-info/SOURCES.txt
 src/dronevis.egg-info/dependency_links.txt
 src/dronevis.egg-info/entry_points.txt
 src/dronevis.egg-info/requires.txt
 src/dronevis.egg-info/top_level.txt
 src/dronevis/abstract/__init__.py
-src/dronevis/abstract/abstract_gluoncv_model.py
 src/dronevis/abstract/abstract_model.py
 src/dronevis/abstract/abstract_torch_model.py
 src/dronevis/abstract/base_drone.py
 src/dronevis/abstract/base_video_thread.py
 src/dronevis/abstract/noop_model.py
 src/dronevis/assets/__init__.py
 src/dronevis/assets/backward.png
@@ -37,23 +36,22 @@
 src/dronevis/drone_connect/command.py
 src/dronevis/drone_connect/demo_drone.py
 src/dronevis/drone_connect/drone.py
 src/dronevis/drone_connect/navdata.py
 src/dronevis/drone_connect/navdata_decode.py
 src/dronevis/drone_connect/video.py
 src/dronevis/models/__init__.py
+src/dronevis/models/face_detection.py
 src/dronevis/models/faster_rcnn_torch.py
+src/dronevis/models/gesture_recognition.py
 src/dronevis/models/human_tracking.py
-src/dronevis/models/mediapipe_face_detection.py
 src/dronevis/models/pose_mediapipe.py
 src/dronevis/models/ssd_torch.py
 src/dronevis/models/yolov5_torch.py
+src/dronevis/models/yolov8.py
 src/dronevis/ui/__init__.py
-src/dronevis/ui/circular_progressbar.py
 src/dronevis/ui/drone_cli.py
 src/dronevis/ui/drone_gui.py
-src/dronevis/ui/image_bw_button.py
-src/dronevis/ui/main_button.py
-src/dronevis/ui/navdata_frame.py
+src/dronevis/ui/gui_components.py
 src/dronevis/utils/__init__.py
 src/dronevis/utils/control_utils.py
 src/dronevis/utils/general.py
```


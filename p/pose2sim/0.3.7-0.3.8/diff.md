# Comparing `tmp/pose2sim-0.3.7.tar.gz` & `tmp/pose2sim-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pose2sim-0.3.7.tar", last modified: Wed Jun  7 08:25:04 2023, max compression
+gzip compressed data, was "pose2sim-0.3.8.tar", last modified: Mon Jul 31 18:36:42 2023, max compression
```

## Comparing `pose2sim-0.3.7.tar` & `pose2sim-0.3.8.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.932855 pose2sim-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-07 08:24:51.000000 pose2sim-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    33028 2023-06-07 08:25:04.932855 pose2sim-0.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.740854 pose2sim-0.3.7/Pose2Sim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.740854 pose2sim-0.3.7/Pose2Sim/Demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.744854 pose2sim-0.3.7/Pose2Sim/Demo/User/
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/User/Config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/User/test.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.744854 pose2sim-0.3.7/Pose2Sim/Demo/calib-2d/
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/calib-2d/Calib.qca.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.744854 pose2sim-0.3.7/Pose2Sim/Demo/opensim/
--rw-r--r--   0 runner    (1001) docker     (123)   127289 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Balancing_for_IK.trc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.776854 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/
--rw-r--r--   0 runner    (1001) docker     (123)    87711 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/bofoot.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/capitate_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/capitate_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    29750 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv1sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv2sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv3sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv4sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv5sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv6sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv7.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/femur_l.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/femur_r.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/fibula_l.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/fibula_r.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    97470 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/foot.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hamate_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hamate_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)   137969 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hat_jaw.vtp
--rw-r--r--   0 runner    (1001) docker     (123)   737930 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hat_ribs_scap.vtp
--rw-r--r--   0 runner    (1001) docker     (123)   315678 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hat_skull.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    37639 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/humerus_lv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    37639 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/humerus_rv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_medial_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_medial_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    88317 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/l_bofoot.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    97518 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/l_foot.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/l_patella.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/l_pelvis.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_medial_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_medial_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar1.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar2.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar3.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar4.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar5.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lunate_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lunate_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal1_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    32726 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal1_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    24962 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal2_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    24966 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal2_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal3_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    35418 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal3_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal4_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal4_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    42678 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal5_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    42670 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal5_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_medial_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_medial_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/pisiform_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/pisiform_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/r_patella.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/r_pelvis.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/radius_lv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/radius_rv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_medial_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_medial_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/sacrum.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/scaphoid_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/scaphoid_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    51083 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/talus_lv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    51083 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/talus_rv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic10_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic11_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic12_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic1_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic2_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic3_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic4_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic5_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic6_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic7_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic8_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic9_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thumb_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thumb_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/tibia_l.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/tibia_r.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/trapezium_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/trapezium_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/trapezoid_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/trapezoid_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/triquetrum_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/triquetrum_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ulna_lv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ulna_rv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml
--rw-r--r--   0 runner    (1001) docker     (123)   453333 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim
--rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
--rw-r--r--   0 runner    (1001) docker     (123)    32333 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/opensim/Standing_for_Scaling.trc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.736854 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.804854 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0000.json
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0002.json
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0003.json
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0004.json
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0005.json
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0006.json
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0007.json
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0008.json
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0009.json
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0010.json
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0011.json
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0012.json
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0013.json
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0014.json
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0015.json
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0016.json
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0017.json
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0018.json
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0019.json
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0020.json
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0021.json
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0022.json
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0023.json
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0024.json
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0025.json
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0026.json
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0027.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0028.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0029.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0030.json
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0031.json
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0032.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0033.json
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0034.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0035.json
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0036.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0037.json
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0038.json
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0039.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0040.json
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0041.json
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0042.json
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0043.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0044.json
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0045.json
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0046.json
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0047.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0048.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0049.json
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0050.json
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0051.json
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0052.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0053.json
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0054.json
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0055.json
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0056.json
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0057.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0058.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0059.json
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0060.json
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0061.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0062.json
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0063.json
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0064.json
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0065.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0066.json
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0067.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0068.json
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0069.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0070.json
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0071.json
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0072.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0073.json
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0074.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0075.json
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0076.json
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0077.json
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0078.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0079.json
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0080.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0081.json
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0082.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0083.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0084.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0085.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0086.json
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0087.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0088.json
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0089.json
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0090.json
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0091.json
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0092.json
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0093.json
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0094.json
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0095.json
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0096.json
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0097.json
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0098.json
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0099.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.828855 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0000.json
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0002.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0003.json
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0004.json
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0005.json
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0006.json
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0007.json
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0008.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0009.json
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0010.json
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0011.json
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0012.json
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0013.json
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0014.json
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0015.json
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0016.json
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0017.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0018.json
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0019.json
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0020.json
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0021.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0022.json
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0023.json
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0024.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0025.json
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0026.json
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0027.json
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0028.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0029.json
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0030.json
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0031.json
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0032.json
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0033.json
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0034.json
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0035.json
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0036.json
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0037.json
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0038.json
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0039.json
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0040.json
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0041.json
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0042.json
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0043.json
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0044.json
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0045.json
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0046.json
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0047.json
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0048.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0049.json
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0050.json
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0051.json
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0052.json
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0053.json
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0054.json
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0055.json
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0056.json
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0057.json
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0058.json
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0059.json
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0060.json
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0061.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0062.json
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0063.json
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0064.json
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0065.json
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0066.json
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0067.json
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0068.json
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0069.json
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0070.json
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0071.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0072.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0073.json
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0074.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0075.json
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0076.json
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0077.json
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0078.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0079.json
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0080.json
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0081.json
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0082.json
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0083.json
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0084.json
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0085.json
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0086.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0087.json
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0088.json
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0089.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0090.json
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0091.json
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0092.json
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0093.json
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0094.json
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0095.json
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0096.json
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0097.json
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0098.json
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0099.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.852855 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0000.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0001.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0002.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0003.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0004.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0005.json
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0006.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0007.json
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0008.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0009.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0010.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0011.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0012.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0013.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0014.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0015.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0016.json
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0017.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0018.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0019.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0020.json
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0021.json
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0022.json
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0023.json
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0024.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0025.json
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0026.json
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0027.json
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0028.json
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0029.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0030.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0031.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0032.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0033.json
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0034.json
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0035.json
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0036.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0037.json
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0038.json
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0039.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0040.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0041.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0042.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0043.json
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0044.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0045.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0046.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0047.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0048.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0049.json
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0050.json
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0051.json
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0052.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0053.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0054.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0055.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0056.json
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0057.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0058.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0059.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0060.json
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0061.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0062.json
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0063.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0064.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0065.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0066.json
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0067.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0068.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0069.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0070.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0071.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0072.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0073.json
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0074.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0075.json
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0076.json
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0077.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0078.json
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0079.json
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0080.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0081.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0082.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0083.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0084.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0085.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0086.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0087.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0088.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0089.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0090.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0091.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0092.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0093.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0094.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0095.json
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0096.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0097.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0098.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0099.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.876855 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0000.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0001.json
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0002.json
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0003.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0004.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0005.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0006.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0007.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0008.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0009.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0010.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0011.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0012.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0013.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0014.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0015.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0016.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0017.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0018.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0019.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0020.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0021.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0022.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0023.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0024.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0025.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0026.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0027.json
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0028.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0029.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0030.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0031.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0032.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0033.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0034.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0035.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0036.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0037.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0038.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0039.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0040.json
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0041.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0042.json
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0043.json
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0044.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0045.json
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0046.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0047.json
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0048.json
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0049.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0050.json
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0051.json
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0052.json
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0053.json
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0054.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0055.json
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0056.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0057.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0058.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0059.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0060.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0061.json
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0062.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0063.json
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0064.json
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0065.json
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0066.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0067.json
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0068.json
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0069.json
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0070.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0071.json
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0072.json
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0073.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0074.json
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0075.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0076.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0077.json
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0078.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0079.json
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0080.json
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0081.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0082.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0083.json
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0084.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0085.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0086.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0087.json
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0088.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0089.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0090.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0091.json
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0092.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0093.json
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0094.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0095.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0096.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0097.json
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0098.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Demo/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.736854 pose2sim-0.3.7/Pose2Sim/Empty_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.876855 pose2sim-0.3.7/Pose2Sim/Empty_project/User/
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/User/Config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.888855 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.924855 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/
--rw-r--r--   0 runner    (1001) docker     (123)    87711 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    29750 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv3sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv4sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv5sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv6sm.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv7.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/femur_l.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/femur_r.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/fibula_l.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/fibula_r.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    97470 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/foot.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hamate_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hamate_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)   137969 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hat_jaw.vtp
--rw-r--r--   0 runner    (1001) docker     (123)   737930 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hat_ribs_scap.vtp
--rw-r--r--   0 runner    (1001) docker     (123)   315678 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hat_skull.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    37639 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/humerus_lv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    37639 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/humerus_rv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_medial_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_medial_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    88317 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/l_bofoot.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    97518 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/l_foot.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/l_patella.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/l_pelvis.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_medial_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_medial_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar1.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar2.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar3.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar4.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar5.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lunate_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lunate_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    32726 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    24962 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    24966 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    35418 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    42678 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    42670 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/pisiform_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/pisiform_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/r_patella.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/r_pelvis.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/radius_lv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/radius_rv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/sacrum.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    51083 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/talus_lv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    51083 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/talus_rv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic10_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic11_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic12_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic1_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic2_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic3_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic4_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic5_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic6_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic7_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic8_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic9_s.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/tibia_l.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/tibia_r.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/trapezium_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/trapezium_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_lvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_rvs.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ulna_lv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ulna_rv.vtp
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco18.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml
--rw-r--r--   0 runner    (1001) docker     (123)   454633 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim
--rw-r--r--   0 runner    (1001) docker     (123)   456161 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim
--rw-r--r--   0 runner    (1001) docker     (123)   458489 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim
--rw-r--r--   0 runner    (1001) docker     (123)   453368 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim
--rw-r--r--   0 runner    (1001) docker     (123)   456144 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim
--rw-r--r--   0 runner    (1001) docker     (123)   453673 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco18.osim
--rw-r--r--   0 runner    (1001) docker     (123)   453792 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim
--rw-r--r--   0 runner    (1001) docker     (123)   456561 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim
--rw-r--r--   0 runner    (1001) docker     (123)    24023 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30222 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30507 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml
--rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco18.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Pose2Sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.928855 pose2sim-0.3.7/Pose2Sim/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/AlphaPose_to_OpenPose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/DLC_to_OpenPose.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/c3d_to_trc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/calib_from_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/calib_qca_to_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/calib_toml_to_qca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/calib_toml_to_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/calib_yml_to_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/json_display_with_img.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/json_display_without_img.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/trc_Zup_to_Yup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/trc_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/trc_desample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/trc_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/trc_gaitevents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/Utilities/trc_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/calibrate_cams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/filter_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/track_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-06-07 08:24:51.000000 pose2sim-0.3.7/Pose2Sim/triangulate_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    30297 2023-06-07 08:24:51.000000 pose2sim-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:04.932855 pose2sim-0.3.7/pose2sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33028 2023-06-07 08:25:04.000000 pose2sim-0.3.7/pose2sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33119 2023-06-07 08:25:04.000000 pose2sim-0.3.7/pose2sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:25:04.000000 pose2sim-0.3.7/pose2sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:25:04.000000 pose2sim-0.3.7/pose2sim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-07 08:25:04.000000 pose2sim-0.3.7/pose2sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 08:25:04.000000 pose2sim-0.3.7/pose2sim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 08:24:51.000000 pose2sim-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-07 08:25:04.932855 pose2sim-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 08:24:51.000000 pose2sim-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.166090 pose2sim-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-31 18:36:25.000000 pose2sim-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-07-31 18:36:42.166090 pose2sim-0.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.042089 pose2sim-0.3.8/Pose2Sim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.042089 pose2sim-0.3.8/Pose2Sim/Demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.046089 pose2sim-0.3.8/Pose2Sim/Demo/User/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/User/Config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/User/test.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.046089 pose2sim-0.3.8/Pose2Sim/Demo/calib-2d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/calib-2d/Calib.qca.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.046089 pose2sim-0.3.8/Pose2Sim/Demo/opensim/
+-rw-r--r--   0 runner    (1001) docker     (123)   127289 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Balancing_for_IK.trc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.066089 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)    87711 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/bofoot.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/capitate_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/capitate_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    29750 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv1sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv2sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv3sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv4sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv5sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv6sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv7.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/femur_l.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/femur_r.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/fibula_l.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/fibula_r.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    97470 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/foot.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hamate_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hamate_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)   137969 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hat_jaw.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)   737930 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hat_ribs_scap.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)   315678 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hat_skull.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    37639 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/humerus_lv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    37639 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/humerus_rv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_medial_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_medial_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-07-31 18:36:25.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    88317 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/l_bofoot.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    97518 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/l_foot.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/l_patella.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/l_pelvis.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_medial_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_medial_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar1.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar2.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar3.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar4.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar5.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lunate_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lunate_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal1_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    32726 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal1_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    24962 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal2_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    24966 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal2_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal3_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    35418 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal3_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal4_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal4_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    42678 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal5_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    42670 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal5_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_medial_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_medial_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/pisiform_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/pisiform_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/r_patella.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/r_pelvis.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/radius_lv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/radius_rv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_medial_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_medial_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/sacrum.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/scaphoid_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/scaphoid_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    51083 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/talus_lv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    51083 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/talus_rv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic10_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic11_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic12_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic1_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic2_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic3_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic4_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic5_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic6_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic7_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic8_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic9_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thumb_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thumb_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/tibia_l.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/tibia_r.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/trapezium_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/trapezium_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/trapezoid_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/trapezoid_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/triquetrum_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/triquetrum_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ulna_lv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ulna_rv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   453333 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim
+-rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    32333 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/opensim/Standing_for_Scaling.trc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.042089 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.082089 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0000.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0003.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0004.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0005.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0006.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0007.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0008.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0009.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0010.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0011.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0012.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0013.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0014.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0015.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0016.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0017.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0018.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0019.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0020.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0021.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0022.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0023.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0024.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0025.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0026.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0027.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0028.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0029.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0030.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0031.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0032.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0033.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0034.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0035.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0036.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0037.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0038.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0039.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0040.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0041.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0042.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0043.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0044.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0045.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0046.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0047.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0048.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0049.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0050.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0051.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0052.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0053.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0054.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0055.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0056.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0057.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0058.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0059.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0060.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0061.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0062.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0063.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0064.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0065.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0066.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0067.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0068.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0069.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0070.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0071.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0072.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0073.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0074.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0075.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0076.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0077.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0078.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0079.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0080.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0081.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0082.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0083.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0084.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0085.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0086.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0087.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0088.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0089.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0090.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0091.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0092.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0093.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0094.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0095.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0096.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0097.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0098.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0099.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.094089 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0000.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0003.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0004.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0005.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0006.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0007.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0008.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0009.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0010.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0011.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0012.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0013.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0014.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0015.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0016.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0017.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0018.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0019.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0020.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0021.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0022.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0023.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0024.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0025.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0026.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0027.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0028.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0029.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0030.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0031.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0032.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0033.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0034.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0035.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0036.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0037.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0038.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0039.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0040.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0041.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0042.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0043.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0044.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0045.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0046.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0047.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0048.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0049.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0050.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0051.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0052.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0053.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0054.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0055.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0056.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0057.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0058.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0059.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0060.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0061.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0062.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0063.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0064.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0065.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0066.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0067.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0068.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0069.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0070.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0071.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0072.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0073.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0074.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0075.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0076.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0077.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0078.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0079.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0080.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0081.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0082.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0083.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0084.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0085.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0086.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0087.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0088.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0089.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0090.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0091.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0092.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0093.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0094.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0095.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0096.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0097.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0098.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0099.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.110089 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0000.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0002.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0003.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0004.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0005.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0006.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0007.json
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0008.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0009.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0010.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0011.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0012.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0013.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0014.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0015.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0016.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0017.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0018.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0019.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0020.json
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0021.json
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0022.json
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0023.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0024.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0025.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0026.json
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0027.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0028.json
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0029.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0030.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0031.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0032.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0033.json
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0034.json
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0035.json
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0036.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0037.json
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0038.json
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0039.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0040.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0041.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0042.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0043.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0044.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0045.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0046.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0047.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0048.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0049.json
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0050.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0051.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0052.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0053.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0054.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0055.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0056.json
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0057.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0058.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0059.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0060.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0061.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0062.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0063.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0064.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0065.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0066.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0067.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0068.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0069.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0070.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0071.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0072.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0073.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0074.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0075.json
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0076.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0077.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0078.json
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0079.json
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0080.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0081.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0082.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0083.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0084.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0085.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0086.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0087.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0088.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0089.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0090.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0091.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0092.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0093.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0094.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0095.json
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0096.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0097.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0098.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0099.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.126089 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0000.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0002.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0003.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0004.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0005.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0006.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0007.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0008.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0009.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0010.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0011.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0012.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0013.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0014.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0015.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0016.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0017.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0018.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0019.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0020.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0021.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0022.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0023.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0024.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0025.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0026.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0027.json
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0028.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0029.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0030.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0031.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0032.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0033.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0034.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0035.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0036.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0037.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0038.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0039.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0040.json
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0041.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0042.json
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0043.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0044.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0045.json
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0046.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0047.json
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0048.json
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0049.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0050.json
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0051.json
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0052.json
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0053.json
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0054.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0055.json
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0056.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0057.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0058.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0059.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0060.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0061.json
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0062.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0063.json
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0064.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0065.json
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0066.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0067.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0068.json
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0069.json
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0070.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0071.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0072.json
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0073.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0074.json
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0075.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0076.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0077.json
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0078.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0079.json
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0080.json
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0081.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0082.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0083.json
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0084.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0085.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0086.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0087.json
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0088.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0089.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0090.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0091.json
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0092.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0093.json
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0094.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0095.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0096.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0097.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0098.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Demo/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.042089 pose2sim-0.3.8/Pose2Sim/Empty_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.126089 pose2sim-0.3.8/Pose2Sim/Empty_project/User/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/User/Config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.134090 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.162090 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)    87711 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    29750 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv3sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv4sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv5sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv6sm.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv7.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/femur_l.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/femur_r.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/fibula_l.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/fibula_r.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    97470 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/foot.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hamate_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hamate_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)   137969 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hat_jaw.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)   737930 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hat_ribs_scap.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)   315678 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hat_skull.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    37639 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/humerus_lv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    37639 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/humerus_rv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_medial_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_medial_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    88317 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/l_bofoot.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    97518 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/l_foot.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/l_patella.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/l_pelvis.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_medial_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_medial_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar1.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar2.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar3.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar4.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar5.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lunate_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lunate_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    32726 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    24962 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    24966 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    35418 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    42678 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    42670 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/pisiform_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/pisiform_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/r_patella.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/r_pelvis.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/radius_lv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/radius_rv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/sacrum.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    51083 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/talus_lv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    51083 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/talus_rv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic10_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic11_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic12_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic1_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic2_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic3_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic4_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic5_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic6_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic7_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic8_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic9_s.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/tibia_l.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/tibia_r.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/trapezium_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/trapezium_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_lvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_rvs.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ulna_lv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ulna_rv.vtp
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco18.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   454633 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim
+-rw-r--r--   0 runner    (1001) docker     (123)   456161 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim
+-rw-r--r--   0 runner    (1001) docker     (123)   458489 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim
+-rw-r--r--   0 runner    (1001) docker     (123)   453368 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim
+-rw-r--r--   0 runner    (1001) docker     (123)   456144 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim
+-rw-r--r--   0 runner    (1001) docker     (123)   453673 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco18.osim
+-rw-r--r--   0 runner    (1001) docker     (123)   453792 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim
+-rw-r--r--   0 runner    (1001) docker     (123)   456561 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim
+-rw-r--r--   0 runner    (1001) docker     (123)    24023 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30222 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30507 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco18.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Pose2Sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.162090 pose2sim-0.3.8/Pose2Sim/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/AlphaPose_to_OpenPose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/DLC_to_OpenPose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/c3d_to_trc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/calib_from_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/calib_qca_to_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/calib_toml_to_qca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/calib_toml_to_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/calib_yml_to_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/json_display_with_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/json_display_without_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/trc_Zup_to_Yup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/trc_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/trc_desample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/trc_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/trc_gaitevents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/Utilities/trc_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/calibrate_cams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/filter_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/track_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-07-31 18:36:26.000000 pose2sim-0.3.8/Pose2Sim/triangulate_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30322 2023-07-31 18:36:26.000000 pose2sim-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:36:42.166090 pose2sim-0.3.8/pose2sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-07-31 18:36:41.000000 pose2sim-0.3.8/pose2sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33119 2023-07-31 18:36:42.000000 pose2sim-0.3.8/pose2sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:36:41.000000 pose2sim-0.3.8/pose2sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:36:41.000000 pose2sim-0.3.8/pose2sim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-31 18:36:41.000000 pose2sim-0.3.8/pose2sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 18:36:41.000000 pose2sim-0.3.8/pose2sim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-31 18:36:26.000000 pose2sim-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-31 18:36:42.166090 pose2sim-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 18:36:26.000000 pose2sim-0.3.8/setup.py
```

### Comparing `pose2sim-0.3.7/LICENSE` & `pose2sim-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/PKG-INFO` & `pose2sim-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pose2sim
-Version: 0.3.7
+Version: 0.3.8
 Summary: Perform a markerless kinematic analysis from multiple calibrated views as a unified workflow from an OpenPose input to an OpenSim result.
 Home-page: https://github.com/perfanalytics/pose2sim
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/perfanalytics/pose2sim/issues
 Keywords: markerless,kinematics,OpenPose,OpenSim,3D human pose,biomechanics
@@ -250,21 +250,21 @@
        └──Config.toml
    </pre>
 </details>
 
 ### Camera calibration
 > _**Calibrate your cameras.**_
 
-> - Note 1: Calibration is tricky. I plan to make it more user-friendly, but in the meantime, you can refer to [this issue](https://github.com/perfanalytics/pose2sim/issues/23#issuecomment-1493291952) if you struggle.
+> - Note 1: Calibration is tricky. I plan to make it more user-friendly, but in the meantime, you can refer to [this issue](https://github.com/perfanalytics/pose2sim/issues/18) if you struggle.
 > - Note 2: Cameras need to be synchronized. If they are not natively, you can use [this script](https://github.com/perfanalytics/pose2sim/blob/draft/Pose2Sim/Utilities/synchronize_cams.py).
 
 
 1. If you already have a calibration file (.qca.txt from Qualisys for example):
 - copy it in the `calib-2d` folder
-- set [calibration] type to 'qca' in your `Config.toml` file.
+- set [calibration] type to 'qca' in your `Config.toml` file. Change `binning_factor` to 2 if you film in 540p
 
 or
 
 2. If you have taken pictures or videos of a checkerboard with your cameras:
 - create a folder for each camera in your `calib-2d` folder,
 - copy there the images or videos of the checkerboard
 - set [calibration] type to 'checkerboard' in your `Config.toml` file, and adjust other parameters.
```

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/User/Config.toml` & `pose2sim-0.3.8/Pose2Sim/Demo/User/Config.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 ## POSE2SIM PROJECT PARAMETERS                                               ##
 ###############################################################################
 
 # Configure your project parameters here
 
 [project]
-project_dir = '' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
+project_dir = 'D:\softs\github_david\pose2sim\Pose2Sim\Demo' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
 frame_range = [] #For example [10,300], or [] for all frames
 frame_rate = 60 #Hz
 
 rawImg_folder_name = 'raw-2d'
 calib_folder_name = 'calib-2d'
 pose_folder_name = 'pose-2d'
 pose_json_folder_extension = 'json'
@@ -21,17 +21,19 @@
 [pose-2d]
 pose_model = 'BODY_25B' #CUSTOM, BODY_25B, BODY_25, BODY_135, BLAZEPOSE, 
 # HALPE_26, HALPE_68, HALPE_136, COCO_133, COCO, MPII are available,
 # from DeepLabCut, OpenPose, MediaPipe BlazePose, and AlphaPose
 # See Pose2Sim\skeleton.py for their skeleton hierarchy
 
 [calibration]
-type = 'qca' # 'qca', 'checkerboard', 'arucoboard', or 'charucoboard'
+type = 'vicon' # 'qca', 'vicon', 'checkerboard', 'arucoboard', or 'charucoboard'
    [calibration.qca]
-   binning_factor = 1 # Usually 1
+   binning_factor = 1 # Usually 1, except when filming in 540p where it usually is 2
+
+   [calibration.vicon]
 
    [calibration.checkerboard]
    corners_nb = [7,12] # [H,W] rather than [w,h]
    square_size = 80 # mm # [h,w] if square is actually a rectangle
    frame_for_origin = -1 # starting from zero. -1 if board is at origin on last frame
    # /!\ Beware that corners must be detected on all view at frame_for_origin, or else 
    # extrinsic parameters will be wrong. Set show_corner_detection to true to check it.
```

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/User/test.toml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/User/Config.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ## POSE2SIM PROJECT PARAMETERS                                               ##
 ###############################################################################
 
 # Configure your project parameters here
 
 [project]
 project_dir = '' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
-frame_range = [0,10] #For example [10,300], or [] for all frames
+frame_range = [] #For example [10,300], or [] for all frames
 frame_rate = 60 #Hz
 
 rawImg_folder_name = 'raw-2d'
 calib_folder_name = 'calib-2d'
 pose_folder_name = 'pose-2d'
 pose_json_folder_extension = 'json'
 pose_img_folder_extension = 'img'
@@ -23,15 +23,15 @@
 # HALPE_26, HALPE_68, HALPE_136, COCO_133, COCO, MPII are available,
 # from DeepLabCut, OpenPose, MediaPipe BlazePose, and AlphaPose
 # See Pose2Sim\skeleton.py for their skeleton hierarchy
 
 [calibration]
 type = 'qca' # 'qca', 'checkerboard', 'arucoboard', or 'charucoboard'
    [calibration.qca]
-   binning_factor = 1 # Usually 1
+   binning_factor = 1 # Usually 1, except when filming in 540p where it usually is 2
 
    [calibration.checkerboard]
    corners_nb = [7,12] # [H,W] rather than [w,h]
    square_size = 80 # mm # [h,w] if square is actually a rectangle
    frame_for_origin = -1 # starting from zero. -1 if board is at origin on last frame
    # /!\ Beware that corners must be detected on all view at frame_for_origin, or else 
    # extrinsic parameters will be wrong. Set show_corner_detection to true to check it.
@@ -53,15 +53,15 @@
 interpolation = 'cubic' #linear, slinear, quadratic, cubic, or none
 # 'none' if you don't want to interpolate missing points
 interp_if_gap_smaller_than = 10 # do not interpolate bigger gaps
 show_interp_indices = true # true or false (lowercase). For each keypoint, return the frames that need to be interpolated
 
 [3d-filtering]
 type = 'butterworth' # butterworth, butterworth_on_speed, gaussian, LOESS, median
-display_figures = false # true or false (lowercase)
+display_figures = true # true or false (lowercase)
 
    [3d-filtering.butterworth]
    type = 'low'
    order = 4 
    cut_off_frequency = 6 # Hz
    [3d-filtering.butterworth_on_speed]
    type = 'low'
```

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/calib-2d/Calib.qca.txt` & `pose2sim-0.3.8/Pose2Sim/Demo/calib-2d/Calib.qca.txt`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Balancing_for_IK.trc` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Balancing_for_IK.trc`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/bofoot.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/bofoot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/capitate_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/capitate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/capitate_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/capitate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv1sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv1sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv2sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv2sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv3sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv3sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv4sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv4sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv5sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv5sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv6sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv6sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/cerv7.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/cerv7.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/femur_l.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/femur_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/femur_r.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/femur_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/fibula_l.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/fibula_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/fibula_r.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/fibula_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/foot.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/foot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hamate_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hamate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hamate_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hamate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hat_jaw.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hat_jaw.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hat_ribs_scap.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hat_ribs_scap.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/hat_skull.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/hat_skull.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/humerus_lv.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/humerus_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/humerus_rv.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/humerus_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_medial_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_medial_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/index_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/index_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/l_bofoot.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/l_bofoot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/l_foot.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/l_foot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/l_patella.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/l_patella.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/l_pelvis.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/l_pelvis.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_medial_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_medial_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/little_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/little_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar1.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar1.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar2.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar2.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar3.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar3.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar4.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar4.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lumbar5.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lumbar5.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lunate_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lunate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/lunate_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/lunate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal1_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal1_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal1_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal1_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal2_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal2_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal2_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal2_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal3_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal3_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal3_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal3_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal4_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal4_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal4_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal4_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal5_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal5_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/metacarpal5_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/metacarpal5_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_medial_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_medial_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/middle_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/middle_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/pisiform_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/pisiform_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/pisiform_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/pisiform_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/r_patella.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/r_patella.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/r_pelvis.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/r_pelvis.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/radius_lv.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/radius_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/radius_rv.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/radius_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_medial_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_medial_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ring_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ring_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/sacrum.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/sacrum.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/scaphoid_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/scaphoid_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/scaphoid_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/scaphoid_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/talus_lv.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/talus_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/talus_rv.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/talus_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic10_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic10_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic11_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic11_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic12_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic12_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic1_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic1_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic2_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic2_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic3_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic3_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic4_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic4_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic5_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic5_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic6_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic6_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic7_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic7_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic8_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic8_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thoracic9_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thoracic9_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thumb_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thumb_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thumb_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thumb_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/tibia_l.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/tibia_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/tibia_r.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/tibia_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/trapezium_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/trapezium_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/trapezium_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/trapezium_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/trapezoid_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/trapezoid_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/trapezoid_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/trapezoid_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/triquetrum_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/triquetrum_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/triquetrum_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/triquetrum_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ulna_lv.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ulna_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Geometry/ulna_rv.vtp` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Geometry/ulna_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/opensim/Standing_for_Scaling.trc` & `pose2sim-0.3.8/Pose2Sim/Demo/opensim/Standing_for_Scaling.trc`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0000.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0000.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0001.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0001.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0002.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0002.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0003.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0003.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0004.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0004.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0005.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0005.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0006.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0006.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0007.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0007.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0008.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0008.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0009.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0009.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0010.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0010.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0011.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0011.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0012.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0012.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0013.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0013.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0014.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0014.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0015.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0015.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0016.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0016.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0017.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0017.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0018.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0018.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0019.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0019.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0020.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0020.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0021.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0021.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0022.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0022.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0023.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0023.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0024.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0024.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0025.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0025.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0026.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0026.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0027.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0027.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0028.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0028.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0029.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0029.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0030.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0030.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0031.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0031.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0032.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0032.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0033.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0033.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0034.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0034.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0035.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0035.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0036.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0036.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0037.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0037.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0038.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0038.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0039.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0039.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0040.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0040.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0041.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0041.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0042.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0042.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0043.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0043.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0044.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0044.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0045.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0045.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0046.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0046.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0047.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0047.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0048.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0048.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0049.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0049.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0050.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0050.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0051.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0051.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0052.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0052.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0053.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0053.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0054.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0054.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0055.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0055.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0056.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0056.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0057.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0057.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0058.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0058.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0059.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0059.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0060.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0060.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0061.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0061.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0062.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0062.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0063.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0063.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0064.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0064.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0065.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0065.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0066.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0066.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0067.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0067.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0068.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0068.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0069.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0069.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0070.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0070.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0071.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0071.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0072.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0072.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0073.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0073.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0074.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0074.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0075.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0075.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0076.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0076.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0077.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0077.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0078.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0078.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0079.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0079.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0080.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0080.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0081.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0081.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0082.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0082.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0083.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0083.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0084.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0084.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0085.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0085.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0086.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0086.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0087.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0087.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0088.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0088.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0089.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0089.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0090.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0090.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0091.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0091.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0092.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0092.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0093.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0093.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0094.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0094.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0095.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0095.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0096.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0096.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0097.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0097.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0098.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0098.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0099.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0099.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0000.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0000.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0001.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0001.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0002.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0002.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0003.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0003.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0004.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0004.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0005.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0005.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0006.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0006.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0007.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0007.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0008.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0008.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0009.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0009.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0010.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0010.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0011.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0011.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0012.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0012.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0013.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0013.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0014.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0014.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0015.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0015.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0016.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0016.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0017.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0017.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0018.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0018.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0019.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0019.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0020.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0020.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0021.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0021.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0022.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0022.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0023.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0023.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0024.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0024.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0025.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0025.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0026.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0026.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0027.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0027.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0028.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0028.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0029.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0029.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0030.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0030.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0031.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0031.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0032.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0032.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0033.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0033.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0034.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0034.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0035.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0035.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0036.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0036.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0037.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0037.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0038.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0038.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0039.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0039.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0040.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0040.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0041.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0041.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0042.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0042.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0043.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0043.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0044.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0044.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0045.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0045.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0046.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0046.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0047.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0047.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0048.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0048.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0049.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0049.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0050.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0050.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0051.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0051.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0052.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0052.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0053.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0053.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0054.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0054.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0055.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0055.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0056.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0056.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0057.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0057.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0058.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0058.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0059.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0059.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0060.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0060.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0061.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0061.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0062.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0062.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0063.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0063.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0064.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0064.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0065.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0065.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0066.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0066.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0067.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0067.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0068.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0068.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0069.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0069.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0070.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0070.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0071.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0071.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0072.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0072.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0073.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0073.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0074.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0074.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0075.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0075.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0076.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0076.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0077.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0077.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0078.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0078.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0079.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0079.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0080.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0080.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0081.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0081.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0082.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0082.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0083.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0083.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0084.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0084.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0085.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0085.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0086.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0086.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0087.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0087.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0088.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0088.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0089.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0089.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0090.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0090.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0091.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0091.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0092.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0092.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0093.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0093.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0094.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0094.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0095.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0095.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0096.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0096.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0097.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0097.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0098.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0098.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0099.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0099.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0000.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0000.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0001.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0001.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0002.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0002.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0003.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0003.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0004.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0004.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0005.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0005.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0006.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0006.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0007.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0007.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0008.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0008.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0009.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0009.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0010.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0010.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0011.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0011.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0012.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0012.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0013.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0013.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0014.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0014.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0015.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0015.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0016.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0016.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0017.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0017.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0018.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0018.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0019.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0019.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0020.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0020.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0021.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0021.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0022.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0022.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0023.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0023.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0024.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0024.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0025.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0025.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0026.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0026.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0027.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0027.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0028.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0028.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0029.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0029.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0030.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0030.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0031.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0031.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0032.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0032.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0033.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0033.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0034.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0034.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0035.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0035.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0036.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0036.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0037.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0037.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0038.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0038.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0039.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0039.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0040.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0040.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0041.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0041.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0042.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0042.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0043.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0043.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0044.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0044.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0045.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0045.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0046.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0046.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0047.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0047.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0048.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0048.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0049.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0049.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0050.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0050.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0051.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0051.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0052.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0052.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0053.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0053.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0054.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0054.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0055.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0055.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0056.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0056.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0057.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0057.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0058.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0058.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0059.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0059.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0060.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0060.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0061.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0061.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0062.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0062.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0063.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0063.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0064.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0064.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0065.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0065.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0066.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0066.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0067.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0067.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0068.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0068.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0069.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0069.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0070.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0070.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0071.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0071.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0072.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0072.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0073.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0073.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0074.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0074.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0075.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0075.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0076.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0076.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0077.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0077.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0078.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0078.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0079.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0079.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0080.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0080.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0081.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0081.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0082.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0082.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0083.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0083.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0084.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0084.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0085.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0085.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0086.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0086.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0087.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0087.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0088.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0088.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0089.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0089.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0090.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0090.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0091.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0091.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0092.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0092.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0093.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0093.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0094.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0094.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0095.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0095.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0096.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0096.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0097.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0097.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0098.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0098.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0099.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0099.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0000.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0000.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0001.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0001.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0002.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0002.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0003.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0003.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0004.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0004.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0005.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0005.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0006.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0006.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0007.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0007.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0008.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0008.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0009.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0009.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0010.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0010.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0011.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0011.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0012.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0012.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0013.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0013.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0014.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0014.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0015.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0015.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0016.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0016.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0017.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0017.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0018.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0018.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0019.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0019.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0020.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0020.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0021.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0021.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0022.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0022.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0023.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0023.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0024.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0024.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0025.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0025.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0026.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0026.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0027.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0027.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0028.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0028.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0029.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0029.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0030.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0030.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0031.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0031.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0032.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0032.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0033.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0033.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0034.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0034.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0035.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0035.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0036.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0036.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0037.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0037.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0038.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0038.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0039.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0039.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0040.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0040.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0041.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0041.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0042.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0042.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0043.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0043.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0044.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0044.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0045.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0045.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0046.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0046.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0047.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0047.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0048.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0048.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0049.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0049.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0050.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0050.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0051.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0051.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0052.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0052.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0053.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0053.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0054.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0054.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0055.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0055.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0056.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0056.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0057.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0057.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0058.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0058.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0059.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0059.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0060.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0060.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0061.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0061.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0062.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0062.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0063.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0063.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0064.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0064.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0065.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0065.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0066.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0066.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0067.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0067.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0068.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0068.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0069.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0069.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0070.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0070.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0071.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0071.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0072.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0072.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0073.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0073.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0074.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0074.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0075.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0075.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0076.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0076.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0077.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0077.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0078.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0078.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0079.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0079.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0080.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0080.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0081.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0081.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0082.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0082.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0083.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0083.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0084.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0084.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0085.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0085.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0086.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0086.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0087.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0087.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0088.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0088.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0089.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0089.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0090.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0090.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0091.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0091.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0092.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0092.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0093.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0093.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0094.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0094.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0095.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0095.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0096.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0096.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0097.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0097.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0098.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0098.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json` & `pose2sim-0.3.8/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/User/Config.toml` & `pose2sim-0.3.8/Pose2Sim/Demo/User/test.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ## POSE2SIM PROJECT PARAMETERS                                               ##
 ###############################################################################
 
 # Configure your project parameters here
 
 [project]
 project_dir = '' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
-frame_range = [] #For example [10,300], or [] for all frames
+frame_range = [0,10] #For example [10,300], or [] for all frames
 frame_rate = 60 #Hz
 
 rawImg_folder_name = 'raw-2d'
 calib_folder_name = 'calib-2d'
 pose_folder_name = 'pose-2d'
 pose_json_folder_extension = 'json'
 pose_img_folder_extension = 'img'
@@ -23,15 +23,15 @@
 # HALPE_26, HALPE_68, HALPE_136, COCO_133, COCO, MPII are available,
 # from DeepLabCut, OpenPose, MediaPipe BlazePose, and AlphaPose
 # See Pose2Sim\skeleton.py for their skeleton hierarchy
 
 [calibration]
 type = 'qca' # 'qca', 'checkerboard', 'arucoboard', or 'charucoboard'
    [calibration.qca]
-   binning_factor = 1 # Usually 1
+   binning_factor = 1 # Usually 1, except when filming in 540p where it usually is 2
 
    [calibration.checkerboard]
    corners_nb = [7,12] # [H,W] rather than [w,h]
    square_size = 80 # mm # [h,w] if square is actually a rectangle
    frame_for_origin = -1 # starting from zero. -1 if board is at origin on last frame
    # /!\ Beware that corners must be detected on all view at frame_for_origin, or else 
    # extrinsic parameters will be wrong. Set show_corner_detection to true to check it.
@@ -53,15 +53,15 @@
 interpolation = 'cubic' #linear, slinear, quadratic, cubic, or none
 # 'none' if you don't want to interpolate missing points
 interp_if_gap_smaller_than = 10 # do not interpolate bigger gaps
 show_interp_indices = true # true or false (lowercase). For each keypoint, return the frames that need to be interpolated
 
 [3d-filtering]
 type = 'butterworth' # butterworth, butterworth_on_speed, gaussian, LOESS, median
-display_figures = true # true or false (lowercase)
+display_figures = false # true or false (lowercase)
 
    [3d-filtering.butterworth]
    type = 'low'
    order = 4 
    cut_off_frequency = 6 # Hz
    [3d-filtering.butterworth_on_speed]
    type = 'low'
```

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv3sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv3sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv4sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv4sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv5sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv5sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv6sm.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv6sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/cerv7.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/cerv7.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/femur_l.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/femur_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/femur_r.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/femur_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/fibula_l.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/fibula_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/fibula_r.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/fibula_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/foot.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/foot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hamate_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hamate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hamate_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hamate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hat_jaw.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hat_jaw.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hat_ribs_scap.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hat_ribs_scap.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/hat_skull.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/hat_skull.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/humerus_lv.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/humerus_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/humerus_rv.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/humerus_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_medial_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_medial_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/l_bofoot.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/l_bofoot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/l_foot.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/l_foot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/l_patella.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/l_patella.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/l_pelvis.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/l_pelvis.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_medial_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_medial_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar1.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar1.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar2.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar2.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar3.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar3.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar4.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar4.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lumbar5.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lumbar5.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lunate_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lunate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/lunate_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/lunate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/pisiform_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/pisiform_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/pisiform_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/pisiform_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/r_patella.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/r_patella.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/r_pelvis.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/r_pelvis.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/radius_lv.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/radius_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/radius_rv.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/radius_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/sacrum.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/sacrum.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/talus_lv.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/talus_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/talus_rv.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/talus_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic10_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic10_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic11_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic11_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic12_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic12_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic1_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic1_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic2_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic2_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic3_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic3_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic4_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic4_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic5_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic5_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic6_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic6_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic7_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic7_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic8_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic8_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thoracic9_s.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thoracic9_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/tibia_l.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/tibia_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/tibia_r.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/tibia_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/trapezium_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/trapezium_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/trapezium_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/trapezium_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_lvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_rvs.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ulna_lv.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ulna_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Geometry/ulna_rv.vtp` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Geometry/ulna_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco18.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco18.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco18.osim` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco18.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco18.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco18.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml` & `pose2sim-0.3.8/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Pose2Sim.py` & `pose2sim-0.3.8/Pose2Sim/Pose2Sim.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/AlphaPose_to_OpenPose.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/AlphaPose_to_OpenPose.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/Blazepose_runsave.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/Blazepose_runsave.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/DLC_to_OpenPose.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/DLC_to_OpenPose.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/c3d_to_trc.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/c3d_to_trc.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/calib_from_checkerboard.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/calib_from_checkerboard.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/calib_qca_to_toml.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/calib_qca_to_toml.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/calib_toml_to_qca.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/calib_toml_to_qca.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/calib_toml_to_yml.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/calib_toml_to_yml.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/calib_yml_to_toml.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/calib_yml_to_toml.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/json_display_with_img.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/json_display_with_img.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/json_display_without_img.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/json_display_without_img.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/trc_Zup_to_Yup.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/trc_Zup_to_Yup.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/trc_combine.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/trc_combine.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/trc_desample.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/trc_desample.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/trc_filter.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/trc_filter.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/trc_gaitevents.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/trc_gaitevents.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/Utilities/trc_plot.py` & `pose2sim-0.3.8/Pose2Sim/Utilities/trc_plot.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/calibrate_cams.py` & `pose2sim-0.3.8/Pose2Sim/calibrate_cams.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import numpy as np
 import cv2
 import glob
 import toml
 import re
 from lxml import etree
 
-from Pose2Sim.common import RT_qca2cv, rotate_cam, euclidean_distance, natural_sort
+from Pose2Sim.common import RT_qca2cv, rotate_cam, quat2mat, euclidean_distance, natural_sort
 
 
 ## AUTHORSHIP INFORMATION
 __author__ = "David Pagnon"
 __copyright__ = "Copyright 2021, Pose2Sim"
 __credits__ = ["David Pagnon"]
 __license__ = "BSD 3-Clause License"
@@ -124,16 +124,16 @@
         ret += [float(tag.attrib.get('avg-residual'))/1000]
         C += [tag.attrib.get('serial')]
         if tag.attrib.get('model') in ('Miqus Video', 'Miqus Video UnderWater', 'none'):
             vid_id += [i]
     
     # Image size
     for tag in root.findall('cameras/camera/fov_video'):
-        w = (float(tag.attrib.get('right')) - float(tag.attrib.get('left'))) /binning_factor
-        h = (float(tag.attrib.get('bottom')) - float(tag.attrib.get('top'))) /binning_factor
+        w = (float(tag.attrib.get('right')) - float(tag.attrib.get('left')) +1) /binning_factor
+        h = (float(tag.attrib.get('bottom')) - float(tag.attrib.get('top')) +1) /binning_factor
         S += [[w, h]]
     
     # Intrinsic parameters: distorsion and intrinsic matrix
     for i, tag in enumerate(root.findall('cameras/camera/intrinsic')):
         k1 = float(tag.get('radialDistortion1'))/64/binning_factor
         k2 = float(tag.get('radialDistortion2'))/64/binning_factor
         p1 = float(tag.get('tangentalDistortion1'))/64/binning_factor
@@ -178,14 +178,143 @@
     K = [K[c] for c in C_id]
     R = [R[c] for c in C_id]
     T = [T[c] for c in C_id]
    
     return ret, C, S, D, K, R, T
 
 
+def calib_optitrack_fun(config):
+    '''
+    Convert an Optitrack calibration file 
+
+    INPUTS:
+    - a Config.toml file
+
+    OUTPUTS:
+    - ret: residual reprojection error in _mm_: list of floats
+    - C: camera name: list of strings
+    - S: image size: list of list of floats
+    - D: distorsion: list of arrays of floats
+    - K: intrinsic parameters: list of 3x3 arrays of floats
+    - R: extrinsic rotation: list of arrays of floats
+    - T: extrinsic translation: list of arrays of floats
+
+    '''
+
+    pass
+
+
+def calib_vicon_fun(config):
+    '''
+    Convert a Vicon .xcp calibration file 
+    Converts from camera view to object view, 
+    and converts rotation with Rodrigues formula
+
+    INPUTS:
+    - file_to_convert_path: path of the .qca.text file to convert
+    - binning_factor: always 1 with Vicon calibration
+
+    OUTPUTS:
+    - ret: residual reprojection error in _mm_: list of floats
+    - C: camera name: list of strings
+    - S: image size: list of list of floats
+    - D: distorsion: list of arrays of floats
+    - K: intrinsic parameters: list of 3x3 arrays of floats
+    - R: extrinsic rotation: list of arrays of floats
+    - T: extrinsic translation: list of arrays of floats
+
+    '''
+   
+    project_dir = config.get('project').get('project_dir')
+    if project_dir == '': project_dir = os.getcwd()
+    calib_folder_name = config.get('project').get('calib_folder_name')
+    calib_dir = os.path.join(project_dir, calib_folder_name)
+    print(calib_dir)
+    vicon_path = glob.glob(os.path.join(calib_dir, '*.xcp'))[0]
+
+    ret, C, S, D, K, R, T = read_vicon(vicon_path)
+    
+    RT = [RT_qca2cv(r,t) for r, t in zip(R, T)]
+    R = [rt[0] for rt in RT]
+    T = [rt[1] for rt in RT]
+
+    R = [np.array(cv2.Rodrigues(r)[0]).flatten() for r in R]
+    T = np.array(T)
+    
+    return ret, C, S, D, K, R, T
+
+
+def read_vicon(vicon_path):
+    '''
+    Reads a Vicon .xcp calibration file 
+    Returns 6 lists of size N (N=number of cameras)
+    
+    INPUTS: 
+    - vicon_path: path to .xcp calibration file: string
+
+    OUTPUTS:
+    - ret: residual reprojection error in _mm_: list of floats
+    - C: camera name: list of strings
+    - S: image size: list of list of floats
+    - D: distorsion: list of arrays of floats
+    - K: intrinsic parameters: list of 3x3 arrays of floats
+    - R: extrinsic rotation: list of 3x3 arrays of floats
+    - T: extrinsic translation: list of arrays of floats
+    '''
+
+    root = etree.parse(vicon_path).getroot()
+    ret, C, S, D, K, R, T = [], [], [], [], [], [], []
+    vid_id = []
+    
+    # Camera name and image size
+    for i, tag in enumerate(root.findall('Camera')):
+        C += [tag.attrib.get('DEVICEID')]
+        S += [[float(t) for t in tag.attrib.get('SENSOR_SIZE').split()]]
+        ret += [float(tag.findall('KeyFrames/KeyFrame')[0].attrib.get('WORLD_ERROR'))]
+        # if tag.attrib.get('model') in ('Miqus Video', 'Miqus Video UnderWater', 'none'):
+        vid_id += [i]
+
+    # Intrinsic parameters: distorsion and intrinsic matrix
+    for cam_elem in root.findall('Camera'):
+        try:
+            dist = cam_elem.findall('KeyFrames/KeyFrame')[0].attrib.get('VICON_RADIAL2').split()[3:5]
+        except:
+            dist = cam_elem.findall('KeyFrames/KeyFrame')[0].attrib.get('VICON_RADIAL').split()
+        D += [[float(d) for d in dist] + [0.0, 0.0]]
+
+        fu = float(cam_elem.findall('KeyFrames/KeyFrame')[0].attrib.get('FOCAL_LENGTH'))
+        fv = fu / float(cam_elem.attrib.get('PIXEL_ASPECT_RATIO'))
+        cam_center = cam_elem.findall('KeyFrames/KeyFrame')[0].attrib.get('PRINCIPAL_POINT').split()
+        cu, cv = [float(c) for c in cam_center]
+        K += [np.array([fu, 0., cu, 0., fv, cv, 0., 0., 1.]).reshape(3,3)]
+
+    # Extrinsic parameters: rotation matrix and translation vector
+    for cam_elem in root.findall('Camera'):
+        rot = cam_elem.findall('KeyFrames/KeyFrame')[0].attrib.get('ORIENTATION').split()
+        R_quat = [float(r) for r in rot]
+        R_mat = quat2mat(R_quat, scalar_idx=3)
+        R += [R_mat]
+
+        trans = cam_elem.findall('KeyFrames/KeyFrame')[0].attrib.get('POSITION').split()
+        T += [[float(t)/1000 for t in trans]]
+   
+    # Cameras names by natural order
+    C_vid = [C[v] for v in vid_id]
+    C_vid_id = [C_vid.index(c) for c in natural_sort(C_vid)]
+    C_id = [vid_id[c] for c in C_vid_id]
+    C = [C[c] for c in C_id]
+    S = [S[c] for c in C_id]
+    D = [D[c] for c in C_id]
+    K = [K[c] for c in C_id]
+    R = [R[c] for c in C_id]
+    T = [T[c] for c in C_id]
+   
+    return ret, C, S, D, K, R, T
+
+
 def findCorners(img, corners_nb, criteria, show):
     '''
     Find corners _of internal squares_ in the checkerboard
 
     INPUTS:
     - img: image read by opencv
     - corners_nb: [H, W] internal corners in checkerboard: list of two integers [9,6]
@@ -210,14 +339,15 @@
             cv2.waitKey(0)
         return imgp
     else:
         if show:
             print('Corners not found.')
         return
 
+
 def calib_checkerboard_fun(config):
     '''
     Calibrates from images or videos of a checkerboard
 
     INPUTS:
     - a Config.toml file
 
@@ -362,14 +492,15 @@
     - T: extrinsic translation: list of arrays of floats
     '''
 
     # Map calib function
     calib_type = config.get('calibration').get('type')
     calib_mapping = {
         'qca': calib_qca_fun,
+        'vicon': calib_vicon_fun,
         'checkerboard': calib_checkerboard_fun
         }
     calib_fun = calib_mapping[calib_type]
 
     # Calibrate
     ret, C, S, D, K, R, T = calib_fun(config)
     return ret, C, S, D, K, R, T
@@ -389,14 +520,17 @@
     for c, cam in enumerate(calib.keys()):
         if cam != 'metadata':
             fm = calib[cam]['matrix'][0][0]
             Dm = euclidean_distance(calib[cam]['translation'], [0,0,0])
             if calib_type=='qca':
                 ret_m.append( np.around(ret[c]*1000, decimals=3) )
                 ret_px.append( np.around(ret[c] / Dm * fm, decimals=3) )
+            if calib_type=='vicon':
+                ret_m.append( np.around(ret[c], decimals=3) )
+                ret_px.append( np.around(ret[c] / (Dm*1000) * fm, decimals=3) )
             elif calib_type=='checkerboard':
                 ret_px.append( np.around(ret[c], decimals=3) )
                 ret_m.append( np.around(ret[c]*1000 * Dm / fm, decimals=3) )
 
     logging.info(f'\n--> Residual (RMS) calibration errors for each camera are respectively {ret_px} px, which corresponds to {ret_m} mm.\n')
     logging.info(f'Calibration file is stored at {calib_path}.')
 
@@ -417,14 +551,17 @@
 
     # Read config
     project_dir = config.get('project').get('project_dir')
     if project_dir == '': project_dir = os.getcwd()
     calib_folder_name = config.get('project').get('calib_folder_name')
     calib_dir = os.path.join(project_dir, calib_folder_name)
     calib_type = config.get('calibration').get('type')
+    if calib_type=='vicon':
+        vicon_path = glob.glob(os.path.join(calib_dir, '*.xcp'))[0]
+        calib_path = vicon_path.replace('.xcp', '_xcp.toml')
     if calib_type=='qca':
         qca_path = glob.glob(os.path.join(calib_dir, '*.qca.txt'))[0]
         calib_path = qca_path.replace('.qca.txt', '_qca.toml')
     elif calib_type=='checkerboard':
         calib_path = os.path.join(calib_dir, 'Calib_checkerboard.toml')
     
     # Calibrate
```

### Comparing `pose2sim-0.3.7/Pose2Sim/common.py` & `pose2sim-0.3.8/Pose2Sim/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -134,14 +134,46 @@
     dist = q2 - q1
     
     euc_dist = np.sqrt(np.sum( [d**2 for d in dist]))
     
     return euc_dist
 
 
+def quat2mat(quat, scalar_idx=0):
+    '''
+    Converts quaternion to rotation matrix
+
+    INPUT:
+    - quat: quaternion. np.array of size 4
+    - scalar_idx: index of scalar part of quaternion. Default: 0, sometimes 3
+
+    OUTPUT:
+    - mat: 3x3 rotation matrix
+    '''
+
+    if scalar_idx == 0:
+        w, qx, qy, qz = np.array(quat)
+    elif scalar_idx == 3:
+        qx, qy, qz, w = np.array(quat)
+    else:
+        print('Error: scalar_idx should be 0 or 3')
+
+    r11 = 1 - 2 * (qy**2 + qz**2)
+    r12 = 2 * (qx*qy - qz*w)
+    r13 = 2 * (qx*qz + qy*w)
+    r21 = 2 * (qx*qy + qz*w)
+    r22 = 1 - 2 * (qx**2 + qz**2)
+    r23 = 2 * (qy*qz - qx*w)
+    r31 = 2 * (qx*qz - qy*w)
+    r32 = 2 * (qy*qz + qx*w)
+    r33 = 1 - 2 * (qx**2 + qy**2)
+    mat = np.array([r11, r12, r13, r21, r22, r23, r31, r32, r33]).reshape(3,3).T
+
+    return mat
+	
 def RT_qca2cv(r, t):
     '''
     Converts rotation R and translation T 
     from Qualisys object centered perspective
     to OpenCV camera centered perspective
     and inversely.
```

### Comparing `pose2sim-0.3.7/Pose2Sim/filter_3d.py` & `pose2sim-0.3.8/Pose2Sim/filter_3d.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/skeletons.py` & `pose2sim-0.3.8/Pose2Sim/skeletons.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/track_2d.py` & `pose2sim-0.3.8/Pose2Sim/track_2d.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/Pose2Sim/triangulate_3d.py` & `pose2sim-0.3.8/Pose2Sim/triangulate_3d.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/README.md` & `pose2sim-0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -223,21 +223,21 @@
        └──Config.toml
    </pre>
 </details>
 
 ### Camera calibration
 > _**Calibrate your cameras.**_
 
-> - Note 1: Calibration is tricky. I plan to make it more user-friendly, but in the meantime, you can refer to [this issue](https://github.com/perfanalytics/pose2sim/issues/23#issuecomment-1493291952) if you struggle.
+> - Note 1: Calibration is tricky. I plan to make it more user-friendly, but in the meantime, you can refer to [this issue](https://github.com/perfanalytics/pose2sim/issues/18) if you struggle.
 > - Note 2: Cameras need to be synchronized. If they are not natively, you can use [this script](https://github.com/perfanalytics/pose2sim/blob/draft/Pose2Sim/Utilities/synchronize_cams.py).
 
 
 1. If you already have a calibration file (.qca.txt from Qualisys for example):
 - copy it in the `calib-2d` folder
-- set [calibration] type to 'qca' in your `Config.toml` file.
+- set [calibration] type to 'qca' in your `Config.toml` file. Change `binning_factor` to 2 if you film in 540p
 
 or
 
 2. If you have taken pictures or videos of a checkerboard with your cameras:
 - create a folder for each camera in your `calib-2d` folder,
 - copy there the images or videos of the checkerboard
 - set [calibration] type to 'checkerboard' in your `Config.toml` file, and adjust other parameters.
```

### Comparing `pose2sim-0.3.7/pose2sim.egg-info/PKG-INFO` & `pose2sim-0.3.8/pose2sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pose2sim
-Version: 0.3.7
+Version: 0.3.8
 Summary: Perform a markerless kinematic analysis from multiple calibrated views as a unified workflow from an OpenPose input to an OpenSim result.
 Home-page: https://github.com/perfanalytics/pose2sim
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/perfanalytics/pose2sim/issues
 Keywords: markerless,kinematics,OpenPose,OpenSim,3D human pose,biomechanics
@@ -250,21 +250,21 @@
        └──Config.toml
    </pre>
 </details>
 
 ### Camera calibration
 > _**Calibrate your cameras.**_
 
-> - Note 1: Calibration is tricky. I plan to make it more user-friendly, but in the meantime, you can refer to [this issue](https://github.com/perfanalytics/pose2sim/issues/23#issuecomment-1493291952) if you struggle.
+> - Note 1: Calibration is tricky. I plan to make it more user-friendly, but in the meantime, you can refer to [this issue](https://github.com/perfanalytics/pose2sim/issues/18) if you struggle.
 > - Note 2: Cameras need to be synchronized. If they are not natively, you can use [this script](https://github.com/perfanalytics/pose2sim/blob/draft/Pose2Sim/Utilities/synchronize_cams.py).
 
 
 1. If you already have a calibration file (.qca.txt from Qualisys for example):
 - copy it in the `calib-2d` folder
-- set [calibration] type to 'qca' in your `Config.toml` file.
+- set [calibration] type to 'qca' in your `Config.toml` file. Change `binning_factor` to 2 if you film in 540p
 
 or
 
 2. If you have taken pictures or videos of a checkerboard with your cameras:
 - create a folder for each camera in your `calib-2d` folder,
 - copy there the images or videos of the checkerboard
 - set [calibration] type to 'checkerboard' in your `Config.toml` file, and adjust other parameters.
```

### Comparing `pose2sim-0.3.7/pose2sim.egg-info/SOURCES.txt` & `pose2sim-0.3.8/pose2sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.7/setup.cfg` & `pose2sim-0.3.8/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pose2sim
-version = 0.3.7
+version = 0.3.8
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Perform a markerless kinematic analysis from multiple calibrated views as a unified workflow from an OpenPose input to an OpenSim result.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/perfanalytics/pose2sim
 keywords = markerless, kinematics, OpenPose, OpenSim, 3D human pose, biomechanics
```


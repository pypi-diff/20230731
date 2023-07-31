# Comparing `tmp/cubids-1.0.8.tar.gz` & `tmp/cubids-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubids-1.0.8.tar", last modified: Mon Sep 12 13:13:49 2022, max compression
+gzip compressed data, was "cubids-1.0.9.tar", last modified: Mon Jul 31 06:47:31 2023, max compression
```

## Comparing `cubids-1.0.8.tar` & `cubids-1.0.9.tar`

### file list

```diff
@@ -1,313 +1,286 @@
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.935052 cubids-1.0.8/
--rw-r--r--   0 scovitz    (502) staff       (20)      409 2022-05-01 16:12:43.000000 cubids-1.0.8/AUTHORS.rst
--rw-r--r--   0 scovitz    (502) staff       (20)     3517 2022-05-03 14:42:13.000000 cubids-1.0.8/CONTRIBUTING.rst
--rw-r--r--   0 scovitz    (502) staff       (20)       89 2022-02-09 03:05:59.000000 cubids-1.0.8/HISTORY.rst
--rw-r--r--   0 scovitz    (502) staff       (20)     1102 2022-02-09 03:05:59.000000 cubids-1.0.8/LICENSE
--rw-r--r--   0 scovitz    (502) staff       (20)      298 2022-02-09 03:05:59.000000 cubids-1.0.8/MANIFEST.in
--rw-r--r--   0 scovitz    (502) staff       (20)     2448 2022-09-12 13:13:49.935152 cubids-1.0.8/PKG-INFO
--rw-r--r--   0 scovitz    (502) staff       (20)     1546 2022-05-03 16:55:56.000000 cubids-1.0.8/README.rst
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.848283 cubids-1.0.8/cubids/
--rw-r--r--   0 scovitz    (502) staff       (20)      148 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/__init__.py
--rw-r--r--   0 scovitz    (502) staff       (20)    39368 2022-08-19 17:19:14.000000 cubids-1.0.8/cubids/cli.py
--rw-r--r--   0 scovitz    (502) staff       (20)      423 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/config.py
--rw-r--r--   0 scovitz    (502) staff       (20)      711 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/constants.py
--rw-r--r--   0 scovitz    (502) staff       (20)    61121 2022-09-12 13:02:38.000000 cubids-1.0.8/cubids/cubids.py
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.849487 cubids-1.0.8/cubids/data/
--rw-r--r--   0 scovitz    (502) staff       (20)    10942 2022-05-16 15:26:01.000000 cubids-1.0.8/cubids/data/config.yml
--rw-r--r--   0 scovitz    (502) staff       (20)     9908 2022-08-19 17:19:14.000000 cubids-1.0.8/cubids/metadata_merge.py
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.850148 cubids-1.0.8/cubids/testdata/
--rw-r--r--   0 scovitz    (502) staff       (20)     6148 2022-04-29 15:55:16.000000 cubids-1.0.8/cubids/testdata/.DS_Store
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.850909 cubids-1.0.8/cubids/testdata/BIDS_Dataset/
--rw-r--r--   0 scovitz    (502) staff       (20)      368 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/README
--rw-r--r--   0 scovitz    (502) staff       (20)      189 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/dataset_description.json
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.839565 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.839851 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.851362 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)     1067 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.854031 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)       44 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)      245 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     2011 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     6084 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.855878 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1675 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1698 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1787 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.856333 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     2234 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.839984 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.840301 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.856889 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)     1036 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.858000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     2042 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.860568 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1675 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1698 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1787 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     2012 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.860955 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     2168 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.840451 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.840775 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.861369 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)     1036 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.862271 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1975 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.863792 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1675 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1698 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1787 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.864213 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     2202 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.840937 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.841271 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.864768 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)     1036 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.866253 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     2007 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.867941 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1675 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1698 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1787 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.868390 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     2202 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-05-02 14:18:21.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)    69774 2022-05-02 14:16:26.000000 cubids-1.0.8/cubids/testdata/BIDS_Dataset.zip
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.869041 cubids-1.0.8/cubids/testdata/complete/
--rw-r--r--   0 scovitz    (502) staff       (20)       73 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/README
--rw-r--r--   0 scovitz    (502) staff       (20)      189 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/dataset_description.json
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.841478 cubids-1.0.8/cubids/testdata/complete/sub-01/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.841761 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.869488 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.870463 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.873268 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1604 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.873644 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1970 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.841889 cubids-1.0.8/cubids/testdata/complete/sub-02/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.842159 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.874222 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.880377 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.882670 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.883073 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1970 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.842291 cubids-1.0.8/cubids/testdata/complete/sub-03/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.842566 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.884243 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.885586 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.887344 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.887659 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1970 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.888094 cubids-1.0.8/cubids/testdata/inconsistent/
--rw-r--r--   0 scovitz    (502) staff       (20)      368 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/README
--rw-r--r--   0 scovitz    (502) staff       (20)      189 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/dataset_description.json
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.842801 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.843215 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.888471 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.889563 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.891272 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.891637 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1970 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.843380 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.843728 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.892093 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.893194 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1761 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.894713 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1782 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.895094 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1937 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.843880 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.844156 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.895502 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.896533 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.899050 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.899341 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1971 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2022-02-09 03:05:59.000000 cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     3694 2022-08-19 17:19:14.000000 cubids-1.0.8/cubids/validator.py
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.849355 cubids-1.0.8/cubids.egg-info/
--rw-r--r--   0 scovitz    (502) staff       (20)     2448 2022-09-12 13:13:49.000000 cubids-1.0.8/cubids.egg-info/PKG-INFO
--rw-r--r--   0 scovitz    (502) staff       (20)    16514 2022-09-12 13:13:49.000000 cubids-1.0.8/cubids.egg-info/SOURCES.txt
--rw-r--r--   0 scovitz    (502) staff       (20)        1 2022-09-12 13:13:49.000000 cubids-1.0.8/cubids.egg-info/dependency_links.txt
--rw-r--r--   0 scovitz    (502) staff       (20)      579 2022-09-12 13:13:49.000000 cubids-1.0.8/cubids.egg-info/entry_points.txt
--rw-r--r--   0 scovitz    (502) staff       (20)        1 2022-02-22 20:30:10.000000 cubids-1.0.8/cubids.egg-info/not-zip-safe
--rw-r--r--   0 scovitz    (502) staff       (20)      517 2022-09-12 13:13:49.000000 cubids-1.0.8/cubids.egg-info/requires.txt
--rw-r--r--   0 scovitz    (502) staff       (20)        7 2022-09-12 13:13:49.000000 cubids-1.0.8/cubids.egg-info/top_level.txt
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.902574 cubids-1.0.8/docs/
--rw-r--r--   0 scovitz    (502) staff       (20)      607 2022-02-09 03:05:59.000000 cubids-1.0.8/docs/Makefile
--rw-r--r--   0 scovitz    (502) staff       (20)     1383 2022-05-03 15:36:13.000000 cubids-1.0.8/docs/README.rst
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.844364 cubids-1.0.8/docs/_build/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.844488 cubids-1.0.8/docs/_build/html/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.909244 cubids-1.0.8/docs/_build/html/_images/
--rw-r--r--   0 scovitz    (502) staff       (20)    63002 2022-04-14 20:35:13.000000 cubids-1.0.8/docs/_build/html/_images/cubids_workflow.png
--rw-r--r--   0 scovitz    (502) staff       (20)   121910 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_images/screenshot_1.png
--rw-r--r--   0 scovitz    (502) staff       (20)   183503 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_images/screenshot_2.png
--rw-r--r--   0 scovitz    (502) staff       (20)   140263 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_images/screenshot_3.png
--rw-r--r--   0 scovitz    (502) staff       (20)   186964 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_images/screenshot_4.png
--rw-r--r--   0 scovitz    (502) staff       (20)   189860 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_images/screenshot_5.png
--rw-r--r--   0 scovitz    (502) staff       (20)   218126 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_images/screenshot_6.png
--rw-r--r--   0 scovitz    (502) staff       (20)   359707 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_images/screenshot_7.png
--rw-r--r--   0 scovitz    (502) staff       (20)   434468 2022-05-02 21:34:17.000000 cubids-1.0.8/docs/_build/html/_images/screenshot_8.png
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.923295 cubids-1.0.8/docs/_build/html/_static/
--rw-r--r--   0 scovitz    (502) staff       (20)    94377 2022-03-23 16:52:54.000000 cubids-1.0.8/docs/_build/html/_static/checked_dataset_into_datalad.png
--rw-r--r--   0 scovitz    (502) staff       (20)    63002 2022-04-13 18:27:20.000000 cubids-1.0.8/docs/_build/html/_static/cubids_workflow.png
--rw-r--r--   0 scovitz    (502) staff       (20)      286 2022-04-13 15:21:48.000000 cubids-1.0.8/docs/_build/html/_static/file.png
--rw-r--r--   0 scovitz    (502) staff       (20)       90 2022-04-13 15:21:48.000000 cubids-1.0.8/docs/_build/html/_static/minus.png
--rw-r--r--   0 scovitz    (502) staff       (20)       90 2022-04-13 15:21:48.000000 cubids-1.0.8/docs/_build/html/_static/plus.png
--rw-r--r--   0 scovitz    (502) staff       (20)   121910 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_static/screenshot_1.png
--rw-r--r--   0 scovitz    (502) staff       (20)   183503 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_static/screenshot_2.png
--rw-r--r--   0 scovitz    (502) staff       (20)   140263 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_static/screenshot_3.png
--rw-r--r--   0 scovitz    (502) staff       (20)   186964 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_static/screenshot_4.png
--rw-r--r--   0 scovitz    (502) staff       (20)   189860 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_static/screenshot_5.png
--rw-r--r--   0 scovitz    (502) staff       (20)   218126 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_static/screenshot_6.png
--rw-r--r--   0 scovitz    (502) staff       (20)   359707 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_build/html/_static/screenshot_7.png
--rw-r--r--   0 scovitz    (502) staff       (20)   434468 2022-05-02 21:34:17.000000 cubids-1.0.8/docs/_build/html/_static/screenshot_8.png
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.933050 cubids-1.0.8/docs/_static/
--rw-r--r--   0 scovitz    (502) staff       (20)    94377 2022-04-14 20:35:13.000000 cubids-1.0.8/docs/_static/checked_dataset_into_datalad.png
--rw-r--r--   0 scovitz    (502) staff       (20)    63002 2022-05-02 03:20:16.000000 cubids-1.0.8/docs/_static/cubids_workflow.png
--rw-r--r--   0 scovitz    (502) staff       (20)   121910 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_static/screenshot_1.png
--rw-r--r--   0 scovitz    (502) staff       (20)   183503 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_static/screenshot_2.png
--rw-r--r--   0 scovitz    (502) staff       (20)   140263 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_static/screenshot_3.png
--rw-r--r--   0 scovitz    (502) staff       (20)   186964 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_static/screenshot_4.png
--rw-r--r--   0 scovitz    (502) staff       (20)   189860 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_static/screenshot_5.png
--rw-r--r--   0 scovitz    (502) staff       (20)   218126 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_static/screenshot_6.png
--rw-r--r--   0 scovitz    (502) staff       (20)   359707 2022-04-26 19:35:09.000000 cubids-1.0.8/docs/_static/screenshot_7.png
--rw-r--r--   0 scovitz    (502) staff       (20)   434468 2022-05-02 21:34:17.000000 cubids-1.0.8/docs/_static/screenshot_8.png
--rw-r--r--   0 scovitz    (502) staff       (20)     3934 2022-08-15 17:30:01.000000 cubids-1.0.8/docs/about.rst
--rw-r--r--   0 scovitz    (502) staff       (20)       28 2022-02-09 03:05:59.000000 cubids-1.0.8/docs/authors.rst
--rwxr-xr-x   0 scovitz    (502) staff       (20)     5579 2022-08-16 18:03:12.000000 cubids-1.0.8/docs/conf.py
--rw-r--r--   0 scovitz    (502) staff       (20)       33 2022-02-09 03:05:59.000000 cubids-1.0.8/docs/contributing.rst
--rw-r--r--   0 scovitz    (502) staff       (20)    17183 2022-08-17 21:54:12.000000 cubids-1.0.8/docs/example.rst
--rw-r--r--   0 scovitz    (502) staff       (20)       28 2022-02-09 03:05:59.000000 cubids-1.0.8/docs/history.rst
--rw-r--r--   0 scovitz    (502) staff       (20)      194 2022-05-05 18:45:11.000000 cubids-1.0.8/docs/index.rst
--rw-r--r--   0 scovitz    (502) staff       (20)     2427 2022-08-16 18:03:12.000000 cubids-1.0.8/docs/installation.rst
--rw-r--r--   0 scovitz    (502) staff       (20)      768 2022-02-09 03:05:59.000000 cubids-1.0.8/docs/make.bat
--rw-r--r--   0 scovitz    (502) staff       (20)    11684 2022-08-17 21:54:12.000000 cubids-1.0.8/docs/usage.rst
--rw-r--r--   0 scovitz    (502) staff       (20)       60 2022-02-09 03:05:59.000000 cubids-1.0.8/pyproject.toml
--rw-r--r--   0 scovitz    (502) staff       (20)     1496 2022-09-12 13:13:49.935691 cubids-1.0.8/setup.cfg
--rw-r--r--   0 scovitz    (502) staff       (20)     2102 2022-09-12 13:09:53.000000 cubids-1.0.8/setup.py
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2022-09-12 13:13:49.934443 cubids-1.0.8/tests/
--rw-r--r--   0 scovitz    (502) staff       (20)    37791 2022-08-31 19:20:18.000000 cubids-1.0.8/tests/test_bond.py
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.479490 cubids-1.0.9/
+-rw-r--r--   0 scovitz    (502) staff       (20)      409 2023-05-04 11:48:08.000000 cubids-1.0.9/AUTHORS.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)     3508 2023-06-05 12:52:08.000000 cubids-1.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)       89 2023-05-04 11:48:08.000000 cubids-1.0.9/HISTORY.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)     1102 2023-05-04 11:48:08.000000 cubids-1.0.9/LICENSE
+-rw-r--r--   0 scovitz    (502) staff       (20)      298 2023-05-04 11:48:08.000000 cubids-1.0.9/MANIFEST.in
+-rw-r--r--   0 scovitz    (502) staff       (20)     2428 2023-07-31 06:47:31.479580 cubids-1.0.9/PKG-INFO
+-rw-r--r--   0 scovitz    (502) staff       (20)     1546 2023-05-04 11:48:08.000000 cubids-1.0.9/README.rst
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.436551 cubids-1.0.9/cubids/
+-rw-r--r--   0 scovitz    (502) staff       (20)      148 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/__init__.py
+-rw-r--r--   0 scovitz    (502) staff       (20)    39368 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/cli.py
+-rw-r--r--   0 scovitz    (502) staff       (20)      423 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/config.py
+-rw-r--r--   0 scovitz    (502) staff       (20)      711 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/constants.py
+-rw-r--r--   0 scovitz    (502) staff       (20)    62321 2023-06-05 12:53:20.000000 cubids-1.0.9/cubids/cubids.py
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.437586 cubids-1.0.9/cubids/data/
+-rw-r--r--   0 scovitz    (502) staff       (20)    10942 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/data/config.yml
+-rw-r--r--   0 scovitz    (502) staff       (20)     9908 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/metadata_merge.py
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.437703 cubids-1.0.9/cubids/testdata/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.437986 cubids-1.0.9/cubids/testdata/BIDS_Dataset/
+-rw-r--r--   0 scovitz    (502) staff       (20)      368 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/README
+-rw-r--r--   0 scovitz    (502) staff       (20)      189 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/dataset_description.json
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.428965 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.429232 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.438233 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1067 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.438771 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)       44 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)      245 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     2011 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     6084 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.439710 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1675 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1698 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1787 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.439957 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     2234 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.429355 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.429623 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.440253 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1036 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.440791 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     2042 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.441801 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1675 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1698 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1787 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     2012 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.442044 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     2168 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.429751 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430012 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.442298 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1036 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.442841 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     1975 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.443814 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1675 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1698 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1787 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.444053 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     2202 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430132 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430392 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.444306 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1036 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.444884 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     2007 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.445847 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1675 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1698 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1787 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.446087 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     2202 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)    69774 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset.zip
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.446332 cubids-1.0.9/cubids/testdata/complete/
+-rw-r--r--   0 scovitz    (502) staff       (20)       73 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/README
+-rw-r--r--   0 scovitz    (502) staff       (20)      189 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/dataset_description.json
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430589 cubids-1.0.9/cubids/testdata/complete/sub-01/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430850 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.446563 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.447103 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.449349 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1604 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.449792 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1970 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430971 cubids-1.0.9/cubids/testdata/complete/sub-02/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.431246 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.450186 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.451000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.452605 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.452952 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1970 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.431394 cubids-1.0.9/cubids/testdata/complete/sub-03/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.431782 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.453314 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.454075 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.455740 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.456291 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1970 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.456698 cubids-1.0.9/cubids/testdata/inconsistent/
+-rw-r--r--   0 scovitz    (502) staff       (20)      368 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/README
+-rw-r--r--   0 scovitz    (502) staff       (20)      189 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/dataset_description.json
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.431989 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.432260 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.457140 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.457843 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.459082 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.459354 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1970 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.432379 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.432667 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.459893 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.460764 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     1761 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.462304 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1782 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.462947 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1937 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.432794 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.433048 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.463273 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/
+-rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
+-rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.464267 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/
+-rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.467015 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.467597 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/
+-rw-r--r--   0 scovitz    (502) staff       (20)     1971 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0 scovitz    (502) staff       (20)     3694 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/validator.py
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.437471 cubids-1.0.9/cubids.egg-info/
+-rw-r--r--   0 scovitz    (502) staff       (20)     2428 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/PKG-INFO
+-rw-r--r--   0 scovitz    (502) staff       (20)    15549 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/SOURCES.txt
+-rw-r--r--   0 scovitz    (502) staff       (20)        1 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/dependency_links.txt
+-rw-r--r--   0 scovitz    (502) staff       (20)      579 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/entry_points.txt
+-rw-r--r--   0 scovitz    (502) staff       (20)        1 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/not-zip-safe
+-rw-r--r--   0 scovitz    (502) staff       (20)      522 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/requires.txt
+-rw-r--r--   0 scovitz    (502) staff       (20)        7 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/top_level.txt
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.469891 cubids-1.0.9/docs/
+-rw-r--r--   0 scovitz    (502) staff       (20)      607 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/Makefile
+-rw-r--r--   0 scovitz    (502) staff       (20)     1383 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/README.rst
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.476728 cubids-1.0.9/docs/_static/
+-rw-r--r--   0 scovitz    (502) staff       (20)    94377 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/checked_dataset_into_datalad.png
+-rw-r--r--   0 scovitz    (502) staff       (20)    63002 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/cubids_workflow.png
+-rw-r--r--   0 scovitz    (502) staff       (20)   121910 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_1.png
+-rw-r--r--   0 scovitz    (502) staff       (20)   183503 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_2.png
+-rw-r--r--   0 scovitz    (502) staff       (20)   140263 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_3.png
+-rw-r--r--   0 scovitz    (502) staff       (20)   186964 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_4.png
+-rw-r--r--   0 scovitz    (502) staff       (20)   189860 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_5.png
+-rw-r--r--   0 scovitz    (502) staff       (20)   218126 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_6.png
+-rw-r--r--   0 scovitz    (502) staff       (20)   359707 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_7.png
+-rw-r--r--   0 scovitz    (502) staff       (20)   434468 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_8.png
+-rw-r--r--   0 scovitz    (502) staff       (20)     3934 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/about.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)       28 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/authors.rst
+-rwxr-xr-x   0 scovitz    (502) staff       (20)     5579 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/conf.py
+-rw-r--r--   0 scovitz    (502) staff       (20)       33 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/contributing.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)    17209 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/example.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)       28 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/history.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)      194 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/index.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)     2427 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/installation.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)      768 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/make.bat
+-rw-r--r--   0 scovitz    (502) staff       (20)    12979 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/usage.rst
+-rw-r--r--   0 scovitz    (502) staff       (20)       60 2023-05-04 11:48:08.000000 cubids-1.0.9/pyproject.toml
+-rw-r--r--   0 scovitz    (502) staff       (20)     1501 2023-07-31 06:47:31.480097 cubids-1.0.9/setup.cfg
+-rw-r--r--   0 scovitz    (502) staff       (20)     2102 2023-07-31 06:45:34.000000 cubids-1.0.9/setup.py
+drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.479020 cubids-1.0.9/tests/
+-rw-r--r--   0 scovitz    (502) staff       (20)    37792 2023-05-04 11:48:08.000000 cubids-1.0.9/tests/test_bond.py
```

### Comparing `cubids-1.0.8/CONTRIBUTING.rst` & `cubids-1.0.9/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
+3. The pull request should work for 5, 3.6, 3.7 and 3.8, and for PyPy. Check
    https://circleci.com/gh/PennLINC/CuBIDS
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `cubids-1.0.8/LICENSE` & `cubids-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/PKG-INFO` & `cubids-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cubids
-Version: 1.0.8
+Version: 1.0.9
 Summary: BIDS Curation Tool
 Home-page: https://github.com/pennlinc/cubids
 Author: Neuroinformatics Team of PennLINC
 Author-email: sydney.covitz@pennmecidine.upenn.edu
 Maintainer: Sydney Covitz
 License: MIT License
 Keywords: cubids
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -63,9 +62,7 @@
 History
 =======
 
 0.1.0 (2020-10-07)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `cubids-1.0.8/README.rst` & `cubids-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/cli.py` & `cubids-1.0.9/cubids/cli.py`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/constants.py` & `cubids-1.0.9/cubids/constants.py`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/cubids.py` & `cubids-1.0.9/cubids/cubids.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,23 +52,26 @@
 
         if self.acq_group_level == 'session':
             NON_KEY_ENTITIES.remove("session")
 
     @property
     def layout(self):
         if self._layout is None:
+            # print("SETTING LAYOUT OBJECT")
             self.reset_bids_layout()
+            # print("LAYOUT OBJECT SET")
         return self._layout
 
     def reset_bids_layout(self, validate=False):
         # create BIDS Layout Indexer class
+
         ignores = ["code", "stimuli", "sourcedata", "models",
                    re.compile(r'^\.'), re.compile(r'/\.')]
-        indexer = bids.BIDSLayoutIndexer(validate=validate,
-                                         ignore=ignores,
+
+        indexer = bids.BIDSLayoutIndexer(validate=validate, ignore=ignores,
                                          index_metadata=False)
 
         self._layout = bids.BIDSLayout(self.path,
                                        validate=validate,
                                        indexer=indexer)
 
     def create_cubids_code_dir(self):
@@ -186,15 +189,15 @@
                         data["Dim2Size"] = matrix_dims[1]
                     if "Dim3Size" not in data.keys():
                         data["Dim3Size"] = matrix_dims[2]
                     if "NumVolumes" not in data.keys():
                         if img.ndim == 4:
                             data["NumVolumes"] = matrix_dims[3]
                         elif img.ndim == 3:
-                            data["NumVolumes"] = 1.0
+                            data["NumVolumes"] = 1
                     if "ImageOrientation" not in data.keys():
                         orient = nb.orientations.aff2axcodes(img.affine)
                         joined = ''.join(orient) + '+'
                         data["ImageOrientation"] = joined
                     with open(sidecar, 'w') as file:
                         json.dump(data, file, indent=4)
 
@@ -492,14 +495,17 @@
         # RENAME INTENDED FORS!
         ses_path = self.path + '/' + sub + '/' + ses
         for path in Path(ses_path).rglob("fmap/*.json"):
             self.IF_rename_paths.append(str(path))
             # json_file = self.layout.get_file(str(path))
             # data = json_file.get_dict()
             data = get_sidecar_metadata(str(path))
+            if data == "Erroneous sidecar":
+                print('Error parsing sidecar: ', str(path))
+                continue
 
             if 'IntendedFor' in data.keys():
                 # check if IntendedFor field is a str or list
                 if isinstance(data['IntendedFor'], str):
                     if data['IntendedFor'] == \
                             _get_intended_for_reference(filepath):
                         # replace old filename with new one (overwrite string)
@@ -623,17 +629,19 @@
             if_scans.append(_get_intended_for_reference(self.path + scan))
 
         for path in Path(self.path).rglob("sub-*/*/fmap/*.json"):
 
             # json_file = self.layout.get_file(str(path))
             # data = json_file.get_dict()
             data = get_sidecar_metadata(str(path))
+            if data == "Erroneous sidecar":
+                print('Error parsing sidecar: ', str(path))
+                continue
 
             # remove scan references in the IntendedFor
-
             if 'IntendedFor' in data.keys():
                 # check if IntendedFor field value is a list or a string
                 if isinstance(data['IntendedFor'], str):
                     if data['IntendedFor'] in if_scans:
                         data['IntendedFor'] = []
                         # update the json with the new data dictionary
                         _update_json(str(path), data)
@@ -750,15 +758,19 @@
                                      extension=['.nii.gz', '.nii'])
 
         misfits = []
         files_to_fmaps = defaultdict(list)
         for fmap_file in tqdm(fmap_files):
             # intentions = listify(fmap_file.get_metadata().get("IntendedFor"))
             fmap_json = img_to_new_ext(fmap_file.path, '.json')
-            if_list = get_sidecar_metadata(fmap_json).get("IntendedFor")
+            metadata = get_sidecar_metadata(fmap_json)
+            if metadata == "Erroneous sidecar":
+                print('Error parsing sidecar: ', str(fmap_json))
+                continue
+            if_list = metadata.get("IntendedFor")
             intentions = listify(if_list)
             subject_prefix = "sub-%s" % fmap_file.entities['subject']
 
             if intentions is not None:
                 for intended_for in intentions:
                     full_path = Path(self.path) / subject_prefix / intended_for
                     files_to_fmaps[str(full_path)].append(fmap_file)
@@ -817,14 +829,17 @@
             print("Unusual Modality Detected")
             modality = 'other'
 
         ret = _get_param_groups(
             to_include, self.layout, self.fieldmap_lookup, key_group,
             self.grouping_config, modality, self.keys_files)
 
+        if ret == "erroneous sidecar found":
+            return "erroneous sidecar found"
+
         # add modality to the retun tuple
         l_ret = list(ret)
         l_ret.append(modality)
         tup_ret = tuple(l_ret)
         return tup_ret
 
     def create_data_dictionary(self):
@@ -939,16 +954,19 @@
     def get_param_groups_dataframes(self):
         '''Creates DataFrames of files x param groups and a summary'''
 
         key_groups = self.get_key_groups()
         labeled_files = []
         param_group_summaries = []
         for key_group in key_groups:
-            labeled_file_params, param_summary, modality = \
-                self.get_param_groups_from_key_group(key_group)
+            try:
+                labeled_file_params, param_summary, modality = \
+                    self.get_param_groups_from_key_group(key_group)
+            except Exception:
+                continue
             if labeled_file_params is None:
                 continue
             param_group_summaries.append(param_summary)
             labeled_files.append(labeled_file_params)
 
         big_df = _order_columns(pd.concat(labeled_files, ignore_index=True))
 
@@ -1141,15 +1159,15 @@
 
         summary.to_csv(path_prefix + "_summary.tsv", sep="\t", index=False)
 
         # Calculate the acq groups
         group_by_acquisition_sets(path_prefix + "_files.tsv", path_prefix,
                                   self.acq_group_level)
 
-        print("Detected " + str(len(summary)) + " Parameter Groups.")
+        print("CuBIDS detected " + str(len(summary)) + " Parameter Groups.")
 
     def get_key_groups(self):
         '''Identifies the key groups for the bids dataset'''
 
         # reset self.keys_files
         self.keys_files = {}
 
@@ -1331,66 +1349,70 @@
     derived_params = grouping_config.get('derived_params')
     derived_params = derived_params[modality]
 
     imaging_params.update(derived_params)
 
     dfs = []
     # path needs to be relative to the root with no leading prefix
+
     for path in files:
         # metadata = layout.get_metadata(path)
         metadata = get_sidecar_metadata(img_to_new_ext(path, '.json'))
-        intentions = metadata.get("IntendedFor", [])
-        slice_times = metadata.get("SliceTiming", [])
+        if metadata == "Erroneous sidecar":
+            print('Error parsing sidecar: ', img_to_new_ext(path, '.json'))
+        else:
+            intentions = metadata.get("IntendedFor", [])
+            slice_times = metadata.get("SliceTiming", [])
 
-        wanted_keys = metadata.keys() & imaging_params
-        example_data = {key: metadata[key] for key in wanted_keys}
-        example_data["KeyGroup"] = key_group_name
-
-        # Get the fieldmaps out and add their types
-        if 'FieldmapKey' in relational_params:
-            fieldmap_types = sorted([_file_to_key_group(fmap.path) for
-                                    fmap in fieldmap_lookup[path]])
-
-            # check if config says columns or bool
-            if relational_params['FieldmapKey']['display_mode'] == \
-                    'bool':
-                if len(fieldmap_types) > 0:
-                    example_data['HasFieldmap'] = True
+            wanted_keys = metadata.keys() & imaging_params
+            example_data = {key: metadata[key] for key in wanted_keys}
+            example_data["KeyGroup"] = key_group_name
+
+            # Get the fieldmaps out and add their types
+            if 'FieldmapKey' in relational_params:
+                fieldmap_types = sorted([_file_to_key_group(fmap.path) for
+                                        fmap in fieldmap_lookup[path]])
+
+                # check if config says columns or bool
+                if relational_params['FieldmapKey']['display_mode'] == \
+                        'bool':
+                    if len(fieldmap_types) > 0:
+                        example_data['HasFieldmap'] = True
+                    else:
+                        example_data['HasFieldmap'] = False
                 else:
-                    example_data['HasFieldmap'] = False
-            else:
-                for fmap_num, fmap_type in enumerate(fieldmap_types):
-                    example_data['FieldmapKey%02d' % fmap_num] = fmap_type
+                    for fmap_num, fmap_type in enumerate(fieldmap_types):
+                        example_data['FieldmapKey%02d' % fmap_num] = fmap_type
 
-        # Add the number of slice times specified
-        if "NSliceTimes" in derived_params:
-            example_data["NSliceTimes"] = len(slice_times)
-
-        example_data["FilePath"] = path
-
-        # If it's a fieldmap, see what key group it's intended to correct
-        if "IntendedForKey" in relational_params:
-            intended_key_groups = sorted([_file_to_key_group(intention) for
-                                          intention in intentions])
-
-            # check if config says columns or bool
-            if relational_params['IntendedForKey']['display_mode'] == \
-                    'bool':
-                if len(intended_key_groups) > 0:
-                    example_data["UsedAsFieldmap"] = True
+            # Add the number of slice times specified
+            if "NSliceTimes" in derived_params:
+                example_data["NSliceTimes"] = len(slice_times)
+
+            example_data["FilePath"] = path
+
+            # If it's a fieldmap, see what key group it's intended to correct
+            if "IntendedForKey" in relational_params:
+                intended_key_groups = sorted([_file_to_key_group(intention) for
+                                             intention in intentions])
+
+                # check if config says columns or bool
+                if relational_params['IntendedForKey']['display_mode'] == \
+                        'bool':
+                    if len(intended_key_groups) > 0:
+                        example_data["UsedAsFieldmap"] = True
+                    else:
+                        example_data["UsedAsFieldmap"] = False
                 else:
-                    example_data["UsedAsFieldmap"] = False
-            else:
-                for intention_num, intention_key_group in \
-                        enumerate(intended_key_groups):
-                    example_data[
-                        "IntendedForKey%02d" % intention_num] = \
-                                intention_key_group
+                    for intention_num, intention_key_group in \
+                            enumerate(intended_key_groups):
+                        example_data[
+                            "IntendedForKey%02d" % intention_num] = \
+                                    intention_key_group
 
-        dfs.append(example_data)
+            dfs.append(example_data)
 
     # Assign each file to a ParamGroup
 
     # round param groups based on precision
     df = round_params(pd.DataFrame(dfs), grouping_config, modality)
 
     # cluster param groups based on tolerance
@@ -1399,18 +1421,21 @@
 
     # get the subset of columns to drop duplicates by
     check_cols = []
     for col in list(df.columns):
         if "Cluster_" + col not in list(df.columns) and col != 'FilePath':
             check_cols.append(col)
 
-    # Find the unique ParamGroups and assign ID numbers in "ParamGroup"
-    deduped = df.drop('FilePath', axis=1).drop_duplicates(subset=check_cols,
-                                                          ignore_index=True)
+    # Find the unique ParamGroups and assign ID numbers in "ParamGroup"\
+    try:
+        deduped = df.drop('FilePath', axis=1)
+    except Exception:
+        return "erroneous sidecar found"
 
+    deduped = deduped.drop_duplicates(subset=check_cols, ignore_index=True)
     deduped["ParamGroup"] = np.arange(deduped.shape[0]) + 1
 
     # add the modality as a column
     deduped["Modality"] = modality
 
     # add key group count column (will delete later)
     deduped["KeyGroupCount"] = len(keys_files[key_group_name])
@@ -1457,26 +1482,31 @@
     to_format = config['sidecar_params'][modality]
     to_format.update(config['derived_params'][modality])
 
     for column_name, column_fmt in to_format.items():
         if column_name not in param_group_df:
             continue
         if 'precision' in column_fmt:
-            param_group_df[column_name] = \
-                param_group_df[column_name].round(column_fmt['precision'])
+            if isinstance(param_group_df[column_name], float):
+                param_group_df[column_name] = \
+                    param_group_df[column_name].round(column_fmt['precision'])
 
     return param_group_df
 
 
 def get_sidecar_metadata(json_file):
     # get all metadata values in a file's sidecar
     # transform json dictionary to python dictionary
-    with open(json_file) as json_file:
-        data = json.load(json_file)
-    return data
+    try:
+        with open(json_file) as json_file:
+            data = json.load(json_file)
+            return data
+    except Exception:
+        # print("Error loading sidecar: ", json_filename)
+        return "Erroneous sidecar"
 
 
 def format_params(param_group_df, config, modality):
     '''Run AgglomerativeClustering on param groups, add columns to dataframe'''
 
     to_format = config['sidecar_params'][modality]
     to_format.update(config['derived_params'][modality])
```

### Comparing `cubids-1.0.8/cubids/data/config.yml` & `cubids-1.0.9/cubids/data/config.yml`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/metadata_merge.py` & `cubids-1.0.9/cubids/metadata_merge.py`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/BIDS_Dataset.zip` & `cubids-1.0.9/cubids/testdata/BIDS_Dataset.zip`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids/validator.py` & `cubids-1.0.9/cubids/validator.py`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids.egg-info/PKG-INFO` & `cubids-1.0.9/cubids.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cubids
-Version: 1.0.8
+Version: 1.0.9
 Summary: BIDS Curation Tool
 Home-page: https://github.com/pennlinc/cubids
 Author: Neuroinformatics Team of PennLINC
 Author-email: sydney.covitz@pennmecidine.upenn.edu
 Maintainer: Sydney Covitz
 License: MIT License
 Keywords: cubids
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -63,9 +62,7 @@
 History
 =======
 
 0.1.0 (2020-10-07)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `cubids-1.0.8/cubids.egg-info/SOURCES.txt` & `cubids-1.0.9/cubids.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 cubids.egg-info/SOURCES.txt
 cubids.egg-info/dependency_links.txt
 cubids.egg-info/entry_points.txt
 cubids.egg-info/not-zip-safe
 cubids.egg-info/requires.txt
 cubids.egg-info/top_level.txt
 cubids/data/config.yml
-cubids/testdata/.DS_Store
 cubids/testdata/BIDS_Dataset.zip
 cubids/testdata/BIDS_Dataset/README
 cubids/testdata/BIDS_Dataset/dataset_description.json
 cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
 cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
 cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
 cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
@@ -197,38 +196,15 @@
 docs/conf.py
 docs/contributing.rst
 docs/example.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
-docs/readme.rst
 docs/usage.rst
-docs/_build/html/_images/cubids_workflow.png
-docs/_build/html/_images/screenshot_1.png
-docs/_build/html/_images/screenshot_2.png
-docs/_build/html/_images/screenshot_3.png
-docs/_build/html/_images/screenshot_4.png
-docs/_build/html/_images/screenshot_5.png
-docs/_build/html/_images/screenshot_6.png
-docs/_build/html/_images/screenshot_7.png
-docs/_build/html/_images/screenshot_8.png
-docs/_build/html/_static/checked_dataset_into_datalad.png
-docs/_build/html/_static/cubids_workflow.png
-docs/_build/html/_static/file.png
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/plus.png
-docs/_build/html/_static/screenshot_1.png
-docs/_build/html/_static/screenshot_2.png
-docs/_build/html/_static/screenshot_3.png
-docs/_build/html/_static/screenshot_4.png
-docs/_build/html/_static/screenshot_5.png
-docs/_build/html/_static/screenshot_6.png
-docs/_build/html/_static/screenshot_7.png
-docs/_build/html/_static/screenshot_8.png
 docs/_static/checked_dataset_into_datalad.png
 docs/_static/cubids_workflow.png
 docs/_static/screenshot_1.png
 docs/_static/screenshot_2.png
 docs/_static/screenshot_3.png
 docs/_static/screenshot_4.png
 docs/_static/screenshot_5.png
```

### Comparing `cubids-1.0.8/cubids.egg-info/entry_points.txt` & `cubids-1.0.9/cubids.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/cubids.egg-info/requires.txt` & `cubids-1.0.9/cubids.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pyyaml
 pybids
 pandas
 tqdm
 numpy
-sklearn
+scikit-learn
 datalad>=0.13.5
 wrapt<2,>=1.10
 Sphinx
 jinja2<3.1
 
 [all]
 datalad
```

### Comparing `cubids-1.0.8/docs/Makefile` & `cubids-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/README.rst` & `cubids-1.0.9/docs/README.rst`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/cubids_workflow.png` & `cubids-1.0.9/docs/_static/cubids_workflow.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/screenshot_1.png` & `cubids-1.0.9/docs/_static/screenshot_1.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/screenshot_2.png` & `cubids-1.0.9/docs/_static/screenshot_2.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/screenshot_3.png` & `cubids-1.0.9/docs/_static/screenshot_3.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/screenshot_4.png` & `cubids-1.0.9/docs/_static/screenshot_4.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/screenshot_5.png` & `cubids-1.0.9/docs/_static/screenshot_5.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/screenshot_6.png` & `cubids-1.0.9/docs/_static/screenshot_6.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/screenshot_7.png` & `cubids-1.0.9/docs/_static/screenshot_7.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_images/screenshot_8.png` & `cubids-1.0.9/docs/_static/screenshot_8.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/_build/html/_static/checked_dataset_into_datalad.png` & `cubids-1.0.9/docs/_static/checked_dataset_into_datalad.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/about.rst` & `cubids-1.0.9/docs/about.rst`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/conf.py` & `cubids-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/example.rst` & `cubids-1.0.9/docs/example.rst`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 The next step in the ``CuBIDS`` workflow is to run BIDS validation
 to detect potential curation errors using ``cubids-validate``.
 
 .. code-block:: console
 
     $ cubids-validate BIDS_Dataset_DataLad v0 --sequential
 
-.. note::  The use of the ``--sequential`` flag forces the validator to treat each participant as its own BIDS dataset. This can be helpful for identifying heterogenous elements, but can be slowed down by extremely large datasets.
+.. note::  The use of the ``--sequential`` flag forces the validator to treat each participant as its own BIDS dataset. This can be helpful for identifying heterogeneous elements, but can be slowed down by extremely large datasets.
 
 This command produces the following tsv: 
 
 .. csv-table:: v0_validation.tsv
    :file: _static/v0_validation.csv
    :widths: 10, 10, 10, 10, 10, 40, 10
    :header-rows: 1
@@ -191,15 +191,17 @@
 For the purpose of this demonstration, we elect to remove 
 the scan. To do this, we run the ``cubids-purge`` command.
 
 ``cubids-purge`` requires as input a list of files to cleanly 
 "purge" from the dataset. You can create this file in any
 text editor, as long as it is saved as plain text ``.txt``. For this example, we created the following file: 
 
-... code-block:: console
+.. code-block:: console
+    
+    $ cat no_ped.txt
     
     /AN/EXAMPLE/PATH/CuBIDS_Test/BIDS_Dataset_Datalad/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
 
 
 and saved it in our ``CuBIDS_Test directory``. 
 
 To safely purge this file from the dataset, run:
```

### Comparing `cubids-1.0.8/docs/installation.rst` & `cubids-1.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/make.bat` & `cubids-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cubids-1.0.8/docs/usage.rst` & `cubids-1.0.9/docs/usage.rst`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 Even though two images may belong to the same Key Group and are valid BIDS, they
 may have images with different acquisition parameters. There is nothing fundamentally
 wrong with this — the ``bids-validator`` will often simply flag these differences,
 with a ``Warning``, but not necessarily suggest changes. That being said,
 there can be detrimental consequences downstream if the different parameters cause the
 same preprocessing pipelines to configure differently to images of the same Key Group.
 
+Acquisition Group
+~~~~~~~~~~~~~~~~~
+
+Acquisition Groups are sets of subjects who's images belong to all the same Key and Parameter Groups. The Acquistion Groups that subjects belong to are listed in ``_AcqGrouping.csv``, while the Key Groups and Parameter Groups that define each Acquisition Group are noted in ``_AcqGroupingInfo.txt``.
+
 
 .. _acquisitiongroup:
 
 Acquisition Group
 ~~~~~~~~~~~~~~~~~~
 
 We define an “Acquisition Group” as a collection of sessions across participants that contain the exact 
@@ -87,17 +92,38 @@
 
 This file contains one row per imaging file in the BIDS directory. You won't need to edit this file
 directly, but it keeps track of every file's assignment to Key and Parameter Groups.
 
 
 .. _acqgrouptsv:
 
+Modifying Key and Parameter Group Assignments
+---------------------------------------------
+
+Sometimes we see that there are important differences in acquisition parameters within a Key Group.
+If these differences impact how a pipeline will process the data, it makes sense to assign the scans
+in that Parameter Group to a different Key Group (i.e. assign them a different BIDS name). This can
+be accomplished by editing the empty columns in the `_summary.csv` file produced by ``cubids-group``.
+
+Once the columns have been edited you can apply the changes to BIDS data using
+
+.. code-block:: console
+
+    $ cubids-apply /bids/dir keyparam_edited new_keyparam_prefix
+
+The changes in ``keyparam_edited_summary.csv`` will be applied to the BIDS data in ``/bids/dir``
+and the new Key and Parameter groups will be saved to csv files starting with ``new_keyparam_prefix``. Note:
+fieldmaps keygroups with variant parameters will be identified but not renamed. 
+
+
+
 The ``_AcqGrouping.tsv`` file
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+
 The ``_AcqGrouping.tsv`` file organizes the dataset by session and tags each one with its Acquisition Group number.
 
 .. _acqgrouptxt:
 
 The ``_AcqGroupInfo.txt`` file
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -112,15 +138,15 @@
 .. code-block:: console
 
     $ cubids-group FULL/PATH/TO/BIDS/DIR FULL/PATH/TO/v0
 
 This will output four files, including the summary and files tsvs described above, 
 prefixed by the second argument ``v0``.
 
-Appplying changes 
+Applying changes 
 ------------------
 
 The ``cubids-apply`` program provides an easy way for users to manipulate their datasets. 
 Specifically, ``cubids-apply`` can rename files according to the users’ specification in a tracked 
 and organized way. Here, the summary.tsv functions as an interface modifications; users can mark 
 ``Parameter Groups`` they want to rename (or delete) in a dedicated column of the summary.tsv and 
 pass that edited tsv as an argument to ``cubids-apply``.
@@ -132,25 +158,25 @@
 scanning parameters that vary from those in their Key Groups’ Dominant Parameter Groups. Renaming 
 is automatically suggested when the summary.tsv is generated from a cubids-group run, with the suggested 
 new name listed in the tsv’s “Rename Key Group” column. CuBIDS populates this column for all Variant 
 Groups—e.g., every Parameter Group except the Dominant one. Specifically, CuBIDS will suggest renaming 
 all non-dominant Parameter Group to include VARIANT* in their acquisition field where * is the reason 
 the Parameter Group varies from the Dominant Group. For example, when CuBIDS encounters a Parameter 
 Group with a repetition time that varies from the one present in the Dominant Group, it will automatically 
-suggest renaming all scans in that Variant Group to include ``acquisition-VARIANTRepetitionTime`` in thier 
+suggest renaming all scans in that Variant Group to include ``acquisition-VARIANTRepetitionTime`` in their 
 filenames. When the user runs ``cubids-apply``, filenames will get renamed according to the auto-generated 
 names in the “Rename Key Group” column in the summary.tsv
 
 Deleting a mistake
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To remove files in a Parameter Group from your BIDS data, you simply set the ``MergeInto`` value
 to ``0``. We see in our data that there is a strange scan that has a ``RepetitionTime`` of 12.3
 seconds and is also variant with respect to EffectiveEchoSpacing and EchoTime. We elect to remove this scan from 
-our dataset becasuse we do not want these parameters to affect our analyses.
+our dataset because we do not want these parameters to affect our analyses.
 To remove these files from your BIDS data, add a ``0`` to ``MergeInto`` and save the new tsv as ``v0_edited_summary.tsv``
 
 .. csv-table:: Pre Apply Groupings with Deletion Requested
     :file: _static/PNC_pre_apply_summary_dwi_run1_deletion.csv
     :widths: 3, 3, 3, 3, 3, 3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 3
     :header-rows: 1
```

### Comparing `cubids-1.0.8/setup.cfg` & `cubids-1.0.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 per-file-ignores = 
 	__init__.py: F401
 putty-ignore = 
 	*/__init__.py : +F401
 	/^\s*\.\. _.*?: http/ : +E501
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	pyyaml
 	pybids
 	pandas
 	tqdm
 	numpy
-	sklearn
+	scikit-learn
 	datalad>=0.13.5
 	wrapt<2,>=1.10
 	Sphinx
 	jinja2 < 3.1
 test_requires = 
 	nibabel
 	pytest==4.6.5
```

### Comparing `cubids-1.0.8/setup.py` & `cubids-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     include_package_data=True,
     keywords='cubids',
     name='cubids',
     packages=find_packages(include=['cubids', 'cubids.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     url='https://github.com/pennlinc/cubids',
-    version='1.0.8',
+    version='1.0.9',
     zip_safe=False,
 )
```

### Comparing `cubids-1.0.8/tests/test_bond.py` & `cubids-1.0.9/tests/test_bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,15 +813,15 @@
     if 'bold' in img_path:
         no_suffix = img_path.rpartition('_')[0]
         bold_ext_file = no_suffix + '_events' + '.tsv'
         Path(bold_ext_file).touch()
 
 
 def _edit_a_json(json_file):
-    """Open a json file, write somthing to it and save it to the same name."""
+    """Open a json file, write something to it and save it to the same name."""
     with open(json_file, "r") as metadatar:
         metadata = json.load(metadatar)
 
     metadata["THIS_IS_A_TEST"] = True
     with open(json_file, "w") as metadataw:
         json.dump(metadata, metadataw)
```


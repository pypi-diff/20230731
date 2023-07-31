# Comparing `tmp/soursop-0.2.3.tar.gz` & `tmp/soursop-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soursop-0.2.3.tar", last modified: Tue Feb 14 11:56:25 2023, max compression
+gzip compressed data, was "soursop-0.2.4.tar", last modified: Mon Jul 31 02:58:44 2023, max compression
```

## Comparing `soursop-0.2.3.tar` & `soursop-0.2.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.863272 soursop-0.2.3/
--rw-r--r--   0 alex       (501) staff       (20)     7371 2019-03-14 11:56:50.000000 soursop-0.2.3/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)      205 2022-06-07 04:54:17.000000 soursop-0.2.3/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     4958 2023-02-14 11:56:25.863368 soursop-0.2.3/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     4677 2023-02-11 20:21:27.000000 soursop-0.2.3/README.md
--rw-r--r--   0 alex       (501) staff       (20)      323 2023-02-14 11:56:25.863697 soursop-0.2.3/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     2332 2023-02-11 19:19:05.000000 soursop-0.2.3/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.863870 soursop-0.2.3/soursop/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.579102 soursop-0.2.3/soursop/.ipynb_checkpoints/
--rw-r--r--   0 alex       (501) staff       (20)       72 2022-06-25 11:23:06.000000 soursop-0.2.3/soursop/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0 alex       (501) staff       (20)     1041 2022-06-07 04:54:17.000000 soursop-0.2.3/soursop/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    10145 2022-04-17 22:31:34.000000 soursop-0.2.3/soursop/_internal_data.py
--rw-r--r--   0 alex       (501) staff       (20)      498 2023-02-14 11:56:25.863906 soursop-0.2.3/soursop/_version.py
--rw-r--r--   0 alex       (501) staff       (20)      912 2022-04-17 22:31:13.000000 soursop-0.2.3/soursop/configs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.579501 soursop-0.2.3/soursop/data/
--rw-r--r--   0 alex       (501) staff       (20)     1020 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/SASA_SUMMARY.csv
--rw-r--r--   0 alex       (501) staff       (20)     2628 2019-11-24 19:02:41.000000 soursop-0.2.3/soursop/data/bbseg2.dat
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.608989 soursop-0.2.3/soursop/data/test_data/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.609272 soursop-0.2.3/soursop/data/test_data/.ipynb_checkpoints/
--rw-r--r--   0 alex       (501) staff       (20)       72 2022-01-04 04:19:19.000000 soursop-0.2.3/soursop/data/test_data/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0 alex       (501) staff       (20)    22635 2022-07-01 17:59:57.000000 soursop-0.2.3/soursop/data/test_data/all_residues.pdb
--rw-r--r--   0 alex       (501) staff       (20)    14000 2022-07-01 17:58:32.000000 soursop-0.2.3/soursop/data/test_data/all_residues.xtc
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.616140 soursop-0.2.3/soursop/data/test_data/cap_tests/
--rw-r--r--   0 alex       (501) staff       (20)     3138 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/ACD_start_1.pdb
--rw-r--r--   0 alex       (501) staff       (20)     3183 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/ACD_start_10.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5751 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_NH2.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5952 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_NME.pdb
--rw-r--r--   0 alex       (501) staff       (20)    17610 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_NME_multichain.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5952 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_NME_start_at_5.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5617 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_UCAP.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5550 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/FOR_NH2.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5751 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/FOR_NME.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5416 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/FOR_UCAP.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5483 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/UCAP_NH2.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5684 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/UCAP_NME.pdb
--rw-r--r--   0 alex       (501) staff       (20)     5349 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/UCAP_UCAP.pdb
--rw-r--r--   0 alex       (501) staff       (20)     3138 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/cap_tests/__START.pdb
--rw-r--r--   0 alex       (501) staff       (20)   119208 2022-11-20 15:26:26.000000 soursop-0.2.3/soursop/data/test_data/ctl9.pdb
--rw-r--r--   0 alex       (501) staff       (20)  5820924 2022-11-20 15:26:31.000000 soursop-0.2.3/soursop/data/test_data/ctl9.xtc
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.621899 soursop-0.2.3/soursop/data/test_data/gromacs1chain/
--rwxr--r--   0 alex       (501) staff       (20)    76233 2021-03-11 02:48:11.000000 soursop-0.2.3/soursop/data/test_data/gromacs1chain/top.pdb
--rwxr--r--   0 alex       (501) staff       (20)    73232 2021-03-11 02:47:50.000000 soursop-0.2.3/soursop/data/test_data/gromacs1chain/traj.xtc
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.622877 soursop-0.2.3/soursop/data/test_data/gromacs2chains/
--rwxr--r--   0 alex       (501) staff       (20)    76073 2021-03-11 02:45:08.000000 soursop-0.2.3/soursop/data/test_data/gromacs2chains/top.pdb
--rwxr--r--   0 alex       (501) staff       (20)    76940 2021-03-11 02:45:14.000000 soursop-0.2.3/soursop/data/test_data/gromacs2chains/traj.xtc
--rw-r--r--   0 alex       (501) staff       (20)     4636 2020-05-21 18:00:07.000000 soursop-0.2.3/soursop/data/test_data/gs6.dcd
--rw-r--r--   0 alex       (501) staff       (20)     5808 2019-06-03 21:17:26.000000 soursop-0.2.3/soursop/data/test_data/gs6.pdb
--rw-r--r--   0 alex       (501) staff       (20)     1736 2019-06-03 21:17:46.000000 soursop-0.2.3/soursop/data/test_data/gs6.xtc
--rw-r--r--   0 alex       (501) staff       (20)     5808 2020-12-10 07:11:58.000000 soursop-0.2.3/soursop/data/test_data/gs6_invalid_r1.pdb
--rw-r--r--   0 alex       (501) staff       (20)   110036 2020-05-21 18:00:07.000000 soursop-0.2.3/soursop/data/test_data/ntl9.dcd
--rw-r--r--   0 alex       (501) staff       (20)    73722 2019-05-18 18:15:15.000000 soursop-0.2.3/soursop/data/test_data/ntl9.pdb
--rw-r--r--   0 alex       (501) staff       (20)    36336 2019-05-18 18:15:23.000000 soursop-0.2.3/soursop/data/test_data/ntl9.xtc
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.624163 soursop-0.2.3/soursop/data/test_data/pre_data/
--rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.3/soursop/data/test_data/pre_data/PRE_109_unweighted.csv
--rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.3/soursop/data/test_data/pre_data/PRE_119_unweighted.csv
--rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.3/soursop/data/test_data/pre_data/PRE_149_unweighted.csv
--rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.3/soursop/data/test_data/pre_data/PRE_61_unweighted.csv
--rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.3/soursop/data/test_data/pre_data/PRE_74_unweighted.csv
--rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.3/soursop/data/test_data/pre_data/PRE_96_unweighted.csv
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.624300 soursop-0.2.3/soursop/plugins/
--rw-r--r--   0 alex       (501) staff       (20)      166 2023-02-11 19:36:50.000000 soursop-0.2.3/soursop/plugins/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.751556 soursop-0.2.3/soursop/plugins/sparrow_plugin/
--rw-r--r--   0 alex       (501) staff       (20)     2461 2023-02-11 20:00:55.000000 soursop-0.2.3/soursop/plugins/sparrow_plugin/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1486 2022-06-25 11:26:21.000000 soursop-0.2.3/soursop/soursop.py
--rw-r--r--   0 alex       (501) staff       (20)     4004 2022-11-20 15:17:08.000000 soursop-0.2.3/soursop/ssdata.py
--rw-r--r--   0 alex       (501) staff       (20)     1200 2022-04-17 22:28:43.000000 soursop-0.2.3/soursop/ssexceptions.py
--rw-r--r--   0 alex       (501) staff       (20)     1568 2022-04-17 22:29:32.000000 soursop-0.2.3/soursop/ssio.py
--rw-r--r--   0 alex       (501) staff       (20)     5042 2022-06-23 16:18:42.000000 soursop-0.2.3/soursop/ssmutualinformation.py
--rw-r--r--   0 alex       (501) staff       (20)    29348 2022-04-17 20:44:59.000000 soursop-0.2.3/soursop/ssnmr.py
--rw-r--r--   0 alex       (501) staff       (20)     1358 2022-11-20 15:18:10.000000 soursop-0.2.3/soursop/sspolymer.py
--rw-r--r--   0 alex       (501) staff       (20)    10555 2022-11-20 16:30:04.000000 soursop-0.2.3/soursop/sspre.py
--rw-r--r--   0 alex       (501) staff       (20)   209014 2023-02-11 16:44:41.000000 soursop-0.2.3/soursop/ssprotein.py
--rw-r--r--   0 alex       (501) staff       (20)     2808 2022-04-17 14:08:06.000000 soursop-0.2.3/soursop/sstools.py
--rw-r--r--   0 alex       (501) staff       (20)    41841 2022-12-22 02:21:59.000000 soursop-0.2.3/soursop/sstrajectory.py
--rw-r--r--   0 alex       (501) staff       (20)     7390 2022-06-07 04:54:17.000000 soursop-0.2.3/soursop/ssutils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.755807 soursop-0.2.3/soursop/tests/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.862798 soursop-0.2.3/soursop/tests/.ipynb_checkpoints/
--rw-r--r--   0 alex       (501) staff       (20)     2004 2023-01-04 15:14:46.000000 soursop-0.2.3/soursop/tests/.ipynb_checkpoints/test_scratchpad-checkpoint.ipynb
--rw-r--r--   0 alex       (501) staff       (20)      112 2019-03-14 11:56:50.000000 soursop-0.2.3/soursop/tests/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     3580 2022-11-20 15:36:34.000000 soursop-0.2.3/soursop/tests/conftest.py
--rw-r--r--   0 alex       (501) staff       (20)     1794 2021-08-06 13:55:34.000000 soursop-0.2.3/soursop/tests/test_caps.py
--rw-r--r--   0 alex       (501) staff       (20)     1658 2021-08-06 13:56:07.000000 soursop-0.2.3/soursop/tests/test_numbering.py
--rw-r--r--   0 alex       (501) staff       (20)     1676 2021-08-06 13:52:22.000000 soursop-0.2.3/soursop/tests/test_soursop.py
--rw-r--r--   0 alex       (501) staff       (20)      874 2022-06-23 16:18:42.000000 soursop-0.2.3/soursop/tests/test_ssmutual_information.py
--rw-r--r--   0 alex       (501) staff       (20)    10216 2021-08-06 13:55:07.000000 soursop-0.2.3/soursop/tests/test_ssnmr.py
--rw-r--r--   0 alex       (501) staff       (20)     1413 2021-08-06 13:56:36.000000 soursop-0.2.3/soursop/tests/test_ssnmr_extended.py
--rw-r--r--   0 alex       (501) staff       (20)     1266 2023-01-07 17:19:45.000000 soursop-0.2.3/soursop/tests/test_sspre.py
--rw-r--r--   0 alex       (501) staff       (20)    39061 2023-02-11 16:29:23.000000 soursop-0.2.3/soursop/tests/test_ssproteins.py
--rw-r--r--   0 alex       (501) staff       (20)    24723 2022-04-18 00:15:08.000000 soursop-0.2.3/soursop/tests/test_sstrajectory.py
--rw-r--r--   0 alex       (501) staff       (20)     1384 2022-06-07 04:54:17.000000 soursop-0.2.3/soursop/tests/test_ssutils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-14 11:56:25.578915 soursop-0.2.3/soursop.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     4958 2023-02-14 11:56:25.000000 soursop-0.2.3/soursop.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     2787 2023-02-14 11:56:25.000000 soursop-0.2.3/soursop.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-02-14 11:56:25.000000 soursop-0.2.3/soursop.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       84 2023-02-14 11:56:25.000000 soursop-0.2.3/soursop.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        8 2023-02-14 11:56:25.000000 soursop-0.2.3/soursop.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)    81180 2022-06-07 04:54:17.000000 soursop-0.2.3/versioneer.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:44.190656 soursop-0.2.4/
+-rw-r--r--   0 alex       (501) staff       (20)     7371 2019-03-14 11:56:50.000000 soursop-0.2.4/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)      205 2022-06-07 04:54:17.000000 soursop-0.2.4/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     5358 2023-07-31 02:58:44.190745 soursop-0.2.4/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     5114 2023-07-31 02:57:05.000000 soursop-0.2.4/README.md
+-rw-r--r--   0 alex       (501) staff       (20)      323 2023-07-31 02:58:44.191088 soursop-0.2.4/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     2332 2023-02-11 19:19:05.000000 soursop-0.2.4/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:44.191255 soursop-0.2.4/soursop/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:43.864569 soursop-0.2.4/soursop/.ipynb_checkpoints/
+-rw-r--r--   0 alex       (501) staff       (20)       72 2022-06-25 11:23:06.000000 soursop-0.2.4/soursop/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0 alex       (501) staff       (20)     1041 2022-06-07 04:54:17.000000 soursop-0.2.4/soursop/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    10145 2022-04-17 22:31:34.000000 soursop-0.2.4/soursop/_internal_data.py
+-rw-r--r--   0 alex       (501) staff       (20)      498 2023-07-31 02:58:44.191291 soursop-0.2.4/soursop/_version.py
+-rw-r--r--   0 alex       (501) staff       (20)      912 2022-04-17 22:31:13.000000 soursop-0.2.4/soursop/configs.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:43.865039 soursop-0.2.4/soursop/data/
+-rw-r--r--   0 alex       (501) staff       (20)     1020 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/SASA_SUMMARY.csv
+-rw-r--r--   0 alex       (501) staff       (20)     2628 2019-11-24 19:02:41.000000 soursop-0.2.4/soursop/data/bbseg2.dat
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:43.915860 soursop-0.2.4/soursop/data/test_data/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:43.916098 soursop-0.2.4/soursop/data/test_data/.ipynb_checkpoints/
+-rw-r--r--   0 alex       (501) staff       (20)       72 2022-01-04 04:19:19.000000 soursop-0.2.4/soursop/data/test_data/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0 alex       (501) staff       (20)    22635 2022-07-01 17:59:57.000000 soursop-0.2.4/soursop/data/test_data/all_residues.pdb
+-rw-r--r--   0 alex       (501) staff       (20)    14000 2022-07-01 17:58:32.000000 soursop-0.2.4/soursop/data/test_data/all_residues.xtc
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:43.940354 soursop-0.2.4/soursop/data/test_data/cap_tests/
+-rw-r--r--   0 alex       (501) staff       (20)     3138 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/ACD_start_1.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     3183 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/ACD_start_10.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5751 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_NH2.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5952 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_NME.pdb
+-rw-r--r--   0 alex       (501) staff       (20)    17610 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_NME_multichain.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5952 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_NME_start_at_5.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5617 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_UCAP.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5550 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/FOR_NH2.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5751 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/FOR_NME.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5416 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/FOR_UCAP.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5483 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/UCAP_NH2.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5684 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/UCAP_NME.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     5349 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/UCAP_UCAP.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     3138 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/cap_tests/__START.pdb
+-rw-r--r--   0 alex       (501) staff       (20)   119208 2022-11-20 15:26:26.000000 soursop-0.2.4/soursop/data/test_data/ctl9.pdb
+-rw-r--r--   0 alex       (501) staff       (20)  5820924 2022-11-20 15:26:31.000000 soursop-0.2.4/soursop/data/test_data/ctl9.xtc
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:43.941398 soursop-0.2.4/soursop/data/test_data/gromacs1chain/
+-rwxr--r--   0 alex       (501) staff       (20)    76233 2021-03-11 02:48:11.000000 soursop-0.2.4/soursop/data/test_data/gromacs1chain/top.pdb
+-rwxr--r--   0 alex       (501) staff       (20)    73232 2021-03-11 02:47:50.000000 soursop-0.2.4/soursop/data/test_data/gromacs1chain/traj.xtc
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:44.067885 soursop-0.2.4/soursop/data/test_data/gromacs2chains/
+-rwxr--r--   0 alex       (501) staff       (20)    76073 2021-03-11 02:45:08.000000 soursop-0.2.4/soursop/data/test_data/gromacs2chains/top.pdb
+-rwxr--r--   0 alex       (501) staff       (20)    76940 2021-03-11 02:45:14.000000 soursop-0.2.4/soursop/data/test_data/gromacs2chains/traj.xtc
+-rw-r--r--   0 alex       (501) staff       (20)     4636 2020-05-21 18:00:07.000000 soursop-0.2.4/soursop/data/test_data/gs6.dcd
+-rw-r--r--   0 alex       (501) staff       (20)     5808 2019-06-03 21:17:26.000000 soursop-0.2.4/soursop/data/test_data/gs6.pdb
+-rw-r--r--   0 alex       (501) staff       (20)     1736 2019-06-03 21:17:46.000000 soursop-0.2.4/soursop/data/test_data/gs6.xtc
+-rw-r--r--   0 alex       (501) staff       (20)     5808 2020-12-10 07:11:58.000000 soursop-0.2.4/soursop/data/test_data/gs6_invalid_r1.pdb
+-rw-r--r--   0 alex       (501) staff       (20)   110036 2020-05-21 18:00:07.000000 soursop-0.2.4/soursop/data/test_data/ntl9.dcd
+-rw-r--r--   0 alex       (501) staff       (20)    73722 2019-05-18 18:15:15.000000 soursop-0.2.4/soursop/data/test_data/ntl9.pdb
+-rw-r--r--   0 alex       (501) staff       (20)    36336 2019-05-18 18:15:23.000000 soursop-0.2.4/soursop/data/test_data/ntl9.xtc
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:44.069823 soursop-0.2.4/soursop/data/test_data/pre_data/
+-rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.4/soursop/data/test_data/pre_data/PRE_109_unweighted.csv
+-rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.4/soursop/data/test_data/pre_data/PRE_119_unweighted.csv
+-rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.4/soursop/data/test_data/pre_data/PRE_149_unweighted.csv
+-rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.4/soursop/data/test_data/pre_data/PRE_61_unweighted.csv
+-rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.4/soursop/data/test_data/pre_data/PRE_74_unweighted.csv
+-rw-r--r--   0 alex       (501) staff       (20)     2300 2022-11-20 15:35:48.000000 soursop-0.2.4/soursop/data/test_data/pre_data/PRE_96_unweighted.csv
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:44.070062 soursop-0.2.4/soursop/plugins/
+-rw-r--r--   0 alex       (501) staff       (20)      166 2023-02-11 19:36:50.000000 soursop-0.2.4/soursop/plugins/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:44.070357 soursop-0.2.4/soursop/plugins/sparrow_plugin/
+-rw-r--r--   0 alex       (501) staff       (20)     2461 2023-02-11 20:00:55.000000 soursop-0.2.4/soursop/plugins/sparrow_plugin/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1486 2022-06-25 11:26:21.000000 soursop-0.2.4/soursop/soursop.py
+-rw-r--r--   0 alex       (501) staff       (20)     4004 2022-11-20 15:17:08.000000 soursop-0.2.4/soursop/ssdata.py
+-rw-r--r--   0 alex       (501) staff       (20)     1200 2022-04-17 22:28:43.000000 soursop-0.2.4/soursop/ssexceptions.py
+-rw-r--r--   0 alex       (501) staff       (20)     1568 2022-04-17 22:29:32.000000 soursop-0.2.4/soursop/ssio.py
+-rw-r--r--   0 alex       (501) staff       (20)     5042 2022-06-23 16:18:42.000000 soursop-0.2.4/soursop/ssmutualinformation.py
+-rw-r--r--   0 alex       (501) staff       (20)    29348 2022-04-17 20:44:59.000000 soursop-0.2.4/soursop/ssnmr.py
+-rw-r--r--   0 alex       (501) staff       (20)     1358 2022-11-20 15:18:10.000000 soursop-0.2.4/soursop/sspolymer.py
+-rw-r--r--   0 alex       (501) staff       (20)    10555 2022-11-20 16:30:04.000000 soursop-0.2.4/soursop/sspre.py
+-rw-r--r--   0 alex       (501) staff       (20)   209014 2023-07-14 11:40:41.000000 soursop-0.2.4/soursop/ssprotein.py
+-rw-r--r--   0 alex       (501) staff       (20)     2808 2022-04-17 14:08:06.000000 soursop-0.2.4/soursop/sstools.py
+-rw-r--r--   0 alex       (501) staff       (20)    44350 2023-07-14 12:36:09.000000 soursop-0.2.4/soursop/sstrajectory.py
+-rw-r--r--   0 alex       (501) staff       (20)     7390 2022-06-07 04:54:17.000000 soursop-0.2.4/soursop/ssutils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:44.190019 soursop-0.2.4/soursop/tests/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:44.190336 soursop-0.2.4/soursop/tests/.ipynb_checkpoints/
+-rw-r--r--   0 alex       (501) staff       (20)     2004 2023-01-04 15:14:46.000000 soursop-0.2.4/soursop/tests/.ipynb_checkpoints/test_scratchpad-checkpoint.ipynb
+-rw-r--r--   0 alex       (501) staff       (20)      112 2019-03-14 11:56:50.000000 soursop-0.2.4/soursop/tests/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3580 2022-11-20 15:36:34.000000 soursop-0.2.4/soursop/tests/conftest.py
+-rw-r--r--   0 alex       (501) staff       (20)     1794 2021-08-06 13:55:34.000000 soursop-0.2.4/soursop/tests/test_caps.py
+-rw-r--r--   0 alex       (501) staff       (20)     1658 2021-08-06 13:56:07.000000 soursop-0.2.4/soursop/tests/test_numbering.py
+-rw-r--r--   0 alex       (501) staff       (20)     1676 2021-08-06 13:52:22.000000 soursop-0.2.4/soursop/tests/test_soursop.py
+-rw-r--r--   0 alex       (501) staff       (20)      874 2022-06-23 16:18:42.000000 soursop-0.2.4/soursop/tests/test_ssmutual_information.py
+-rw-r--r--   0 alex       (501) staff       (20)    10216 2021-08-06 13:55:07.000000 soursop-0.2.4/soursop/tests/test_ssnmr.py
+-rw-r--r--   0 alex       (501) staff       (20)     1413 2021-08-06 13:56:36.000000 soursop-0.2.4/soursop/tests/test_ssnmr_extended.py
+-rw-r--r--   0 alex       (501) staff       (20)     1266 2023-01-07 17:19:45.000000 soursop-0.2.4/soursop/tests/test_sspre.py
+-rw-r--r--   0 alex       (501) staff       (20)    39061 2023-02-11 16:29:23.000000 soursop-0.2.4/soursop/tests/test_ssproteins.py
+-rw-r--r--   0 alex       (501) staff       (20)    24723 2022-04-18 00:15:08.000000 soursop-0.2.4/soursop/tests/test_sstrajectory.py
+-rw-r--r--   0 alex       (501) staff       (20)     1384 2022-06-07 04:54:17.000000 soursop-0.2.4/soursop/tests/test_ssutils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-31 02:58:43.860809 soursop-0.2.4/soursop.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     5358 2023-07-31 02:58:43.000000 soursop-0.2.4/soursop.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2787 2023-07-31 02:58:43.000000 soursop-0.2.4/soursop.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-31 02:58:43.000000 soursop-0.2.4/soursop.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       84 2023-07-31 02:58:43.000000 soursop-0.2.4/soursop.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        8 2023-07-31 02:58:43.000000 soursop-0.2.4/soursop.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)    81180 2022-06-07 04:54:17.000000 soursop-0.2.4/versioneer.py
```

### Comparing `soursop-0.2.3/LICENSE` & `soursop-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/PKG-INFO` & `soursop-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: soursop
-Version: 0.2.3
-Summary: UNKNOWN
+Version: 0.2.4
 Home-page: https://github.com/holehouse-lab/soursop
 Author: Alex Holehouse
 Author-email: alex.holehouse@wustl.edu
 License: LGPLv3
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 SOURSOP
 ==============================
 [![Build Status](https://github.com/jaredl7/soursop/actions/workflows/soursop-ci.yml/badge.svg?branch=master)](https://github.com/jaredl7/soursop/actions)
 [![codecov](https://codecov.io/gh/jaredl7/soursop/branch/master/graph/badge.svg?token=RHGII0235L)](https://codecov.io/gh/jaredl7/soursop)
 [![Documentation Status](https://readthedocs.org/projects/soursop/badge/?version=latest)](https://soursop.readthedocs.io/en/latest/?badge=latest)
 ## ABOUT
 SOURSOP is a Python-based simulation analysis package for working with intrinsically disordered and unfolded proteins. It is built on top of [mdtraj](https://mdtraj.org/), and was developed by Jared Lalmansingh and Alex Holehouse. 
 
-The current stable release candidate on PyPI is 0.2.3 (Feb 2023).
+The current stable release candidate on PyPI is 0.2.4 (July 2023).
 
 ## DOCUMENTATION
 All documentation, including installation information [can be found here](https://soursop.readthedocs.io/). 
 
 ## ERRORS, FEATURES, REQUESTS
 If you find a bug, typo, or error [please raise an issue or GitHub](https://github.com/holehouse-lab/soursop/issues).
 
 If you wish to add a new feature, please see our Development information in the docs (especially for adding plugins).
 
 ## MISCELLANEOUS
-* As of right now, the continuous integration fails because of a specific mismatch in how an edge-case error is handled between different versions of mdtraj. All other tests are passing and SOURSOP is ready for production.
+* As of right now, the continuous integration fails because of a specific mismatch in how an edge-case error is handled between different versions of mdtraj. All other tests are passing and SOURSOP is ready for production. Do not be alarmed by the `failing` status above!
 
-## PREPRINT
-To read about SOURSOP please see our preprint:
+## PUBLICATION
+To read about SOURSOP please see our paper:
+
+Lalmansingh, J. M., Keeley, A. T., Ruff, K. M., Pappu, R. V. & Holehouse, A. S. SOURSOP: A Python Package for the Analysis of Simulations of Intrinsically Disordered Proteins. J. Chem. Theory Comput. (2023). doi:10.1021/acs.jctc.3c00190
+
+* [Journal link](https://pubs.acs.org/doi/full/10.1021/acs.jctc.3c00190)
+* [Paper PDF](https://www.dropbox.com/s/bd5szapvxpn83r6/soursop_jctc.pdf?dl=0)
 
-**SOURSOP: A Python package for the analysis of simulations of intrinsically disordered proteins**
 
-Jared Lalmansingh, Alex Keeley, Kiersten Ruff, Rohit Pappu, Alex Holehouse
 
 
 #### Copyright
 Copyright (c) 2015-2023 under the GNU LESSER GENERAL PUBLIC LICENSE 
 
 # Changelog
+#### Update July 2023
+* Added in `explicit_residue_checking` flag into SSTrajectory constructor, which makes it possible to use a solvated `.gro` file as an input file.
+
 #### Update February 2023
 * Added plugins example
 * Added additional tests and finalized documentation
 
 #### Update July 2022
 For version 0.2.1 we introduce potentially breaking changes into how COM distances are reported. 
 
@@ -71,9 +75,7 @@
 
 #### Update May 2019
 This is the *development* repository of CAMPARITraj and SHOULD NOT be used for production. Seriously, it is being modified constantly and with no building requirements during code pushes. If you want a building copy PLEASE contact Alex directly! [last touched June 24th 2019].
 
 #### Acknowledgements
 Project based on the
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.0.
-
-
```

### Comparing `soursop-0.2.3/README.md` & `soursop-0.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,39 +2,45 @@
 ==============================
 [![Build Status](https://github.com/jaredl7/soursop/actions/workflows/soursop-ci.yml/badge.svg?branch=master)](https://github.com/jaredl7/soursop/actions)
 [![codecov](https://codecov.io/gh/jaredl7/soursop/branch/master/graph/badge.svg?token=RHGII0235L)](https://codecov.io/gh/jaredl7/soursop)
 [![Documentation Status](https://readthedocs.org/projects/soursop/badge/?version=latest)](https://soursop.readthedocs.io/en/latest/?badge=latest)
 ## ABOUT
 SOURSOP is a Python-based simulation analysis package for working with intrinsically disordered and unfolded proteins. It is built on top of [mdtraj](https://mdtraj.org/), and was developed by Jared Lalmansingh and Alex Holehouse. 
 
-The current stable release candidate on PyPI is 0.2.3 (Feb 2023).
+The current stable release candidate on PyPI is 0.2.4 (July 2023).
 
 ## DOCUMENTATION
 All documentation, including installation information [can be found here](https://soursop.readthedocs.io/). 
 
 ## ERRORS, FEATURES, REQUESTS
 If you find a bug, typo, or error [please raise an issue or GitHub](https://github.com/holehouse-lab/soursop/issues).
 
 If you wish to add a new feature, please see our Development information in the docs (especially for adding plugins).
 
 ## MISCELLANEOUS
-* As of right now, the continuous integration fails because of a specific mismatch in how an edge-case error is handled between different versions of mdtraj. All other tests are passing and SOURSOP is ready for production.
+* As of right now, the continuous integration fails because of a specific mismatch in how an edge-case error is handled between different versions of mdtraj. All other tests are passing and SOURSOP is ready for production. Do not be alarmed by the `failing` status above!
 
-## PREPRINT
-To read about SOURSOP please see our preprint:
+## PUBLICATION
+To read about SOURSOP please see our paper:
+
+Lalmansingh, J. M., Keeley, A. T., Ruff, K. M., Pappu, R. V. & Holehouse, A. S. SOURSOP: A Python Package for the Analysis of Simulations of Intrinsically Disordered Proteins. J. Chem. Theory Comput. (2023). doi:10.1021/acs.jctc.3c00190
+
+* [Journal link](https://pubs.acs.org/doi/full/10.1021/acs.jctc.3c00190)
+* [Paper PDF](https://www.dropbox.com/s/bd5szapvxpn83r6/soursop_jctc.pdf?dl=0)
 
-**SOURSOP: A Python package for the analysis of simulations of intrinsically disordered proteins**
 
-Jared Lalmansingh, Alex Keeley, Kiersten Ruff, Rohit Pappu, Alex Holehouse
 
 
 #### Copyright
 Copyright (c) 2015-2023 under the GNU LESSER GENERAL PUBLIC LICENSE 
 
 # Changelog
+#### Update July 2023
+* Added in `explicit_residue_checking` flag into SSTrajectory constructor, which makes it possible to use a solvated `.gro` file as an input file.
+
 #### Update February 2023
 * Added plugins example
 * Added additional tests and finalized documentation
 
 #### Update July 2022
 For version 0.2.1 we introduce potentially breaking changes into how COM distances are reported.
```

### Comparing `soursop-0.2.3/setup.py` & `soursop-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/__init__.py` & `soursop-0.2.4/soursop/__init__.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/_internal_data.py` & `soursop-0.2.4/soursop/_internal_data.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/configs.py` & `soursop-0.2.4/soursop/configs.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/SASA_SUMMARY.csv` & `soursop-0.2.4/soursop/data/SASA_SUMMARY.csv`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/bbseg2.dat` & `soursop-0.2.4/soursop/data/bbseg2.dat`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/all_residues.pdb` & `soursop-0.2.4/soursop/data/test_data/all_residues.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/all_residues.xtc` & `soursop-0.2.4/soursop/data/test_data/all_residues.xtc`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/ACD_start_1.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/ACD_start_1.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/ACD_start_10.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/ACD_start_10.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_NH2.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_NH2.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_NME.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_NME.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_NME_multichain.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_NME_multichain.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_NME_start_at_5.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_NME_start_at_5.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/ACE_UCAP.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/ACE_UCAP.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/FOR_NH2.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/FOR_NH2.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/FOR_NME.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/FOR_NME.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/FOR_UCAP.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/FOR_UCAP.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/UCAP_NH2.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/UCAP_NH2.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/UCAP_NME.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/UCAP_NME.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/UCAP_UCAP.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/UCAP_UCAP.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/cap_tests/__START.pdb` & `soursop-0.2.4/soursop/data/test_data/cap_tests/__START.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/ctl9.pdb` & `soursop-0.2.4/soursop/data/test_data/ctl9.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/ctl9.xtc` & `soursop-0.2.4/soursop/data/test_data/ctl9.xtc`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/gromacs1chain/top.pdb` & `soursop-0.2.4/soursop/data/test_data/gromacs1chain/top.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/gromacs1chain/traj.xtc` & `soursop-0.2.4/soursop/data/test_data/gromacs1chain/traj.xtc`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/gromacs2chains/top.pdb` & `soursop-0.2.4/soursop/data/test_data/gromacs2chains/top.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/gromacs2chains/traj.xtc` & `soursop-0.2.4/soursop/data/test_data/gromacs2chains/traj.xtc`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/gs6.dcd` & `soursop-0.2.4/soursop/data/test_data/gs6.dcd`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/gs6.pdb` & `soursop-0.2.4/soursop/data/test_data/gs6.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/gs6.xtc` & `soursop-0.2.4/soursop/data/test_data/gs6.xtc`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/gs6_invalid_r1.pdb` & `soursop-0.2.4/soursop/data/test_data/gs6_invalid_r1.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/ntl9.dcd` & `soursop-0.2.4/soursop/data/test_data/ntl9.dcd`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/ntl9.pdb` & `soursop-0.2.4/soursop/data/test_data/ntl9.pdb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/ntl9.xtc` & `soursop-0.2.4/soursop/data/test_data/ntl9.xtc`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/pre_data/PRE_109_unweighted.csv` & `soursop-0.2.4/soursop/data/test_data/pre_data/PRE_109_unweighted.csv`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/pre_data/PRE_119_unweighted.csv` & `soursop-0.2.4/soursop/data/test_data/pre_data/PRE_119_unweighted.csv`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/pre_data/PRE_149_unweighted.csv` & `soursop-0.2.4/soursop/data/test_data/pre_data/PRE_149_unweighted.csv`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/pre_data/PRE_61_unweighted.csv` & `soursop-0.2.4/soursop/data/test_data/pre_data/PRE_61_unweighted.csv`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/pre_data/PRE_74_unweighted.csv` & `soursop-0.2.4/soursop/data/test_data/pre_data/PRE_74_unweighted.csv`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/data/test_data/pre_data/PRE_96_unweighted.csv` & `soursop-0.2.4/soursop/data/test_data/pre_data/PRE_96_unweighted.csv`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/plugins/sparrow_plugin/__init__.py` & `soursop-0.2.4/soursop/plugins/sparrow_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/soursop.py` & `soursop-0.2.4/soursop/soursop.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/ssdata.py` & `soursop-0.2.4/soursop/ssdata.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/ssexceptions.py` & `soursop-0.2.4/soursop/ssexceptions.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/ssio.py` & `soursop-0.2.4/soursop/ssio.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/ssmutualinformation.py` & `soursop-0.2.4/soursop/ssmutualinformation.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/ssnmr.py` & `soursop-0.2.4/soursop/ssnmr.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/sspolymer.py` & `soursop-0.2.4/soursop/sspolymer.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/sspre.py` & `soursop-0.2.4/soursop/sspre.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/ssprotein.py` & `soursop-0.2.4/soursop/ssprotein.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/sstools.py` & `soursop-0.2.4/soursop/sstools.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/sstrajectory.py` & `soursop-0.2.4/soursop/sstrajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,22 @@
 
 
 class SSTrajectory:
 
     #oxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxo
     #
     #
-    def __init__(self, trajectory_filename=None, pdb_filename=None, TRJ=None, protein_grouping=None, pdblead=False, debug=False, extra_valid_residue_names=None):
+    def __init__(self, trajectory_filename=None,
+                 pdb_filename=None,
+                 TRJ=None,
+                 protein_grouping=None,
+                 pdblead=False,
+                 debug=False,
+                 extra_valid_residue_names=None,
+                 explicit_residue_checking=False):
         
         """
         SSTrajectory is the class used to read in a work with simulation
         trajectories in SOURSOP.
 
         There are two ways new SSTrajectory objects can be generated;
 
@@ -114,14 +121,27 @@
                         
             This keyword allows the user to pass a list of ADDITIONAL residues 
             that we want SOURSOP to recognize as valid residues to extract a 
             chain as a protein molecule. This can be especially useful if you 
             want to trick SOURSOP into analyzing polymer simulations where your 
             PDB file may have non-standard residue names (e.g., XXX).
 
+        explicit_residue_checking : bool
+            In early versions of SOURSOP we operate under the assumption that 
+            every residue in a chain will be protein if the first residue is 
+            a protein. In general this is a good assumption, especially because
+            it means we can implicitly deal with non-standard residue names that
+            are internal to a chain. However, if you're reading in a .gro file, or
+            any kind of topology file that lacks explicit chains, then any 
+            non-protein residues end up being brought in and counted which if you
+            have 10000s of solvent molecules makes parsing impossible. If 
+            explicit_residue_checking is set to True, then each residue in each
+            chain is explicitly checked, meaning solvent molecules/atoms in 
+            a single chain are discarded.
+
 
         Example
         -----------
         Example of reading in an XTC trajectory file::
 
             from soursop.sstrajectory import SSTrajectory
 
@@ -156,19 +176,19 @@
             self.traj = self.__readTrajectory(trajectory_filename, pdb_filename, pdblead)
 
 
         # Next, having read in the trajectory we parse out into proteins
         # extract a list of protein trajectories where each protein is assumed
         # to be in its own chain
         if protein_grouping == None:
-            self.proteinTrajectoryList = self.__get_proteins(self.traj, debug)        
+            self.proteinTrajectoryList = self.__get_proteins(self.traj, debug, explicit_residue_checking=explicit_residue_checking)        
         else:
             self.proteinTrajectoryList = self.__get_proteins_by_residue(self.traj, protein_grouping, debug)
 
-        self.__single_protein_traj = self.__get_all_proteins(self.traj)
+        self.__single_protein_traj = self.__get_all_proteins(self.traj, explicit_residue_checking=explicit_residue_checking)
 
 
     def  __repr__(self):
         return "SSTrajectory (%s): %i proteins and %i frames" % (hex(id(self)), self.n_proteins, self.n_frames)
 
 
     def __len__(self):
@@ -278,15 +298,15 @@
                                                                            
         return traj
 
 
     #oxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxo
     #
     #
-    def __get_all_proteins(self, trajectory):
+    def __get_all_proteins(self, trajectory, explicit_residue_checking=False):
         """
         Internal function that builds a single trajectory which contains all protein
         residues. 
 
         Parameters
         -----------
         trajectory : mdtraj.Trajectory
@@ -306,35 +326,55 @@
         protein_atoms = []
         
         # for each chain in this toplogy determine if the 
         # first residue is protein or not. If it's protein we parse it if 
         # not it gets skipped
         for chain in topology.chains:
 
-            # if the first residue in the chain is protein
-            # note that a formic acid cap ('FOR') is not recognized as protein
-            # so we include an edgecase here for that
-            if chain.residue(0).name in self.valid_residue_names:
 
-                # intialize an empty list of atoms
+            
+            # if explicit residue checking is False we assume the first residue of the
+            # chain is representative of the whole chain. This is generally
+            # fair assumption
+            if explicit_residue_checking is False:
+                
+                if chain.residue(0).name in self.valid_residue_names:
+
+                    # intialize an empty list of atoms
+                    local_atoms = []
+
+                    # get every atom in this chain
+                    for atom in chain.atoms:
+                        protein_atoms.append(atom.index)
+
+                    protein_atoms.extend(local_atoms)
+            else:
+                
+                # initialize an empty list of atoms
                 local_atoms = []
+                
+                for res in chain.residues:
 
-                # get every atom in this chain
-                for atom in chain.atoms:
-                    protein_atoms.append(atom.index)
+                    # for each residue in that chain ask if that residue is valid
+                    if res.name in self.valid_residue_names:
+
+                        # if yes 
+                        local_atoms.extend([a.index for a in res.atoms])
 
                 protein_atoms.extend(local_atoms)
 
+            
+
         return SSProtein(trajectory.atom_slice(protein_atoms))
         
 
     #oxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxoxoxoxoxoxoxoxoxoxooxoxo
     #
     #
-    def __get_proteins(self, trajectory, debug):
+    def __get_proteins(self, trajectory, debug, explicit_residue_checking=False):
         """
         Internal function that takes an MDTraj trajectory and returns a list 
         of mdtraj trajectory objects corresponding to each protein in the 
         system, ASSUMING that each protein is in its own chain.
         
         The way this works is to cycle through each chain, identify if that 
         chain contains protein or not, and if it does grab all the atoms in 
@@ -361,32 +401,50 @@
         chainAtoms = []
         
         # for each chain in this toplogy determine if the 
         # first residue is protein or not. If it's protein we parse it if 
         # not it gets skipped
         for chain in topology.chains:
 
-            # if the first residue in the chain is protein
-            # note that a formic acid cap ('FOR') is not recognized as protein
-            # so we include an edgecase here for that
-            if chain.residue(0).name in self.valid_residue_names:
 
-                # intialize an empty list of atoms
-                local_atoms = []
+            # if hybrid chains is False we assume the first residue of the
+            # chain is representative of the whole chain. This is generally
+            # fair assumption
+            if explicit_residue_checking is False:
+                # if the first residue in the chain is protein
+                # so we include an edgecase here for that
+                if chain.residue(0).name in self.valid_residue_names:
+                
+                    # intialize an empty list of atoms
+                    local_atoms = []
 
-                # get every atom in this chain
-                for atom in chain.atoms:
-                    local_atoms.append(atom.index)
+                    # get every atom in this chain
+                    for atom in chain.atoms:
+                        local_atoms.append(atom.index)
+
+                    chainAtoms.append(local_atoms)
+
+                else:
+                    if debug:
+                        ssio.debug_message('Skipping residue %s from %s' %(chain.residue(0).name, chain))
+            else:
 
-                chainAtoms.append(local_atoms)
+                # initialize an empty list of atoms
+                local_atoms = []
+                
+                for res in chain.residues:
 
-            else:
-                if debug:
-                    ssio.debug_message('Skipping residue %s from %s' %(chain.residue(0).name, chain))
+                    # for each residue in that chain ask if that residue is valid
+                    if res.name in self.valid_residue_names:
+
+                        # if yes 
+                        local_atoms.extend([a.index for a in res.atoms])
 
+                chainAtoms.append(local_atoms)
+                    
         # for each protein chain that we have atomic indices
         # for (hopefully all of them!) cycle through and create
         # sub-trajectories
         proteinTrajectoryList = []
         for local_chain_atoms in chainAtoms:
 
             # generate a trajectory composed of *JUST* the
```

### Comparing `soursop-0.2.3/soursop/ssutils.py` & `soursop-0.2.4/soursop/ssutils.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/.ipynb_checkpoints/test_scratchpad-checkpoint.ipynb` & `soursop-0.2.4/soursop/tests/.ipynb_checkpoints/test_scratchpad-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/conftest.py` & `soursop-0.2.4/soursop/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_caps.py` & `soursop-0.2.4/soursop/tests/test_caps.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_numbering.py` & `soursop-0.2.4/soursop/tests/test_numbering.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_soursop.py` & `soursop-0.2.4/soursop/tests/test_soursop.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_ssmutual_information.py` & `soursop-0.2.4/soursop/tests/test_ssmutual_information.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_ssnmr.py` & `soursop-0.2.4/soursop/tests/test_ssnmr.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_ssnmr_extended.py` & `soursop-0.2.4/soursop/tests/test_ssnmr_extended.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_sspre.py` & `soursop-0.2.4/soursop/tests/test_sspre.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_ssproteins.py` & `soursop-0.2.4/soursop/tests/test_ssproteins.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_sstrajectory.py` & `soursop-0.2.4/soursop/tests/test_sstrajectory.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop/tests/test_ssutils.py` & `soursop-0.2.4/soursop/tests/test_ssutils.py`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/soursop.egg-info/PKG-INFO` & `soursop-0.2.4/soursop.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: soursop
-Version: 0.2.3
-Summary: UNKNOWN
+Version: 0.2.4
 Home-page: https://github.com/holehouse-lab/soursop
 Author: Alex Holehouse
 Author-email: alex.holehouse@wustl.edu
 License: LGPLv3
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 SOURSOP
 ==============================
 [![Build Status](https://github.com/jaredl7/soursop/actions/workflows/soursop-ci.yml/badge.svg?branch=master)](https://github.com/jaredl7/soursop/actions)
 [![codecov](https://codecov.io/gh/jaredl7/soursop/branch/master/graph/badge.svg?token=RHGII0235L)](https://codecov.io/gh/jaredl7/soursop)
 [![Documentation Status](https://readthedocs.org/projects/soursop/badge/?version=latest)](https://soursop.readthedocs.io/en/latest/?badge=latest)
 ## ABOUT
 SOURSOP is a Python-based simulation analysis package for working with intrinsically disordered and unfolded proteins. It is built on top of [mdtraj](https://mdtraj.org/), and was developed by Jared Lalmansingh and Alex Holehouse. 
 
-The current stable release candidate on PyPI is 0.2.3 (Feb 2023).
+The current stable release candidate on PyPI is 0.2.4 (July 2023).
 
 ## DOCUMENTATION
 All documentation, including installation information [can be found here](https://soursop.readthedocs.io/). 
 
 ## ERRORS, FEATURES, REQUESTS
 If you find a bug, typo, or error [please raise an issue or GitHub](https://github.com/holehouse-lab/soursop/issues).
 
 If you wish to add a new feature, please see our Development information in the docs (especially for adding plugins).
 
 ## MISCELLANEOUS
-* As of right now, the continuous integration fails because of a specific mismatch in how an edge-case error is handled between different versions of mdtraj. All other tests are passing and SOURSOP is ready for production.
+* As of right now, the continuous integration fails because of a specific mismatch in how an edge-case error is handled between different versions of mdtraj. All other tests are passing and SOURSOP is ready for production. Do not be alarmed by the `failing` status above!
 
-## PREPRINT
-To read about SOURSOP please see our preprint:
+## PUBLICATION
+To read about SOURSOP please see our paper:
+
+Lalmansingh, J. M., Keeley, A. T., Ruff, K. M., Pappu, R. V. & Holehouse, A. S. SOURSOP: A Python Package for the Analysis of Simulations of Intrinsically Disordered Proteins. J. Chem. Theory Comput. (2023). doi:10.1021/acs.jctc.3c00190
+
+* [Journal link](https://pubs.acs.org/doi/full/10.1021/acs.jctc.3c00190)
+* [Paper PDF](https://www.dropbox.com/s/bd5szapvxpn83r6/soursop_jctc.pdf?dl=0)
 
-**SOURSOP: A Python package for the analysis of simulations of intrinsically disordered proteins**
 
-Jared Lalmansingh, Alex Keeley, Kiersten Ruff, Rohit Pappu, Alex Holehouse
 
 
 #### Copyright
 Copyright (c) 2015-2023 under the GNU LESSER GENERAL PUBLIC LICENSE 
 
 # Changelog
+#### Update July 2023
+* Added in `explicit_residue_checking` flag into SSTrajectory constructor, which makes it possible to use a solvated `.gro` file as an input file.
+
 #### Update February 2023
 * Added plugins example
 * Added additional tests and finalized documentation
 
 #### Update July 2022
 For version 0.2.1 we introduce potentially breaking changes into how COM distances are reported. 
 
@@ -71,9 +75,7 @@
 
 #### Update May 2019
 This is the *development* repository of CAMPARITraj and SHOULD NOT be used for production. Seriously, it is being modified constantly and with no building requirements during code pushes. If you want a building copy PLEASE contact Alex directly! [last touched June 24th 2019].
 
 #### Acknowledgements
 Project based on the
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.0.
-
-
```

### Comparing `soursop-0.2.3/soursop.egg-info/SOURCES.txt` & `soursop-0.2.4/soursop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soursop-0.2.3/versioneer.py` & `soursop-0.2.4/versioneer.py`

 * *Files identical despite different names*


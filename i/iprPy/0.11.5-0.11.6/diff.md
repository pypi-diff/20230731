# Comparing `tmp/iprPy-0.11.5.tar.gz` & `tmp/iprPy-0.11.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\iprPy\dist\.tmp-qrolqopu\iprPy-0.11.5.tar", last modified: Tue Apr 18 20:31:01 2023, max compression
+gzip compressed data, was "iprPy-0.11.6.tar", last modified: Mon Jul 31 21:07:13 2023, max compression
```

## Comparing `iprPy-0.11.5.tar` & `iprPy-0.11.6.tar`

### file list

```diff
@@ -1,417 +1,418 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/
--rw-rw-rw-   0        0        0     2776 2019-07-10 17:30:09.000000 iprPy-0.11.5/LICENSE.TXT
--rw-rw-rw-   0        0        0      181 2021-09-14 19:12:36.000000 iprPy-0.11.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2584 2023-04-18 20:31:01.000000 iprPy-0.11.5/PKG-INFO
--rw-rw-rw-   0        0        0     1779 2022-07-22 14:05:14.000000 iprPy-0.11.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/bin/
--rw-rw-rw-   0        0        0     3216 2022-06-01 13:45:46.000000 iprPy-0.11.5/bin/README.rst
--rw-rw-rw-   0        0        0     7371 2022-05-23 16:10:36.000000 iprPy-0.11.5/bin/check_runners.py
--rw-rw-rw-   0        0        0      148 2020-07-31 19:29:10.000000 iprPy-0.11.5/bin/iprPy
--rw-rw-rw-   0        0        0      341 2022-04-07 17:25:44.000000 iprPy-0.11.5/bin/iprPy_prepare
--rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/iprPy_prepare_pool_1
--rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/iprPy_prepare_pool_2
--rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/iprPy_prepare_pool_3
--rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/iprPy_prepare_pool_4
--rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/iprPy_prepare_pool_5
--rw-rw-rw-   0        0        0      289 2021-01-07 21:36:18.000000 iprPy-0.11.5/bin/iprPy_slurm
--rw-rw-rw-   0        0        0      291 2021-01-07 21:36:18.000000 iprPy-0.11.5/bin/iprPy_slurm_16
--rw-rw-rw-   0        0        0      289 2021-01-07 21:36:18.000000 iprPy-0.11.5/bin/iprPy_slurm_4
--rw-rw-rw-   0        0        0      289 2021-01-07 21:36:18.000000 iprPy-0.11.5/bin/iprPy_slurm_8
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/bin/prepare/
--rw-rw-rw-   0        0        0     3155 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/prepare/master_prepare_ctcms.in
--rw-rw-rw-   0        0        0     1965 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_1.in
--rw-rw-rw-   0        0        0     1950 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_2.in
--rw-rw-rw-   0        0        0     1939 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_3.in
--rw-rw-rw-   0        0        0     2044 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_4.in
--rw-rw-rw-   0        0        0     1988 2022-10-04 13:35:04.000000 iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_5.in
--rw-rw-rw-   0        0        0     3041 2022-05-23 16:10:36.000000 iprPy-0.11.5/bin/prepare/master_prepare_desktop.in
--rw-rw-rw-   0        0        0     2996 2022-04-26 15:37:32.000000 iprPy-0.11.5/bin/prepare/master_prepare_desktop_wsl.in
--rw-rw-rw-   0        0        0     7160 2022-10-17 16:30:15.000000 iprPy-0.11.5/bin/prepare_relax_dynamic_at_temp.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/
--rw-rw-rw-   0        0        0     6271 2023-04-07 15:29:07.000000 iprPy-0.11.5/iprPy/Settings.py
--rw-rw-rw-   0        0        0        6 2023-04-18 20:29:48.000000 iprPy-0.11.5/iprPy/VERSION
--rw-rw-rw-   0        0        0     1169 2023-04-07 15:19:20.000000 iprPy-0.11.5/iprPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/analysis/
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/
--rw-rw-rw-   0        0        0    10425 2022-11-18 21:22:35.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/__init__.py
--rw-rw-rw-   0        0        0     4276 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_crystal.py
--rw-rw-rw-   0        0        0    12591 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_diatom.py
--rw-rw-rw-   0        0        0     7155 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_elastic.py
--rw-rw-rw-   0        0        0     2155 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_empty.py
--rw-rw-rw-   0        0        0    12580 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_evsr.py
--rw-rw-rw-   0        0        0    26217 2023-04-11 18:57:57.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_phonon.py
--rw-rw-rw-   0        0        0     8958 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_point.py
--rw-rw-rw-   0        0        0    11840 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_stacking.py
--rw-rw-rw-   0        0        0     5958 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_surface.py
--rw-rw-rw-   0        0        0      283 2022-11-18 20:44:32.000000 iprPy-0.11.5/iprPy/analysis/__init__.py
--rw-rw-rw-   0        0        0     4931 2022-05-23 16:10:36.000000 iprPy-0.11.5/iprPy/analysis/get_isolated_atom_energies.py
--rw-rw-rw-   0        0        0     3054 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/analysis/match_reference_prototype.py
--rw-rw-rw-   0        0        0    48139 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/analysis/process_relaxations.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/analysis/thermo/
--rw-rw-rw-   0        0        0     5112 2022-11-18 20:42:40.000000 iprPy-0.11.5/iprPy/analysis/thermo/AnalyzeFE.py
--rw-rw-rw-   0        0        0     4590 2023-04-07 14:34:12.000000 iprPy-0.11.5/iprPy/analysis/thermo/AnalyzeMD.py
--rw-rw-rw-   0        0        0     3912 2022-11-18 20:43:35.000000 iprPy-0.11.5/iprPy/analysis/thermo/AnalyzeQHA.py
--rw-rw-rw-   0        0        0      102 2022-11-18 20:44:06.000000 iprPy-0.11.5/iprPy/analysis/thermo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/
--rw-rw-rw-   0        0        0    29258 2023-04-11 18:36:26.000000 iprPy-0.11.5/iprPy/calculation/Calculation.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/
--rw-rw-rw-   0        0        0    21892 2023-04-11 18:48:44.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/EvsRScan.py
--rw-rw-rw-   0        0        0     1725 2022-03-10 16:52:33.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/README.md
--rw-rw-rw-   0        0        0       92 2020-07-31 15:20:45.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/__init__.py
--rw-rw-rw-   0        0        0      275 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan.xsd
--rw-rw-rw-   0        0        0     4925 2022-07-27 14:05:09.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan.xsl
--rw-rw-rw-   0        0        0     3160 2022-07-27 14:04:58.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan_short.xsl
--rw-rw-rw-   0        0        0     5982 2022-03-04 18:07:19.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/e_vs_r_scan.py
--rw-rw-rw-   0        0        0      269 2019-11-25 20:53:45.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/run0.template
--rw-rw-rw-   0        0        0      570 2020-09-22 22:04:08.000000 iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/theory.md
--rw-rw-rw-   0        0        0     3524 2022-10-04 19:31:01.000000 iprPy-0.11.5/iprPy/calculation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/
--rw-rw-rw-   0        0        0    94770 2020-07-29 18:48:37.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/Bain.ipynb
--rw-rw-rw-   0        0        0     7362 2020-08-19 22:39:20.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/Bain.py
--rw-rw-rw-   0        0        0     3352 2020-09-25 16:28:16.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/BainTransformationMap.py
--rw-rw-rw-   0        0        0      131 2020-07-31 15:18:16.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/__init__.py
--rw-rw-rw-   0        0        0    10690 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calc_bain_transformation_map.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/
--rw-rw-rw-   0        0        0     5486 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/CalculationBainTransformationMap.py
--rw-rw-rw-   0        0        0      980 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/README.md
--rw-rw-rw-   0        0        0      160 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/__init__.py
--rw-rw-rw-   0        0        0      287 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/record-calculation-bain-transformation-map.xsd
--rw-rw-rw-   0        0        0     2908 2016-09-16 16:31:10.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/data_model.py
--rw-rw-rw-   0        0        0      409 2020-07-29 18:48:37.000000 iprPy-0.11.5/iprPy/calculation/bain_transformation_map/min.template
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/
--rw-rw-rw-   0        0        0    26044 2023-04-11 18:41:38.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/BondAngleScan.py
--rw-rw-rw-   0        0        0      735 2021-04-02 19:28:45.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/README.md
--rw-rw-rw-   0        0        0      107 2021-04-02 19:34:59.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/__init__.py
--rw-rw-rw-   0        0        0     5097 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/bond_angle_scan.py
--rw-rw-rw-   0        0        0     2355 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/bond_scan.template
--rw-rw-rw-   0        0        0      279 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/calculation_bond_angle_scan.xsd
--rw-rw-rw-   0        0        0     3255 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/prepare_bond_angle_scan.py
--rw-rw-rw-   0        0        0      902 2021-04-02 19:56:56.000000 iprPy-0.11.5/iprPy/calculation/bond_angle_scan/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/crystal_space_group/
--rw-rw-rw-   0        0        0    23286 2023-04-11 18:41:45.000000 iprPy-0.11.5/iprPy/calculation/crystal_space_group/CrystalSpaceGroup.py
--rw-rw-rw-   0        0        0     1453 2022-03-10 16:52:45.000000 iprPy-0.11.5/iprPy/calculation/crystal_space_group/README.md
--rw-rw-rw-   0        0        0      119 2020-07-31 15:20:32.000000 iprPy-0.11.5/iprPy/calculation/crystal_space_group/__init__.py
--rw-rw-rw-   0        0        0      283 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/crystal_space_group/calculation_crystal_space_group.xsd
--rw-rw-rw-   0        0        0     5703 2022-03-10 18:43:15.000000 iprPy-0.11.5/iprPy/calculation/crystal_space_group/crystal_space_group.py
--rw-rw-rw-   0        0        0      463 2020-09-22 21:59:57.000000 iprPy-0.11.5/iprPy/calculation/crystal_space_group/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/
--rw-rw-rw-   0        0        0    19871 2023-04-11 18:41:49.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/DiatomScan.py
--rw-rw-rw-   0        0        0     1077 2022-02-16 18:54:28.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/README.md
--rw-rw-rw-   0        0        0       98 2020-07-31 15:18:45.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/__init__.py
--rw-rw-rw-   0        0        0      275 2021-09-14 18:07:38.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/calculation_diatom_scan.xsd
--rw-rw-rw-   0        0        0     4566 2022-07-27 13:47:53.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/calculation_diatom_scan.xsl
--rw-rw-rw-   0        0        0     2817 2022-07-27 13:49:28.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/calculation_diatom_scan_short.xsl
--rw-rw-rw-   0        0        0     4392 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/diatom_scan.py
--rw-rw-rw-   0        0        0      174 2019-11-25 20:53:45.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/run0.template
--rw-rw-rw-   0        0        0     1377 2020-09-22 22:00:40.000000 iprPy-0.11.5/iprPy/calculation/diatom_scan/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/
--rw-rw-rw-   0        0        0    41247 2023-04-11 18:48:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/DislocationSDVPN.py
--rw-rw-rw-   0        0        0     1828 2022-03-10 16:53:15.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/README.md
--rw-rw-rw-   0        0        0      116 2020-07-31 15:20:42.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/__init__.py
--rw-rw-rw-   0        0        0      281 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/calculation_dislocation_SDVPN.xsd
--rw-rw-rw-   0        0        0     8557 2022-03-11 20:18:23.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/dislocation_SDVPN.py
--rw-rw-rw-   0        0        0      324 2020-09-22 22:03:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/
--rw-rw-rw-   0        0        0      673 2017-12-15 01:46:29.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/README.md
--rw-rw-rw-   0        0        0     1725 2018-06-27 13:54:23.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/__init__.py
--rw-rw-rw-   0        0        0     7475 2018-04-09 16:15:16.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calc_dislocation_Peierls_Nabarro_stress.py
--rw-rw-rw-   0        0        0     1066 2017-12-15 01:43:48.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calc_dislocation_Peierls_Nabarro_stress.template
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/
--rw-rw-rw-   0        0        0     1060 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/README.md
--rw-rw-rw-   0        0        0      401 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/__init__.py
--rw-rw-rw-   0        0        0     4832 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/buildmodel.py
--rw-rw-rw-   0        0        0     1141 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/compare_terms.py
--rw-rw-rw-   0        0        0      298 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/record-calculation-dislocation-Peierls-Nabarro-stress.xsd
--rw-rw-rw-   0        0        0      515 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/schema.py
--rw-rw-rw-   0        0        0     3664 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/todict.py
--rw-rw-rw-   0        0        0    26459 2017-07-24 22:29:09.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/dislocation_Peierls_Nabarro_stress_template.ipynb
--rw-rw-rw-   0        0        0     9722 2018-04-11 20:14:48.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/prepare_dislocation_Peierls_Nabarro_stress.py
--rw-rw-rw-   0        0        0       24 2017-12-14 22:04:14.000000 iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole/
--rw-rw-rw-   0        0        0    27276 2023-04-11 18:41:52.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole/DislocationMonopole.py
--rw-rw-rw-   0        0        0     2534 2022-03-10 16:52:53.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole/README.md
--rw-rw-rw-   0        0        0      125 2020-07-31 15:19:29.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole/__init__.py
--rw-rw-rw-   0        0        0      284 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole/calculation_dislocation_monopole.xsd
--rw-rw-rw-   0        0        0      439 2020-08-27 19:35:19.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole/disl_relax.template
--rw-rw-rw-   0        0        0    18549 2022-03-08 15:33:29.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole/dislocation_monopole.py
--rw-rw-rw-   0        0        0     3519 2020-09-22 22:01:26.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/
--rw-rw-rw-   0        0        0      161 2018-06-27 14:18:08.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/__init__.py
--rw-rw-rw-   0        0        0     1062 2021-02-26 18:52:18.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/calc_crss.template
--rw-rw-rw-   0        0        0    18416 2021-03-03 17:27:38.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/calc_dislocation_monopole_crss.py
--rw-rw-rw-   0        0        0     4133 2016-10-25 14:41:24.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/data_model.py
--rw-rw-rw-   0        0        0    15473 2016-10-25 14:41:24.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/prepare.py
--rw-rw-rw-   0        0        0     4089 2016-10-25 14:41:24.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/read_input.py
--rw-rw-rw-   0        0        0     3199 2021-02-26 18:52:21.000000 iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/strain_system.template
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/
--rw-rw-rw-   0        0        0    28345 2023-04-11 18:41:59.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/DislocationPeriodicArray.py
--rw-rw-rw-   0        0        0     1284 2022-03-10 16:55:13.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/README.md
--rw-rw-rw-   0        0        0      140 2020-07-31 15:19:40.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/__init__.py
--rw-rw-rw-   0        0        0      290 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/calculation_dislocation_periodic_array.xsd
--rw-rw-rw-   0        0        0      439 2020-08-27 19:35:33.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/disl_relax.template
--rw-rw-rw-   0        0        0    18993 2022-03-08 15:37:40.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/dislocation_periodic_array.py
--rw-rw-rw-   0        0        0     3573 2020-09-22 22:02:12.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/
--rw-rw-rw-   0        0        0     2548 2019-07-10 17:30:46.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/DislocationPeriodicArrayStress.py
--rw-rw-rw-   0        0        0     1603 2019-07-10 17:30:46.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/README.md
--rw-rw-rw-   0        0        0      279 2019-07-22 15:37:51.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/__init__.py
--rw-rw-rw-   0        0        0    12411 2019-07-29 16:01:17.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calc_dislocation_periodic_array_stress.py
--rw-rw-rw-   0        0        0     1337 2019-07-10 17:30:46.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calc_dislocation_periodic_array_stress.template
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/
--rw-rw-rw-   0        0        0     6824 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/CalculationDislocationPeriodicArrayStress.py
--rw-rw-rw-   0        0        0      818 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/README.md
--rw-rw-rw-   0        0        0      215 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/__init__.py
--rw-rw-rw-   0        0        0      297 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/record-calculation-dislocation-periodic-array-stress.xsd
--rw-rw-rw-   0        0        0     1944 2019-07-10 17:30:46.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/dislarray_free_stress.template
--rw-rw-rw-   0        0        0     2158 2019-07-10 17:30:46.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/dislarray_rigid_stress.template
--rw-rw-rw-   0        0        0     3573 2019-07-10 17:30:46.000000 iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/
--rw-rw-rw-   0        0        0      161 2019-07-22 15:38:08.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/
--rw-rw-rw-   0        0        0     3101 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/522c8437-eceb-480d-8f0c-77f83cdb3125.json
--rw-rw-rw-   0        0        0   795421 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/base.dat
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc/
--rw-rw-rw-   0        0        0      765 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc/110-edge.json
--rw-rw-rw-   0        0        0      768 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc/111-screw.json
--rw-rw-rw-   0        0        0      765 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc/112-edge.json
--rw-rw-rw-   0        0        0     4399 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc.json
--rw-rw-rw-   0        0        0      963 2016-09-16 16:31:10.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.in
--rw-rw-rw-   0        0        0     1211 2016-09-16 16:31:10.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.py
--rw-rw-rw-   0        0        0     1355 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.template
--rw-rw-rw-   0        0        0      822 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/create_sys.in
--rw-rw-rw-   0        0        0   795381 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl.dat
--rw-rw-rw-   0        0        0  1095015 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl.dump
--rw-rw-rw-   0        0        0      948 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax.in
--rw-rw-rw-   0        0        0      733 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax.template
--rw-rw-rw-   0        0        0      477 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax_notemp.template
--rw-rw-rw-   0        0        0     1913 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax_script.py
--rw-rw-rw-   0        0        0     4177 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/fcc.json
--rw-rw-rw-   0        0        0     4725 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/log.lammps
--rw-rw-rw-   0        0        0     4273 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/results.json
--rw-rw-rw-   0        0        0     3773 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/data_model.py
--rw-rw-rw-   0        0        0    11136 2016-06-21 13:43:04.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/prepare.py
--rw-rw-rw-   0        0        0     3762 2016-09-16 16:31:10.000000 iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/read_input.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/
--rw-rw-rw-   0        0        0      629 2018-06-27 14:18:20.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/__init__.py
--rw-rw-rw-   0        0        0     1365 2017-03-16 13:24:41.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.in
--rw-rw-rw-   0        0        0    29440 2022-10-04 13:35:04.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.py
--rw-rw-rw-   0        0        0     1416 2017-02-17 17:13:16.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.template
--rw-rw-rw-   0        0        0      591 2017-02-13 20:46:19.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/full_relax.template
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_static/
--rw-rw-rw-   0        0        0    17145 2023-04-11 18:48:47.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_static/ElasticConstantsStatic.py
--rw-rw-rw-   0        0        0     1884 2022-03-10 16:52:22.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_static/README.md
--rw-rw-rw-   0        0        0      134 2020-07-31 15:20:28.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_static/__init__.py
--rw-rw-rw-   0        0        0      288 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_static/calculation_elastic_constants_static.xsd
--rw-rw-rw-   0        0        0     3343 2021-01-29 17:33:30.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_static/cij.template
--rw-rw-rw-   0        0        0     8251 2022-03-07 20:09:20.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_static/elastic_constants_static.py
--rw-rw-rw-   0        0        0     1363 2020-09-22 22:04:58.000000 iprPy-0.11.5/iprPy/calculation/elastic_constants_static/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/energy_check/
--rw-rw-rw-   0        0        0     9182 2023-04-11 18:49:09.000000 iprPy-0.11.5/iprPy/calculation/energy_check/EnergyCheck.py
--rw-rw-rw-   0        0        0      636 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/energy_check/README.md
--rw-rw-rw-   0        0        0       99 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/energy_check/__init__.py
--rw-rw-rw-   0        0        0      276 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/energy_check/calculation_energy_check.xsd
--rw-rw-rw-   0        0        0     2160 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/energy_check/energy_check.py
--rw-rw-rw-   0        0        0      269 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/energy_check/run0.template
--rw-rw-rw-   0        0        0      230 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/calculation/energy_check/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/free_energy/
--rw-rw-rw-   0        0        0    27755 2023-04-11 18:49:23.000000 iprPy-0.11.5/iprPy/calculation/free_energy/FreeEnergy.py
--rw-rw-rw-   0        0        0      804 2022-09-20 17:22:25.000000 iprPy-0.11.5/iprPy/calculation/free_energy/README.md
--rw-rw-rw-   0        0        0       77 2022-09-20 17:05:23.000000 iprPy-0.11.5/iprPy/calculation/free_energy/__init__.py
--rw-rw-rw-   0        0        0      275 2022-09-20 17:22:26.000000 iprPy-0.11.5/iprPy/calculation/free_energy/calculation_free_energy.xsd
--rw-rw-rw-   0        0        0    16471 2022-09-20 17:22:39.000000 iprPy-0.11.5/iprPy/calculation/free_energy/free_energy.py
--rw-rw-rw-   0        0        0     1053 2022-09-20 15:32:26.000000 iprPy-0.11.5/iprPy/calculation/free_energy/free_energy.template
--rw-rw-rw-   0        0        0      609 2022-09-19 15:15:23.000000 iprPy-0.11.5/iprPy/calculation/free_energy/msd.template
--rw-rw-rw-   0        0        0      766 2022-09-20 17:22:13.000000 iprPy-0.11.5/iprPy/calculation/free_energy/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/
--rw-rw-rw-   0        0        0    25588 2023-04-11 18:49:32.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/FreeEnergyLiquid.py
--rw-rw-rw-   0        0        0      962 2022-10-18 17:47:07.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/README.md
--rw-rw-rw-   0        0        0    76625 2022-10-26 16:32:59.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/UhlenbeckFordModel.py
--rw-rw-rw-   0        0        0       95 2022-10-18 17:43:55.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/__init__.py
--rw-rw-rw-   0        0        0      282 2022-10-18 17:42:30.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/calculation_free_energy_liquid.xsd
--rw-rw-rw-   0        0        0    11975 2022-10-19 18:31:36.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/free_energy_liquid.py
--rw-rw-rw-   0        0        0     1186 2022-10-19 16:40:06.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/free_energy_liquid.template
--rw-rw-rw-   0        0        0      766 2022-09-20 17:22:13.000000 iprPy-0.11.5/iprPy/calculation/free_energy_liquid/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/
--rw-rw-rw-   0        0        0      638 2018-06-27 14:18:00.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/__init__.py
--rw-rw-rw-   0        0        0    11732 2017-03-13 18:10:32.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/calc_bcc_grain_boundary.py
--rw-rw-rw-   0        0        0     1252 2016-12-30 23:01:13.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/calc_bcc_grain_boundary.template
--rw-rw-rw-   0        0        0     2059 2016-12-30 22:37:08.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/grain_boundary.template
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_search/
--rw-rw-rw-   0        0        0     1020 2017-05-01 19:00:38.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_search/README.md
--rw-rw-rw-   0        0        0       97 2018-06-27 14:18:33.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_search/__init__.py
--rw-rw-rw-   0        0        0      525 2017-07-06 18:31:53.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_search/compare_terms.py
--rw-rw-rw-   0        0        0      285 2016-12-31 00:03:23.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_search/record-calculation-grain-boundary-search.xsd
--rw-rw-rw-   0        0        0      158 2017-05-03 19:21:57.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_search/schema.py
--rw-rw-rw-   0        0        0     1469 2017-05-03 19:22:32.000000 iprPy-0.11.5/iprPy/calculation/grain_boundary_search/todict.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/
--rw-rw-rw-   0        0        0    11570 2023-04-11 18:49:40.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/IsolatedAtom.py
--rw-rw-rw-   0        0        0     1059 2022-03-10 16:52:15.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/README.md
--rw-rw-rw-   0        0        0      127 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/__init__.py
--rw-rw-rw-   0        0        0      277 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/calculation_isolated_atom.xsd
--rw-rw-rw-   0        0        0     2405 2022-07-26 20:19:39.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/calculation_isolated_atom.xsl
--rw-rw-rw-   0        0        0      469 2022-07-19 16:35:37.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/calculation_isolated_atom_short.xsl
--rw-rw-rw-   0        0        0     2725 2022-03-07 20:08:50.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/isolated_atom.py
--rw-rw-rw-   0        0        0      174 2020-07-29 18:48:37.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/run0.template
--rw-rw-rw-   0        0        0      955 2020-09-22 22:05:46.000000 iprPy-0.11.5/iprPy/calculation/isolated_atom/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/phonon/
--rw-rw-rw-   0        0        0    30125 2023-04-11 18:57:57.000000 iprPy-0.11.5/iprPy/calculation/phonon/Phonon.py
--rw-rw-rw-   0        0        0      794 2022-03-10 16:52:05.000000 iprPy-0.11.5/iprPy/calculation/phonon/README.md
--rw-rw-rw-   0        0        0       86 2020-07-31 15:21:30.000000 iprPy-0.11.5/iprPy/calculation/phonon/__init__.py
--rw-rw-rw-   0        0        0    16969 2023-04-18 20:04:30.000000 iprPy-0.11.5/iprPy/calculation/phonon/calc_phonon.py
--rw-rw-rw-   0        0        0      270 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/phonon/calculation_phonon.xsd
--rw-rw-rw-   0        0        0      298 2020-12-21 15:35:11.000000 iprPy-0.11.5/iprPy/calculation/phonon/phonon.template
--rw-rw-rw-   0        0        0      780 2019-07-26 17:47:07.000000 iprPy-0.11.5/iprPy/calculation/phonon/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/
--rw-rw-rw-   0        0        0    30411 2023-04-11 18:50:11.000000 iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/PointDefectDiffusion.py
--rw-rw-rw-   0        0        0     1213 2022-03-10 16:53:46.000000 iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/README.md
--rw-rw-rw-   0        0        0      128 2020-07-31 15:21:39.000000 iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/__init__.py
--rw-rw-rw-   0        0        0      286 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/calculation_point_defect_diffusion.xsd
--rw-rw-rw-   0        0        0     1144 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/diffusion.template
--rw-rw-rw-   0        0        0     9991 2022-03-07 20:41:33.000000 iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/point_defect_diffusion.py
--rw-rw-rw-   0        0        0     1462 2019-07-26 17:49:39.000000 iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/point_defect_static/
--rw-rw-rw-   0        0        0    24890 2023-04-11 18:50:23.000000 iprPy-0.11.5/iprPy/calculation/point_defect_static/PointDefectStatic.py
--rw-rw-rw-   0        0        0     2080 2022-03-10 16:51:46.000000 iprPy-0.11.5/iprPy/calculation/point_defect_static/README.md
--rw-rw-rw-   0        0        0      119 2020-07-31 15:22:45.000000 iprPy-0.11.5/iprPy/calculation/point_defect_static/__init__.py
--rw-rw-rw-   0        0        0      283 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/point_defect_static/calculation_point_defect_static.xsd
--rw-rw-rw-   0        0        0      427 2021-01-07 21:36:18.000000 iprPy-0.11.5/iprPy/calculation/point_defect_static/min.template
--rw-rw-rw-   0        0        0    18254 2022-03-10 20:44:04.000000 iprPy-0.11.5/iprPy/calculation/point_defect_static/point_defect_static.py
--rw-rw-rw-   0        0        0     3954 2019-07-26 19:10:33.000000 iprPy-0.11.5/iprPy/calculation/point_defect_static/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/relax_box/
--rw-rw-rw-   0        0        0     1485 2022-03-10 16:51:20.000000 iprPy-0.11.5/iprPy/calculation/relax_box/README.md
--rw-rw-rw-   0        0        0    30864 2023-04-11 18:50:36.000000 iprPy-0.11.5/iprPy/calculation/relax_box/RelaxBox.py
--rw-rw-rw-   0        0        0       92 2020-07-31 15:22:51.000000 iprPy-0.11.5/iprPy/calculation/relax_box/__init__.py
--rw-rw-rw-   0        0        0      273 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/relax_box/calculation_relax_box.xsd
--rw-rw-rw-   0        0        0     4352 2021-10-20 21:24:11.000000 iprPy-0.11.5/iprPy/calculation/relax_box/cij_run0.template
--rw-rw-rw-   0        0        0    17154 2022-03-07 17:38:17.000000 iprPy-0.11.5/iprPy/calculation/relax_box/relax_box.py
--rw-rw-rw-   0        0        0     1570 2020-09-22 22:06:42.000000 iprPy-0.11.5/iprPy/calculation/relax_box/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/
--rw-rw-rw-   0        0        0     2295 2022-03-10 16:50:31.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/README.md
--rw-rw-rw-   0        0        0    53007 2023-04-11 18:50:53.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/RelaxDynamic.py
--rw-rw-rw-   0        0        0      104 2020-07-31 15:22:56.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/__init__.py
--rw-rw-rw-   0        0        0      277 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/calculation_relax_dynamic.xsd
--rw-rw-rw-   0        0        0      577 2022-03-08 18:15:11.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/full_relax.template
--rw-rw-rw-   0        0        0      570 2022-03-08 18:32:01.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/full_relax_restart.template
--rw-rw-rw-   0        0        0    20476 2022-05-23 16:10:36.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/relax_dynamic.py
--rw-rw-rw-   0        0        0     2051 2020-09-22 22:07:08.000000 iprPy-0.11.5/iprPy/calculation/relax_dynamic/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/
--rw-rw-rw-   0        0        0     1423 2022-10-14 17:45:58.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/README.md
--rw-rw-rw-   0        0        0    45155 2023-04-18 20:04:30.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/RelaxLiquid.py
--rw-rw-rw-   0        0        0      101 2022-10-11 12:17:29.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/__init__.py
--rw-rw-rw-   0        0        0      276 2022-10-11 19:15:07.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/calculation_relax_liquid.xsd
--rw-rw-rw-   0        0        0     3099 2022-11-02 19:22:40.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/liquid_ave_pe.template
--rw-rw-rw-   0        0        0     3044 2022-11-02 19:22:47.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/liquid_ave_te.template
--rw-rw-rw-   0        0        0    14797 2022-11-02 17:44:12.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/relax_liquid.py
--rw-rw-rw-   0        0        0     5838 2022-10-15 13:24:08.000000 iprPy-0.11.5/iprPy/calculation/relax_liquid/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/relax_static/
--rw-rw-rw-   0        0        0     1137 2022-03-10 16:50:26.000000 iprPy-0.11.5/iprPy/calculation/relax_static/README.md
--rw-rw-rw-   0        0        0    34926 2023-04-11 18:51:08.000000 iprPy-0.11.5/iprPy/calculation/relax_static/RelaxStatic.py
--rw-rw-rw-   0        0        0      101 2020-07-31 15:23:02.000000 iprPy-0.11.5/iprPy/calculation/relax_static/__init__.py
--rw-rw-rw-   0        0        0      276 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/relax_static/calculation_relax_static.xsd
--rw-rw-rw-   0        0        0      552 2020-07-29 18:48:37.000000 iprPy-0.11.5/iprPy/calculation/relax_static/minbox.template
--rw-rw-rw-   0        0        0    11585 2022-03-07 17:03:22.000000 iprPy-0.11.5/iprPy/calculation/relax_static/relax_static.py
--rw-rw-rw-   0        0        0      555 2020-09-22 22:07:34.000000 iprPy-0.11.5/iprPy/calculation/relax_static/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/
--rw-rw-rw-   0        0        0     1128 2022-03-10 16:54:23.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/README.md
--rw-rw-rw-   0        0        0    21441 2023-04-11 18:51:20.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/StackingFaultMap2D.py
--rw-rw-rw-   0        0        0      122 2020-07-31 15:23:08.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/__init__.py
--rw-rw-rw-   0        0        0      285 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/calculation_stacking_fault_map_2D.xsd
--rw-rw-rw-   0        0        0      482 2020-08-18 13:49:57.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/sfmin.template
--rw-rw-rw-   0        0        0    15829 2022-03-07 20:57:51.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/stacking_fault_map_2D.py
--rw-rw-rw-   0        0        0     3050 2020-09-22 22:08:55.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_static/
--rw-rw-rw-   0        0        0     1013 2022-03-10 16:54:46.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_static/README.md
--rw-rw-rw-   0        0        0    18699 2023-04-11 18:51:33.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_static/StackingFaultStatic.py
--rw-rw-rw-   0        0        0      125 2020-07-31 15:23:15.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_static/__init__.py
--rw-rw-rw-   0        0        0      285 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_static/calculation_stacking_fault_static.xsd
--rw-rw-rw-   0        0        0      482 2020-08-18 13:49:56.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_static/sfmin.template
--rw-rw-rw-   0        0        0    17048 2022-03-07 20:57:52.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_static/stacking_fault_static.py
--rw-rw-rw-   0        0        0     2829 2020-09-22 22:09:25.000000 iprPy-0.11.5/iprPy/calculation/stacking_fault_static/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation/surface_energy_static/
--rw-rw-rw-   0        0        0     1159 2022-03-10 16:54:57.000000 iprPy-0.11.5/iprPy/calculation/surface_energy_static/README.md
--rw-rw-rw-   0        0        0    17361 2023-04-11 18:51:51.000000 iprPy-0.11.5/iprPy/calculation/surface_energy_static/SurfaceEnergyStatic.py
--rw-rw-rw-   0        0        0      125 2020-07-31 15:23:22.000000 iprPy-0.11.5/iprPy/calculation/surface_energy_static/__init__.py
--rw-rw-rw-   0        0        0      285 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/calculation/surface_energy_static/calculation_surface_energy_static.xsd
--rw-rw-rw-   0        0        0      408 2020-08-18 13:49:53.000000 iprPy-0.11.5/iprPy/calculation/surface_energy_static/min.template
--rw-rw-rw-   0        0        0    12968 2022-03-10 20:44:03.000000 iprPy-0.11.5/iprPy/calculation/surface_energy_static/surface_energy_static.py
--rw-rw-rw-   0        0        0     1844 2020-09-22 22:10:07.000000 iprPy-0.11.5/iprPy/calculation/surface_energy_static/theory.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/calculation_subset/
--rw-rw-rw-   0        0        0    14400 2023-04-10 17:16:00.000000 iprPy-0.11.5/iprPy/calculation_subset/AtommanElasticConstants.py
--rw-rw-rw-   0        0        0     8647 2023-04-10 17:16:10.000000 iprPy-0.11.5/iprPy/calculation_subset/AtommanGammaSurface.py
--rw-rw-rw-   0        0        0    26242 2023-04-10 17:16:23.000000 iprPy-0.11.5/iprPy/calculation_subset/AtommanSystemLoad.py
--rw-rw-rw-   0        0        0    21641 2023-04-10 17:16:40.000000 iprPy-0.11.5/iprPy/calculation_subset/AtommanSystemManipulate.py
--rw-rw-rw-   0        0        0     8322 2023-04-08 17:04:04.000000 iprPy-0.11.5/iprPy/calculation_subset/CalculationSubset.py
--rw-rw-rw-   0        0        0    35750 2023-04-10 17:17:51.000000 iprPy-0.11.5/iprPy/calculation_subset/Dislocation.py
--rw-rw-rw-   0        0        0    23748 2023-04-10 17:17:32.000000 iprPy-0.11.5/iprPy/calculation_subset/FreeSurface.py
--rw-rw-rw-   0        0        0     9644 2023-04-10 17:16:46.000000 iprPy-0.11.5/iprPy/calculation_subset/LammpsCommands.py
--rw-rw-rw-   0        0        0    14048 2023-04-10 17:16:53.000000 iprPy-0.11.5/iprPy/calculation_subset/LammpsMinimize.py
--rw-rw-rw-   0        0        0    15229 2023-04-10 17:17:13.000000 iprPy-0.11.5/iprPy/calculation_subset/LammpsPotential.py
--rw-rw-rw-   0        0        0    21964 2023-04-10 17:19:16.000000 iprPy-0.11.5/iprPy/calculation_subset/PointDefect.py
--rw-rw-rw-   0        0        0    28989 2023-04-10 17:18:02.000000 iprPy-0.11.5/iprPy/calculation_subset/StackingFault.py
--rw-rw-rw-   0        0        0     7119 2023-04-10 17:02:30.000000 iprPy-0.11.5/iprPy/calculation_subset/Units.py
--rw-rw-rw-   0        0        0      617 2023-04-07 16:02:15.000000 iprPy-0.11.5/iprPy/calculation_subset/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-07 15:12:34.000000 iprPy-0.11.5/iprPy/check_modules.py
--rw-rw-rw-   0        0        0    21218 2023-04-07 15:17:36.000000 iprPy-0.11.5/iprPy/command_line.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/database/
--rw-rw-rw-   0        0        0      235 2022-05-23 16:10:37.000000 iprPy-0.11.5/iprPy/database/CDCSDatabase.py
--rw-rw-rw-   0        0        0    26668 2022-05-23 16:10:37.000000 iprPy-0.11.5/iprPy/database/IprPyDatabase.py
--rw-rw-rw-   0        0        0      238 2022-05-23 16:10:37.000000 iprPy-0.11.5/iprPy/database/LocalDatabase.py
--rw-rw-rw-   0        0        0     1642 2022-05-23 16:10:37.000000 iprPy-0.11.5/iprPy/database/MongoDatabase.py
--rw-rw-rw-   0        0        0     1892 2022-05-23 16:10:37.000000 iprPy-0.11.5/iprPy/database/__init__.py
--rw-rw-rw-   0        0        0     1061 2022-02-15 16:32:45.000000 iprPy-0.11.5/iprPy/database/load_database.py
--rw-rw-rw-   0        0        0     5800 2022-04-07 17:25:44.000000 iprPy-0.11.5/iprPy/database/master_prepare.py
--rw-rw-rw-   0        0        0    16414 2022-10-20 11:33:59.000000 iprPy-0.11.5/iprPy/database/prepare.py
--rw-rw-rw-   0        0        0     1817 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/database/reset_orphans.py
--rw-rw-rw-   0        0        0    24405 2022-02-15 16:01:52.000000 iprPy-0.11.5/iprPy/database/runner.py
--rw-rw-rw-   0        0        0     3812 2023-04-07 15:08:49.000000 iprPy-0.11.5/iprPy/fix_lammps_versions.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/input/
--rw-rw-rw-   0        0        0      391 2022-03-03 22:02:42.000000 iprPy-0.11.5/iprPy/input/__init__.py
--rw-rw-rw-   0        0        0      980 2022-03-03 22:15:35.000000 iprPy-0.11.5/iprPy/input/boolean.py
--rw-rw-rw-   0        0        0     1220 2022-03-03 22:05:53.000000 iprPy-0.11.5/iprPy/input/buildcombos.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/
--rw-rw-rw-   0        0        0     5918 2019-07-24 15:27:46.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/README.rst
--rw-rw-rw-   0        0        0      471 2022-03-03 22:19:43.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/__init__.py
--rw-rw-rw-   0        0        0     6741 2022-03-03 22:42:59.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/atomicarchive.py
--rw-rw-rw-   0        0        0     7120 2022-03-03 22:40:49.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/atomicparent.py
--rw-rw-rw-   0        0        0     7354 2022-03-03 22:42:55.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/atomicreference.py
--rw-rw-rw-   0        0        0     6477 2022-03-03 22:41:53.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/crystalprototype.py
--rw-rw-rw-   0        0        0     3097 2022-03-03 22:38:23.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/defect.py
--rw-rw-rw-   0        0        0     3450 2022-03-03 22:38:35.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/diatom.py
--rw-rw-rw-   0        0        0     3057 2022-03-03 22:38:30.000000 iprPy-0.11.5/iprPy/input/buildcombos_functions/lammpspotential.py
--rw-rw-rw-   0        0        0     4050 2022-03-03 22:15:33.000000 iprPy-0.11.5/iprPy/input/parse.py
--rw-rw-rw-   0        0        0     2015 2022-03-03 22:18:09.000000 iprPy-0.11.5/iprPy/input/termtodict.py
--rw-rw-rw-   0        0        0     1698 2022-03-03 22:19:18.000000 iprPy-0.11.5/iprPy/input/value.py
--rw-rw-rw-   0        0        0     1335 2023-04-07 15:07:09.000000 iprPy-0.11.5/iprPy/load_run_directory.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/record/
--rw-rw-rw-   0        0        0    12587 2023-04-07 15:33:56.000000 iprPy-0.11.5/iprPy/record/PotentialProperties.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/
--rw-rw-rw-   0        0        0     5535 2022-06-01 13:45:46.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/CrystalStructure.py
--rw-rw-rw-   0        0        0     1305 2022-02-15 16:01:52.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/DiatomScan.py
--rw-rw-rw-   0        0        0     5317 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/ElasticConstants.py
--rw-rw-rw-   0        0        0     1805 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/EvsRScan.py
--rw-rw-rw-   0        0        0     3847 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/FreeSurface.py
--rw-rw-rw-   0        0        0     6255 2023-04-11 18:57:57.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/Phonon.py
--rw-rw-rw-   0        0        0     4598 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/PointDefect.py
--rw-rw-rw-   0        0        0     1025 2023-03-07 17:45:11.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/PotentialsPropertiesSubset.py
--rw-rw-rw-   0        0        0     6241 2022-07-11 18:42:14.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/StackingFault.py
--rw-rw-rw-   0        0        0      308 2022-11-18 21:23:15.000000 iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/__init__.py
--rw-rw-rw-   0        0        0      322 2023-04-07 15:52:13.000000 iprPy-0.11.5/iprPy/record/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/record/xsd/
--rw-rw-rw-   0        0        0        0 2021-09-14 18:07:39.000000 iprPy-0.11.5/iprPy/record/xsd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:01.000000 iprPy-0.11.5/iprPy/tools/
--rw-rw-rw-   0        0        0      574 2022-11-18 20:44:52.000000 iprPy-0.11.5/iprPy/tools/__init__.py
--rw-rw-rw-   0        0        0     1910 2023-04-07 15:21:37.000000 iprPy-0.11.5/iprPy/tools/dict_insert.py
--rw-rw-rw-   0        0        0     1934 2022-03-03 21:50:13.000000 iprPy-0.11.5/iprPy/tools/dynamic_import.py
--rw-rw-rw-   0        0        0     1679 2023-04-07 15:22:17.000000 iprPy-0.11.5/iprPy/tools/num_deriv_3_point.py
--rw-rw-rw-   0        0        0      746 2023-04-07 15:23:02.000000 iprPy-0.11.5/iprPy/tools/read_calc_file.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy.egg-info/
--rw-rw-rw-   0        0        0     2584 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18763 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2019-07-10 18:55:45.000000 iprPy-0.11.5/iprPy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       89 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 20:31:00.000000 iprPy-0.11.5/iprPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-03 20:26:52.000000 iprPy-0.11.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 20:31:01.000000 iprPy-0.11.5/setup.cfg
--rw-rw-rw-   0        0        0     1846 2023-04-18 20:01:28.000000 iprPy-0.11.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.429928 iprPy-0.11.6/
+-rw-rw-rw-   0        0        0     2776 2019-07-10 17:30:09.000000 iprPy-0.11.6/LICENSE.TXT
+-rw-rw-rw-   0        0        0      181 2021-09-14 19:12:36.000000 iprPy-0.11.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2533 2023-07-31 21:07:13.428928 iprPy-0.11.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1779 2022-07-22 14:05:14.000000 iprPy-0.11.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.816927 iprPy-0.11.6/bin/
+-rw-rw-rw-   0        0        0     3216 2022-06-01 13:45:46.000000 iprPy-0.11.6/bin/README.rst
+-rw-rw-rw-   0        0        0     7371 2022-05-23 16:10:36.000000 iprPy-0.11.6/bin/check_runners.py
+-rw-rw-rw-   0        0        0      148 2020-07-31 19:29:10.000000 iprPy-0.11.6/bin/iprPy
+-rw-rw-rw-   0        0        0      341 2022-04-07 17:25:44.000000 iprPy-0.11.6/bin/iprPy_prepare
+-rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/iprPy_prepare_pool_1
+-rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/iprPy_prepare_pool_2
+-rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/iprPy_prepare_pool_3
+-rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/iprPy_prepare_pool_4
+-rw-rw-rw-   0        0        0      289 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/iprPy_prepare_pool_5
+-rw-rw-rw-   0        0        0      289 2021-01-07 21:36:18.000000 iprPy-0.11.6/bin/iprPy_slurm
+-rw-rw-rw-   0        0        0      291 2021-01-07 21:36:18.000000 iprPy-0.11.6/bin/iprPy_slurm_16
+-rw-rw-rw-   0        0        0      289 2021-01-07 21:36:18.000000 iprPy-0.11.6/bin/iprPy_slurm_4
+-rw-rw-rw-   0        0        0      289 2021-01-07 21:36:18.000000 iprPy-0.11.6/bin/iprPy_slurm_8
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.832928 iprPy-0.11.6/bin/prepare/
+-rw-rw-rw-   0        0        0     3155 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/prepare/master_prepare_ctcms.in
+-rw-rw-rw-   0        0        0     1965 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_1.in
+-rw-rw-rw-   0        0        0     1950 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_2.in
+-rw-rw-rw-   0        0        0     1939 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_3.in
+-rw-rw-rw-   0        0        0     2044 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_4.in
+-rw-rw-rw-   0        0        0     1988 2022-10-04 13:35:04.000000 iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_5.in
+-rw-rw-rw-   0        0        0     3041 2022-05-23 16:10:36.000000 iprPy-0.11.6/bin/prepare/master_prepare_desktop.in
+-rw-rw-rw-   0        0        0     2996 2022-04-26 15:37:32.000000 iprPy-0.11.6/bin/prepare/master_prepare_desktop_wsl.in
+-rw-rw-rw-   0        0        0     7160 2022-10-17 16:30:15.000000 iprPy-0.11.6/bin/prepare_relax_dynamic_at_temp.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.845927 iprPy-0.11.6/iprPy/
+-rw-rw-rw-   0        0        0     6271 2023-04-07 15:29:07.000000 iprPy-0.11.6/iprPy/Settings.py
+-rw-rw-rw-   0        0        0        6 2023-07-31 15:18:02.000000 iprPy-0.11.6/iprPy/VERSION
+-rw-rw-rw-   0        0        0     1335 2023-07-27 20:23:13.000000 iprPy-0.11.6/iprPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.865929 iprPy-0.11.6/iprPy/analysis/
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.885929 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/
+-rw-rw-rw-   0        0        0    10425 2022-11-18 21:22:35.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/__init__.py
+-rw-rw-rw-   0        0        0     4276 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_crystal.py
+-rw-rw-rw-   0        0        0    12591 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_diatom.py
+-rw-rw-rw-   0        0        0     7155 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_elastic.py
+-rw-rw-rw-   0        0        0     2155 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_empty.py
+-rw-rw-rw-   0        0        0    12580 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_evsr.py
+-rw-rw-rw-   0        0        0    26217 2023-04-11 18:57:57.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_phonon.py
+-rw-rw-rw-   0        0        0     8958 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_point.py
+-rw-rw-rw-   0        0        0    11840 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_stacking.py
+-rw-rw-rw-   0        0        0     5958 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_surface.py
+-rw-rw-rw-   0        0        0      283 2022-11-18 20:44:32.000000 iprPy-0.11.6/iprPy/analysis/__init__.py
+-rw-rw-rw-   0        0        0     4931 2022-05-23 16:10:36.000000 iprPy-0.11.6/iprPy/analysis/get_isolated_atom_energies.py
+-rw-rw-rw-   0        0        0     3054 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/analysis/match_reference_prototype.py
+-rw-rw-rw-   0        0        0    48139 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/analysis/process_relaxations.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.892928 iprPy-0.11.6/iprPy/analysis/thermo/
+-rw-rw-rw-   0        0        0     5112 2022-11-18 20:42:40.000000 iprPy-0.11.6/iprPy/analysis/thermo/AnalyzeFE.py
+-rw-rw-rw-   0        0        0     4590 2023-04-07 14:34:12.000000 iprPy-0.11.6/iprPy/analysis/thermo/AnalyzeMD.py
+-rw-rw-rw-   0        0        0     3912 2022-11-18 20:43:35.000000 iprPy-0.11.6/iprPy/analysis/thermo/AnalyzeQHA.py
+-rw-rw-rw-   0        0        0      102 2022-11-18 20:44:06.000000 iprPy-0.11.6/iprPy/analysis/thermo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.895927 iprPy-0.11.6/iprPy/calculation/
+-rw-rw-rw-   0        0        0    29595 2023-05-31 18:04:41.000000 iprPy-0.11.6/iprPy/calculation/Calculation.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.912927 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/
+-rw-rw-rw-   0        0        0    22264 2023-05-31 18:05:56.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/EvsRScan.py
+-rw-rw-rw-   0        0        0     1725 2022-03-10 16:52:33.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/README.md
+-rw-rw-rw-   0        0        0       92 2020-07-31 15:20:45.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/__init__.py
+-rw-rw-rw-   0        0        0      275 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan.xsd
+-rw-rw-rw-   0        0        0     4925 2022-07-27 14:05:09.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan.xsl
+-rw-rw-rw-   0        0        0     3160 2022-07-27 14:04:58.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan_short.xsl
+-rw-rw-rw-   0        0        0     5982 2022-03-04 18:07:19.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/e_vs_r_scan.py
+-rw-rw-rw-   0        0        0      269 2019-11-25 20:53:45.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/run0.template
+-rw-rw-rw-   0        0        0      570 2020-09-22 22:04:08.000000 iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/theory.md
+-rw-rw-rw-   0        0        0     3524 2022-10-04 19:31:01.000000 iprPy-0.11.6/iprPy/calculation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.925928 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/
+-rw-rw-rw-   0        0        0    94770 2020-07-29 18:48:37.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/Bain.ipynb
+-rw-rw-rw-   0        0        0     7362 2020-08-19 22:39:20.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/Bain.py
+-rw-rw-rw-   0        0        0     3352 2020-09-25 16:28:16.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/BainTransformationMap.py
+-rw-rw-rw-   0        0        0      131 2020-07-31 15:18:16.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/__init__.py
+-rw-rw-rw-   0        0        0    10690 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calc_bain_transformation_map.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.932927 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/
+-rw-rw-rw-   0        0        0     5486 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/CalculationBainTransformationMap.py
+-rw-rw-rw-   0        0        0      980 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/README.md
+-rw-rw-rw-   0        0        0      160 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/__init__.py
+-rw-rw-rw-   0        0        0      287 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/record-calculation-bain-transformation-map.xsd
+-rw-rw-rw-   0        0        0     2908 2016-09-16 16:31:10.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/data_model.py
+-rw-rw-rw-   0        0        0      409 2020-07-29 18:48:37.000000 iprPy-0.11.6/iprPy/calculation/bain_transformation_map/min.template
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.945927 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/
+-rw-rw-rw-   0        0        0    26416 2023-05-31 18:05:06.000000 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/BondAngleScan.py
+-rw-rw-rw-   0        0        0      735 2021-04-02 19:28:45.000000 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/README.md
+-rw-rw-rw-   0        0        0      107 2021-04-02 19:34:59.000000 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/__init__.py
+-rw-rw-rw-   0        0        0     5097 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/bond_angle_scan.py
+-rw-rw-rw-   0        0        0     2355 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/bond_scan.template
+-rw-rw-rw-   0        0        0      279 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/calculation_bond_angle_scan.xsd
+-rw-rw-rw-   0        0        0     3255 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/prepare_bond_angle_scan.py
+-rw-rw-rw-   0        0        0      902 2021-04-02 19:56:56.000000 iprPy-0.11.6/iprPy/calculation/bond_angle_scan/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.954927 iprPy-0.11.6/iprPy/calculation/crystal_space_group/
+-rw-rw-rw-   0        0        0    23658 2023-05-31 18:05:21.000000 iprPy-0.11.6/iprPy/calculation/crystal_space_group/CrystalSpaceGroup.py
+-rw-rw-rw-   0        0        0     1453 2022-03-10 16:52:45.000000 iprPy-0.11.6/iprPy/calculation/crystal_space_group/README.md
+-rw-rw-rw-   0        0        0      119 2020-07-31 15:20:32.000000 iprPy-0.11.6/iprPy/calculation/crystal_space_group/__init__.py
+-rw-rw-rw-   0        0        0      283 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/crystal_space_group/calculation_crystal_space_group.xsd
+-rw-rw-rw-   0        0        0     5703 2022-03-10 18:43:15.000000 iprPy-0.11.6/iprPy/calculation/crystal_space_group/crystal_space_group.py
+-rw-rw-rw-   0        0        0      463 2020-09-22 21:59:57.000000 iprPy-0.11.6/iprPy/calculation/crystal_space_group/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.967927 iprPy-0.11.6/iprPy/calculation/diatom_scan/
+-rw-rw-rw-   0        0        0    20243 2023-05-31 18:05:29.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/DiatomScan.py
+-rw-rw-rw-   0        0        0     1077 2022-02-16 18:54:28.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/README.md
+-rw-rw-rw-   0        0        0       98 2020-07-31 15:18:45.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/__init__.py
+-rw-rw-rw-   0        0        0      275 2021-09-14 18:07:38.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/calculation_diatom_scan.xsd
+-rw-rw-rw-   0        0        0     4566 2022-07-27 13:47:53.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/calculation_diatom_scan.xsl
+-rw-rw-rw-   0        0        0     2817 2022-07-27 13:49:28.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/calculation_diatom_scan_short.xsl
+-rw-rw-rw-   0        0        0     4392 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/diatom_scan.py
+-rw-rw-rw-   0        0        0      174 2019-11-25 20:53:45.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/run0.template
+-rw-rw-rw-   0        0        0     1377 2020-09-22 22:00:40.000000 iprPy-0.11.6/iprPy/calculation/diatom_scan/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.978927 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/
+-rw-rw-rw-   0        0        0    41619 2023-05-31 18:05:48.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/DislocationSDVPN.py
+-rw-rw-rw-   0        0        0     1828 2022-03-10 16:53:15.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/README.md
+-rw-rw-rw-   0        0        0      116 2020-07-31 15:20:42.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/__init__.py
+-rw-rw-rw-   0        0        0      281 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/calculation_dislocation_SDVPN.xsd
+-rw-rw-rw-   0        0        0     8557 2022-03-11 20:18:23.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/dislocation_SDVPN.py
+-rw-rw-rw-   0        0        0      324 2020-09-22 22:03:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.991927 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/
+-rw-rw-rw-   0        0        0      673 2017-12-15 01:46:29.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/README.md
+-rw-rw-rw-   0        0        0     1725 2018-06-27 13:54:23.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/__init__.py
+-rw-rw-rw-   0        0        0     7475 2018-04-09 16:15:16.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calc_dislocation_Peierls_Nabarro_stress.py
+-rw-rw-rw-   0        0        0     1066 2017-12-15 01:43:48.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calc_dislocation_Peierls_Nabarro_stress.template
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.003933 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/
+-rw-rw-rw-   0        0        0     1060 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/README.md
+-rw-rw-rw-   0        0        0      401 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/__init__.py
+-rw-rw-rw-   0        0        0     4832 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/buildmodel.py
+-rw-rw-rw-   0        0        0     1141 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/compare_terms.py
+-rw-rw-rw-   0        0        0      298 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/record-calculation-dislocation-Peierls-Nabarro-stress.xsd
+-rw-rw-rw-   0        0        0      515 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/schema.py
+-rw-rw-rw-   0        0        0     3664 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/todict.py
+-rw-rw-rw-   0        0        0    26459 2017-07-24 22:29:09.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/dislocation_Peierls_Nabarro_stress_template.ipynb
+-rw-rw-rw-   0        0        0     9722 2018-04-11 20:14:48.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/prepare_dislocation_Peierls_Nabarro_stress.py
+-rw-rw-rw-   0        0        0       24 2017-12-14 22:04:14.000000 iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.014927 iprPy-0.11.6/iprPy/calculation/dislocation_monopole/
+-rw-rw-rw-   0        0        0    27648 2023-05-31 18:05:37.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole/DislocationMonopole.py
+-rw-rw-rw-   0        0        0     2534 2022-03-10 16:52:53.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole/README.md
+-rw-rw-rw-   0        0        0      125 2020-07-31 15:19:29.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole/__init__.py
+-rw-rw-rw-   0        0        0      284 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole/calculation_dislocation_monopole.xsd
+-rw-rw-rw-   0        0        0      439 2020-08-27 19:35:19.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole/disl_relax.template
+-rw-rw-rw-   0        0        0    18549 2022-03-08 15:33:29.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole/dislocation_monopole.py
+-rw-rw-rw-   0        0        0     3519 2020-09-22 22:01:26.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.027928 iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/
+-rw-rw-rw-   0        0        0      161 2018-06-27 14:18:08.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/__init__.py
+-rw-rw-rw-   0        0        0     1062 2021-02-26 18:52:18.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/calc_crss.template
+-rw-rw-rw-   0        0        0    18416 2021-03-03 17:27:38.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/calc_dislocation_monopole_crss.py
+-rw-rw-rw-   0        0        0     4133 2016-10-25 14:41:24.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/data_model.py
+-rw-rw-rw-   0        0        0    15473 2016-10-25 14:41:24.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/prepare.py
+-rw-rw-rw-   0        0        0     4089 2016-10-25 14:41:24.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/read_input.py
+-rw-rw-rw-   0        0        0     3199 2021-02-26 18:52:21.000000 iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/strain_system.template
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.039928 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/
+-rw-rw-rw-   0        0        0    28717 2023-05-31 18:05:42.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/DislocationPeriodicArray.py
+-rw-rw-rw-   0        0        0     1284 2022-03-10 16:55:13.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/README.md
+-rw-rw-rw-   0        0        0      140 2020-07-31 15:19:40.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/__init__.py
+-rw-rw-rw-   0        0        0      290 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/calculation_dislocation_periodic_array.xsd
+-rw-rw-rw-   0        0        0      439 2020-08-27 19:35:33.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/disl_relax.template
+-rw-rw-rw-   0        0        0    18993 2022-03-08 15:37:40.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/dislocation_periodic_array.py
+-rw-rw-rw-   0        0        0     3573 2020-09-22 22:02:12.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.053930 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/
+-rw-rw-rw-   0        0        0     2548 2019-07-10 17:30:46.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/DislocationPeriodicArrayStress.py
+-rw-rw-rw-   0        0        0     1603 2019-07-10 17:30:46.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/README.md
+-rw-rw-rw-   0        0        0      279 2019-07-22 15:37:51.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/__init__.py
+-rw-rw-rw-   0        0        0    12411 2019-07-29 16:01:17.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calc_dislocation_periodic_array_stress.py
+-rw-rw-rw-   0        0        0     1337 2019-07-10 17:30:46.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calc_dislocation_periodic_array_stress.template
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.060928 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/
+-rw-rw-rw-   0        0        0     6824 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/CalculationDislocationPeriodicArrayStress.py
+-rw-rw-rw-   0        0        0      818 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/README.md
+-rw-rw-rw-   0        0        0      215 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/__init__.py
+-rw-rw-rw-   0        0        0      297 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/record-calculation-dislocation-periodic-array-stress.xsd
+-rw-rw-rw-   0        0        0     1944 2019-07-10 17:30:46.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/dislarray_free_stress.template
+-rw-rw-rw-   0        0        0     2158 2019-07-10 17:30:46.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/dislarray_rigid_stress.template
+-rw-rw-rw-   0        0        0     3573 2019-07-10 17:30:46.000000 iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.066928 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/
+-rw-rw-rw-   0        0        0      161 2019-07-22 15:38:08.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.108929 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/
+-rw-rw-rw-   0        0        0     3101 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/522c8437-eceb-480d-8f0c-77f83cdb3125.json
+-rw-rw-rw-   0        0        0   795421 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/base.dat
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.114928 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc/
+-rw-rw-rw-   0        0        0      765 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc/110-edge.json
+-rw-rw-rw-   0        0        0      768 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc/111-screw.json
+-rw-rw-rw-   0        0        0      765 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc/112-edge.json
+-rw-rw-rw-   0        0        0     4399 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc.json
+-rw-rw-rw-   0        0        0      963 2016-09-16 16:31:10.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.in
+-rw-rw-rw-   0        0        0     1211 2016-09-16 16:31:10.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.py
+-rw-rw-rw-   0        0        0     1355 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.template
+-rw-rw-rw-   0        0        0      822 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/create_sys.in
+-rw-rw-rw-   0        0        0   795381 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl.dat
+-rw-rw-rw-   0        0        0  1095015 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl.dump
+-rw-rw-rw-   0        0        0      948 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax.in
+-rw-rw-rw-   0        0        0      733 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax.template
+-rw-rw-rw-   0        0        0      477 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax_notemp.template
+-rw-rw-rw-   0        0        0     1913 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax_script.py
+-rw-rw-rw-   0        0        0     4177 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/fcc.json
+-rw-rw-rw-   0        0        0     4725 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/log.lammps
+-rw-rw-rw-   0        0        0     4273 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/results.json
+-rw-rw-rw-   0        0        0     3773 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/data_model.py
+-rw-rw-rw-   0        0        0    11136 2016-06-21 13:43:04.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/prepare.py
+-rw-rw-rw-   0        0        0     3762 2016-09-16 16:31:10.000000 iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/read_input.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.123928 iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/
+-rw-rw-rw-   0        0        0      629 2018-06-27 14:18:20.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/__init__.py
+-rw-rw-rw-   0        0        0     1365 2017-03-16 13:24:41.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.in
+-rw-rw-rw-   0        0        0    29440 2022-10-04 13:35:04.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.py
+-rw-rw-rw-   0        0        0     1416 2017-02-17 17:13:16.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.template
+-rw-rw-rw-   0        0        0      591 2017-02-13 20:46:19.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/full_relax.template
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.136927 iprPy-0.11.6/iprPy/calculation/elastic_constants_static/
+-rw-rw-rw-   0        0        0    17517 2023-05-31 18:06:01.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_static/ElasticConstantsStatic.py
+-rw-rw-rw-   0        0        0     1884 2022-03-10 16:52:22.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_static/README.md
+-rw-rw-rw-   0        0        0      134 2020-07-31 15:20:28.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_static/__init__.py
+-rw-rw-rw-   0        0        0      288 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_static/calculation_elastic_constants_static.xsd
+-rw-rw-rw-   0        0        0     3343 2021-01-29 17:33:30.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_static/cij.template
+-rw-rw-rw-   0        0        0     8251 2022-03-07 20:09:20.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_static/elastic_constants_static.py
+-rw-rw-rw-   0        0        0     1363 2020-09-22 22:04:58.000000 iprPy-0.11.6/iprPy/calculation/elastic_constants_static/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.146927 iprPy-0.11.6/iprPy/calculation/energy_check/
+-rw-rw-rw-   0        0        0     9554 2023-05-31 18:06:08.000000 iprPy-0.11.6/iprPy/calculation/energy_check/EnergyCheck.py
+-rw-rw-rw-   0        0        0      636 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/energy_check/README.md
+-rw-rw-rw-   0        0        0       99 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/energy_check/__init__.py
+-rw-rw-rw-   0        0        0      276 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/energy_check/calculation_energy_check.xsd
+-rw-rw-rw-   0        0        0     2160 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/energy_check/energy_check.py
+-rw-rw-rw-   0        0        0      269 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/energy_check/run0.template
+-rw-rw-rw-   0        0        0      230 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/calculation/energy_check/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.161928 iprPy-0.11.6/iprPy/calculation/free_energy/
+-rw-rw-rw-   0        0        0    28127 2023-05-31 18:06:16.000000 iprPy-0.11.6/iprPy/calculation/free_energy/FreeEnergy.py
+-rw-rw-rw-   0        0        0      804 2022-09-20 17:22:25.000000 iprPy-0.11.6/iprPy/calculation/free_energy/README.md
+-rw-rw-rw-   0        0        0       77 2022-09-20 17:05:23.000000 iprPy-0.11.6/iprPy/calculation/free_energy/__init__.py
+-rw-rw-rw-   0        0        0      275 2022-09-20 17:22:26.000000 iprPy-0.11.6/iprPy/calculation/free_energy/calculation_free_energy.xsd
+-rw-rw-rw-   0        0        0    16471 2022-09-20 17:22:39.000000 iprPy-0.11.6/iprPy/calculation/free_energy/free_energy.py
+-rw-rw-rw-   0        0        0     1053 2022-09-20 15:32:26.000000 iprPy-0.11.6/iprPy/calculation/free_energy/free_energy.template
+-rw-rw-rw-   0        0        0      609 2022-09-19 15:15:23.000000 iprPy-0.11.6/iprPy/calculation/free_energy/msd.template
+-rw-rw-rw-   0        0        0      766 2022-09-20 17:22:13.000000 iprPy-0.11.6/iprPy/calculation/free_energy/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.176927 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/
+-rw-rw-rw-   0        0        0    25960 2023-05-31 18:06:28.000000 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/FreeEnergyLiquid.py
+-rw-rw-rw-   0        0        0      962 2022-10-18 17:47:07.000000 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/README.md
+-rw-rw-rw-   0        0        0    76625 2022-10-26 16:32:59.000000 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/UhlenbeckFordModel.py
+-rw-rw-rw-   0        0        0       95 2022-10-18 17:43:55.000000 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/__init__.py
+-rw-rw-rw-   0        0        0      282 2022-10-18 17:42:30.000000 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/calculation_free_energy_liquid.xsd
+-rw-rw-rw-   0        0        0    11975 2022-10-19 18:31:36.000000 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/free_energy_liquid.py
+-rw-rw-rw-   0        0        0     1186 2022-10-19 16:40:06.000000 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/free_energy_liquid.template
+-rw-rw-rw-   0        0        0      766 2022-09-20 17:22:13.000000 iprPy-0.11.6/iprPy/calculation/free_energy_liquid/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.182927 iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/
+-rw-rw-rw-   0        0        0      638 2018-06-27 14:18:00.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/__init__.py
+-rw-rw-rw-   0        0        0    11732 2017-03-13 18:10:32.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/calc_bcc_grain_boundary.py
+-rw-rw-rw-   0        0        0     1252 2016-12-30 23:01:13.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/calc_bcc_grain_boundary.template
+-rw-rw-rw-   0        0        0     2059 2016-12-30 22:37:08.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/grain_boundary.template
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.191928 iprPy-0.11.6/iprPy/calculation/grain_boundary_search/
+-rw-rw-rw-   0        0        0     1020 2017-05-01 19:00:38.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_search/README.md
+-rw-rw-rw-   0        0        0       97 2018-06-27 14:18:33.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_search/__init__.py
+-rw-rw-rw-   0        0        0      525 2017-07-06 18:31:53.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_search/compare_terms.py
+-rw-rw-rw-   0        0        0      285 2016-12-31 00:03:23.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_search/record-calculation-grain-boundary-search.xsd
+-rw-rw-rw-   0        0        0      158 2017-05-03 19:21:57.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_search/schema.py
+-rw-rw-rw-   0        0        0     1469 2017-05-03 19:22:32.000000 iprPy-0.11.6/iprPy/calculation/grain_boundary_search/todict.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.207928 iprPy-0.11.6/iprPy/calculation/isolated_atom/
+-rw-rw-rw-   0        0        0    11942 2023-05-31 18:06:34.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/IsolatedAtom.py
+-rw-rw-rw-   0        0        0     1059 2022-03-10 16:52:15.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/README.md
+-rw-rw-rw-   0        0        0      127 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/__init__.py
+-rw-rw-rw-   0        0        0      277 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/calculation_isolated_atom.xsd
+-rw-rw-rw-   0        0        0     2405 2022-07-26 20:19:39.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/calculation_isolated_atom.xsl
+-rw-rw-rw-   0        0        0      469 2022-07-19 16:35:37.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/calculation_isolated_atom_short.xsl
+-rw-rw-rw-   0        0        0     2725 2022-03-07 20:08:50.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/isolated_atom.py
+-rw-rw-rw-   0        0        0      174 2020-07-29 18:48:37.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/run0.template
+-rw-rw-rw-   0        0        0      955 2020-09-22 22:05:46.000000 iprPy-0.11.6/iprPy/calculation/isolated_atom/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.217928 iprPy-0.11.6/iprPy/calculation/phonon/
+-rw-rw-rw-   0        0        0    30497 2023-05-31 18:06:39.000000 iprPy-0.11.6/iprPy/calculation/phonon/Phonon.py
+-rw-rw-rw-   0        0        0      794 2022-03-10 16:52:05.000000 iprPy-0.11.6/iprPy/calculation/phonon/README.md
+-rw-rw-rw-   0        0        0       86 2020-07-31 15:21:30.000000 iprPy-0.11.6/iprPy/calculation/phonon/__init__.py
+-rw-rw-rw-   0        0        0    16969 2023-04-18 20:04:30.000000 iprPy-0.11.6/iprPy/calculation/phonon/calc_phonon.py
+-rw-rw-rw-   0        0        0      270 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/phonon/calculation_phonon.xsd
+-rw-rw-rw-   0        0        0      298 2020-12-21 15:35:11.000000 iprPy-0.11.6/iprPy/calculation/phonon/phonon.template
+-rw-rw-rw-   0        0        0      780 2019-07-26 17:47:07.000000 iprPy-0.11.6/iprPy/calculation/phonon/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.230927 iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/
+-rw-rw-rw-   0        0        0    30411 2023-04-11 18:50:11.000000 iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/PointDefectDiffusion.py
+-rw-rw-rw-   0        0        0     1213 2022-03-10 16:53:46.000000 iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/README.md
+-rw-rw-rw-   0        0        0      128 2020-07-31 15:21:39.000000 iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/__init__.py
+-rw-rw-rw-   0        0        0      286 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/calculation_point_defect_diffusion.xsd
+-rw-rw-rw-   0        0        0     1144 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/diffusion.template
+-rw-rw-rw-   0        0        0     9991 2022-03-07 20:41:33.000000 iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/point_defect_diffusion.py
+-rw-rw-rw-   0        0        0     1462 2019-07-26 17:49:39.000000 iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.242928 iprPy-0.11.6/iprPy/calculation/point_defect_static/
+-rw-rw-rw-   0        0        0    25262 2023-05-31 18:06:45.000000 iprPy-0.11.6/iprPy/calculation/point_defect_static/PointDefectStatic.py
+-rw-rw-rw-   0        0        0     2080 2022-03-10 16:51:46.000000 iprPy-0.11.6/iprPy/calculation/point_defect_static/README.md
+-rw-rw-rw-   0        0        0      119 2020-07-31 15:22:45.000000 iprPy-0.11.6/iprPy/calculation/point_defect_static/__init__.py
+-rw-rw-rw-   0        0        0      283 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/point_defect_static/calculation_point_defect_static.xsd
+-rw-rw-rw-   0        0        0      427 2021-01-07 21:36:18.000000 iprPy-0.11.6/iprPy/calculation/point_defect_static/min.template
+-rw-rw-rw-   0        0        0    18254 2022-03-10 20:44:04.000000 iprPy-0.11.6/iprPy/calculation/point_defect_static/point_defect_static.py
+-rw-rw-rw-   0        0        0     3954 2019-07-26 19:10:33.000000 iprPy-0.11.6/iprPy/calculation/point_defect_static/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.253931 iprPy-0.11.6/iprPy/calculation/relax_box/
+-rw-rw-rw-   0        0        0     1485 2022-03-10 16:51:20.000000 iprPy-0.11.6/iprPy/calculation/relax_box/README.md
+-rw-rw-rw-   0        0        0    31236 2023-05-31 18:06:52.000000 iprPy-0.11.6/iprPy/calculation/relax_box/RelaxBox.py
+-rw-rw-rw-   0        0        0       92 2020-07-31 15:22:51.000000 iprPy-0.11.6/iprPy/calculation/relax_box/__init__.py
+-rw-rw-rw-   0        0        0      273 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/relax_box/calculation_relax_box.xsd
+-rw-rw-rw-   0        0        0     4352 2021-10-20 21:24:11.000000 iprPy-0.11.6/iprPy/calculation/relax_box/cij_run0.template
+-rw-rw-rw-   0        0        0    17154 2022-03-07 17:38:17.000000 iprPy-0.11.6/iprPy/calculation/relax_box/relax_box.py
+-rw-rw-rw-   0        0        0     1570 2020-09-22 22:06:42.000000 iprPy-0.11.6/iprPy/calculation/relax_box/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.268931 iprPy-0.11.6/iprPy/calculation/relax_dynamic/
+-rw-rw-rw-   0        0        0     2295 2022-03-10 16:50:31.000000 iprPy-0.11.6/iprPy/calculation/relax_dynamic/README.md
+-rw-rw-rw-   0        0        0    53379 2023-05-31 18:07:01.000000 iprPy-0.11.6/iprPy/calculation/relax_dynamic/RelaxDynamic.py
+-rw-rw-rw-   0        0        0      104 2020-07-31 15:22:56.000000 iprPy-0.11.6/iprPy/calculation/relax_dynamic/__init__.py
+-rw-rw-rw-   0        0        0      277 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/relax_dynamic/calculation_relax_dynamic.xsd
+-rw-rw-rw-   0        0        0      577 2022-03-08 18:15:11.000000 iprPy-0.11.6/iprPy/calculation/relax_dynamic/full_relax.template
+-rw-rw-rw-   0        0        0      570 2022-03-08 18:32:01.000000 iprPy-0.11.6/iprPy/calculation/relax_dynamic/full_relax_restart.template
+-rw-rw-rw-   0        0        0    20476 2023-05-31 17:52:21.000000 iprPy-0.11.6/iprPy/calculation/relax_dynamic/relax_dynamic.py
+-rw-rw-rw-   0        0        0     2051 2020-09-22 22:07:08.000000 iprPy-0.11.6/iprPy/calculation/relax_dynamic/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.287929 iprPy-0.11.6/iprPy/calculation/relax_liquid/
+-rw-rw-rw-   0        0        0     1423 2023-07-31 20:44:54.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/README.md
+-rw-rw-rw-   0        0        0    46835 2023-05-31 18:07:07.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/RelaxLiquid.py
+-rw-rw-rw-   0        0        0      101 2022-10-11 12:17:29.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/__init__.py
+-rw-rw-rw-   0        0        0      276 2022-10-11 19:15:07.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/calculation_relax_liquid.xsd
+-rw-rw-rw-   0        0        0     3133 2023-05-15 18:08:33.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/liquid_ave_pe.template
+-rw-rw-rw-   0        0        0     3078 2023-05-15 18:08:31.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/liquid_ave_te.template
+-rw-rw-rw-   0        0        0      962 2023-05-15 18:08:36.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/liquid_restart.template
+-rw-rw-rw-   0        0        0    16671 2023-07-31 20:59:12.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/relax_liquid.py
+-rw-rw-rw-   0        0        0     5838 2022-10-15 13:24:08.000000 iprPy-0.11.6/iprPy/calculation/relax_liquid/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.298928 iprPy-0.11.6/iprPy/calculation/relax_static/
+-rw-rw-rw-   0        0        0     1137 2022-03-10 16:50:26.000000 iprPy-0.11.6/iprPy/calculation/relax_static/README.md
+-rw-rw-rw-   0        0        0    35298 2023-05-31 18:07:15.000000 iprPy-0.11.6/iprPy/calculation/relax_static/RelaxStatic.py
+-rw-rw-rw-   0        0        0      101 2020-07-31 15:23:02.000000 iprPy-0.11.6/iprPy/calculation/relax_static/__init__.py
+-rw-rw-rw-   0        0        0      276 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/relax_static/calculation_relax_static.xsd
+-rw-rw-rw-   0        0        0      552 2020-07-29 18:48:37.000000 iprPy-0.11.6/iprPy/calculation/relax_static/minbox.template
+-rw-rw-rw-   0        0        0    11585 2022-03-07 17:03:22.000000 iprPy-0.11.6/iprPy/calculation/relax_static/relax_static.py
+-rw-rw-rw-   0        0        0      555 2020-09-22 22:07:34.000000 iprPy-0.11.6/iprPy/calculation/relax_static/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.310928 iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/
+-rw-rw-rw-   0        0        0     1128 2022-03-10 16:54:23.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/README.md
+-rw-rw-rw-   0        0        0    21813 2023-05-31 18:07:21.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/StackingFaultMap2D.py
+-rw-rw-rw-   0        0        0      122 2020-07-31 15:23:08.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/__init__.py
+-rw-rw-rw-   0        0        0      285 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/calculation_stacking_fault_map_2D.xsd
+-rw-rw-rw-   0        0        0      482 2020-08-18 13:49:57.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/sfmin.template
+-rw-rw-rw-   0        0        0    15829 2022-03-07 20:57:51.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/stacking_fault_map_2D.py
+-rw-rw-rw-   0        0        0     3050 2020-09-22 22:08:55.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.330927 iprPy-0.11.6/iprPy/calculation/stacking_fault_static/
+-rw-rw-rw-   0        0        0     1013 2022-03-10 16:54:46.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_static/README.md
+-rw-rw-rw-   0        0        0    19071 2023-05-31 18:07:27.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_static/StackingFaultStatic.py
+-rw-rw-rw-   0        0        0      125 2020-07-31 15:23:15.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_static/__init__.py
+-rw-rw-rw-   0        0        0      285 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_static/calculation_stacking_fault_static.xsd
+-rw-rw-rw-   0        0        0      482 2020-08-18 13:49:56.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_static/sfmin.template
+-rw-rw-rw-   0        0        0    17048 2022-03-07 20:57:52.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_static/stacking_fault_static.py
+-rw-rw-rw-   0        0        0     2829 2020-09-22 22:09:25.000000 iprPy-0.11.6/iprPy/calculation/stacking_fault_static/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.342927 iprPy-0.11.6/iprPy/calculation/surface_energy_static/
+-rw-rw-rw-   0        0        0     1159 2022-03-10 16:54:57.000000 iprPy-0.11.6/iprPy/calculation/surface_energy_static/README.md
+-rw-rw-rw-   0        0        0    17733 2023-05-31 18:07:34.000000 iprPy-0.11.6/iprPy/calculation/surface_energy_static/SurfaceEnergyStatic.py
+-rw-rw-rw-   0        0        0      125 2020-07-31 15:23:22.000000 iprPy-0.11.6/iprPy/calculation/surface_energy_static/__init__.py
+-rw-rw-rw-   0        0        0      285 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/calculation/surface_energy_static/calculation_surface_energy_static.xsd
+-rw-rw-rw-   0        0        0      408 2020-08-18 13:49:53.000000 iprPy-0.11.6/iprPy/calculation/surface_energy_static/min.template
+-rw-rw-rw-   0        0        0    12968 2022-03-10 20:44:03.000000 iprPy-0.11.6/iprPy/calculation/surface_energy_static/surface_energy_static.py
+-rw-rw-rw-   0        0        0     1844 2020-09-22 22:10:07.000000 iprPy-0.11.6/iprPy/calculation/surface_energy_static/theory.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.365929 iprPy-0.11.6/iprPy/calculation_subset/
+-rw-rw-rw-   0        0        0    14400 2023-04-10 17:16:00.000000 iprPy-0.11.6/iprPy/calculation_subset/AtommanElasticConstants.py
+-rw-rw-rw-   0        0        0     8647 2023-04-10 17:16:10.000000 iprPy-0.11.6/iprPy/calculation_subset/AtommanGammaSurface.py
+-rw-rw-rw-   0        0        0    26242 2023-04-10 17:16:23.000000 iprPy-0.11.6/iprPy/calculation_subset/AtommanSystemLoad.py
+-rw-rw-rw-   0        0        0    21641 2023-04-10 17:16:40.000000 iprPy-0.11.6/iprPy/calculation_subset/AtommanSystemManipulate.py
+-rw-rw-rw-   0        0        0     8322 2023-04-08 17:04:04.000000 iprPy-0.11.6/iprPy/calculation_subset/CalculationSubset.py
+-rw-rw-rw-   0        0        0    35750 2023-04-10 17:17:51.000000 iprPy-0.11.6/iprPy/calculation_subset/Dislocation.py
+-rw-rw-rw-   0        0        0    23748 2023-04-10 17:17:32.000000 iprPy-0.11.6/iprPy/calculation_subset/FreeSurface.py
+-rw-rw-rw-   0        0        0     9644 2023-04-10 17:16:46.000000 iprPy-0.11.6/iprPy/calculation_subset/LammpsCommands.py
+-rw-rw-rw-   0        0        0    14048 2023-04-10 17:16:53.000000 iprPy-0.11.6/iprPy/calculation_subset/LammpsMinimize.py
+-rw-rw-rw-   0        0        0    15229 2023-04-10 17:17:13.000000 iprPy-0.11.6/iprPy/calculation_subset/LammpsPotential.py
+-rw-rw-rw-   0        0        0    21964 2023-04-10 17:19:16.000000 iprPy-0.11.6/iprPy/calculation_subset/PointDefect.py
+-rw-rw-rw-   0        0        0    28989 2023-04-10 17:18:02.000000 iprPy-0.11.6/iprPy/calculation_subset/StackingFault.py
+-rw-rw-rw-   0        0        0     7119 2023-04-10 17:02:30.000000 iprPy-0.11.6/iprPy/calculation_subset/Units.py
+-rw-rw-rw-   0        0        0      617 2023-04-07 16:02:15.000000 iprPy-0.11.6/iprPy/calculation_subset/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-07 15:12:34.000000 iprPy-0.11.6/iprPy/check_modules.py
+-rw-rw-rw-   0        0        0    21501 2023-07-27 20:21:53.000000 iprPy-0.11.6/iprPy/command_line.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.380928 iprPy-0.11.6/iprPy/database/
+-rw-rw-rw-   0        0        0      235 2022-05-23 16:10:37.000000 iprPy-0.11.6/iprPy/database/CDCSDatabase.py
+-rw-rw-rw-   0        0        0    26668 2022-05-23 16:10:37.000000 iprPy-0.11.6/iprPy/database/IprPyDatabase.py
+-rw-rw-rw-   0        0        0      238 2022-05-23 16:10:37.000000 iprPy-0.11.6/iprPy/database/LocalDatabase.py
+-rw-rw-rw-   0        0        0     1642 2022-05-23 16:10:37.000000 iprPy-0.11.6/iprPy/database/MongoDatabase.py
+-rw-rw-rw-   0        0        0     1892 2022-05-23 16:10:37.000000 iprPy-0.11.6/iprPy/database/__init__.py
+-rw-rw-rw-   0        0        0     1061 2023-07-27 20:25:54.000000 iprPy-0.11.6/iprPy/database/load_database.py
+-rw-rw-rw-   0        0        0     5800 2022-04-07 17:25:44.000000 iprPy-0.11.6/iprPy/database/master_prepare.py
+-rw-rw-rw-   0        0        0    16414 2022-10-20 11:33:59.000000 iprPy-0.11.6/iprPy/database/prepare.py
+-rw-rw-rw-   0        0        0     1817 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/database/reset_orphans.py
+-rw-rw-rw-   0        0        0    24405 2022-02-15 16:01:52.000000 iprPy-0.11.6/iprPy/database/runner.py
+-rw-rw-rw-   0        0        0     4432 2023-04-24 19:37:40.000000 iprPy-0.11.6/iprPy/fix_lammps_versions.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.388927 iprPy-0.11.6/iprPy/input/
+-rw-rw-rw-   0        0        0      391 2022-03-03 22:02:42.000000 iprPy-0.11.6/iprPy/input/__init__.py
+-rw-rw-rw-   0        0        0      980 2022-03-03 22:15:35.000000 iprPy-0.11.6/iprPy/input/boolean.py
+-rw-rw-rw-   0        0        0     1220 2022-03-03 22:05:53.000000 iprPy-0.11.6/iprPy/input/buildcombos.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.401928 iprPy-0.11.6/iprPy/input/buildcombos_functions/
+-rw-rw-rw-   0        0        0     5918 2019-07-24 15:27:46.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/README.rst
+-rw-rw-rw-   0        0        0      471 2022-03-03 22:19:43.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/__init__.py
+-rw-rw-rw-   0        0        0     6741 2022-03-03 22:42:59.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/atomicarchive.py
+-rw-rw-rw-   0        0        0     7120 2022-03-03 22:40:49.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/atomicparent.py
+-rw-rw-rw-   0        0        0     7354 2022-03-03 22:42:55.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/atomicreference.py
+-rw-rw-rw-   0        0        0     6477 2022-03-03 22:41:53.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/crystalprototype.py
+-rw-rw-rw-   0        0        0     3097 2022-03-03 22:38:23.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/defect.py
+-rw-rw-rw-   0        0        0     3450 2022-03-03 22:38:35.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/diatom.py
+-rw-rw-rw-   0        0        0     3057 2022-03-03 22:38:30.000000 iprPy-0.11.6/iprPy/input/buildcombos_functions/lammpspotential.py
+-rw-rw-rw-   0        0        0     4050 2022-03-03 22:15:33.000000 iprPy-0.11.6/iprPy/input/parse.py
+-rw-rw-rw-   0        0        0     2015 2022-03-03 22:18:09.000000 iprPy-0.11.6/iprPy/input/termtodict.py
+-rw-rw-rw-   0        0        0     1698 2022-03-03 22:19:18.000000 iprPy-0.11.6/iprPy/input/value.py
+-rw-rw-rw-   0        0        0     1335 2023-04-07 15:07:09.000000 iprPy-0.11.6/iprPy/load_run_directory.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.404928 iprPy-0.11.6/iprPy/record/
+-rw-rw-rw-   0        0        0    12959 2023-05-31 18:04:25.000000 iprPy-0.11.6/iprPy/record/PotentialProperties.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.417928 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/
+-rw-rw-rw-   0        0        0     5535 2022-06-01 13:45:46.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/CrystalStructure.py
+-rw-rw-rw-   0        0        0     1305 2022-02-15 16:01:52.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/DiatomScan.py
+-rw-rw-rw-   0        0        0     5317 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/ElasticConstants.py
+-rw-rw-rw-   0        0        0     1805 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/EvsRScan.py
+-rw-rw-rw-   0        0        0     3847 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/FreeSurface.py
+-rw-rw-rw-   0        0        0     6255 2023-04-11 18:57:57.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/Phonon.py
+-rw-rw-rw-   0        0        0     4598 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/PointDefect.py
+-rw-rw-rw-   0        0        0     1025 2023-03-07 17:45:11.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/PotentialsPropertiesSubset.py
+-rw-rw-rw-   0        0        0     6241 2022-07-11 18:42:14.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/StackingFault.py
+-rw-rw-rw-   0        0        0      308 2022-11-18 21:23:15.000000 iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/__init__.py
+-rw-rw-rw-   0        0        0      322 2023-04-07 15:52:13.000000 iprPy-0.11.6/iprPy/record/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.420928 iprPy-0.11.6/iprPy/record/xsd/
+-rw-rw-rw-   0        0        0        0 2021-09-14 18:07:39.000000 iprPy-0.11.6/iprPy/record/xsd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:13.426928 iprPy-0.11.6/iprPy/tools/
+-rw-rw-rw-   0        0        0      574 2022-11-18 20:44:52.000000 iprPy-0.11.6/iprPy/tools/__init__.py
+-rw-rw-rw-   0        0        0     1910 2023-04-07 15:21:37.000000 iprPy-0.11.6/iprPy/tools/dict_insert.py
+-rw-rw-rw-   0        0        0     1934 2022-03-03 21:50:13.000000 iprPy-0.11.6/iprPy/tools/dynamic_import.py
+-rw-rw-rw-   0        0        0     1679 2023-04-07 15:22:17.000000 iprPy-0.11.6/iprPy/tools/num_deriv_3_point.py
+-rw-rw-rw-   0        0        0      746 2023-04-07 15:23:02.000000 iprPy-0.11.6/iprPy/tools/read_calc_file.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:07:12.857929 iprPy-0.11.6/iprPy.egg-info/
+-rw-rw-rw-   0        0        0     2533 2023-07-31 21:07:12.000000 iprPy-0.11.6/iprPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18818 2023-07-31 21:07:12.000000 iprPy-0.11.6/iprPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 21:07:12.000000 iprPy-0.11.6/iprPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-31 21:07:12.000000 iprPy-0.11.6/iprPy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2019-07-10 18:55:45.000000 iprPy-0.11.6/iprPy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-07-31 21:07:12.000000 iprPy-0.11.6/iprPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 21:07:12.000000 iprPy-0.11.6/iprPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-02-03 20:26:52.000000 iprPy-0.11.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 21:07:13.429928 iprPy-0.11.6/setup.cfg
+-rw-rw-rw-   0        0        0     1799 2023-07-27 20:21:23.000000 iprPy-0.11.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `iprPy-0.11.5/LICENSE.TXT` & `iprPy-0.11.6/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/PKG-INFO` & `iprPy-0.11.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: iprPy
-Version: 0.11.5
+Version: 0.11.6
 Summary: Interatomic Potential Repository Python Property Calculations and Tools
 Home-page: https://github.com/usnistgov/iprPy
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: atom,atomic,atomistic,molecular dynamics,high-throughput,interatomic potential
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.TXT
```

### Comparing `iprPy-0.11.5/README.rst` & `iprPy-0.11.6/README.rst`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/README.rst` & `iprPy-0.11.6/bin/README.rst`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/check_runners.py` & `iprPy-0.11.6/bin/check_runners.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare/master_prepare_ctcms.in` & `iprPy-0.11.6/bin/prepare/master_prepare_ctcms.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_1.in` & `iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_1.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_2.in` & `iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_2.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_3.in` & `iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_3.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_4.in` & `iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_4.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare/master_prepare_ctcms_pool_5.in` & `iprPy-0.11.6/bin/prepare/master_prepare_ctcms_pool_5.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare/master_prepare_desktop.in` & `iprPy-0.11.6/bin/prepare/master_prepare_desktop.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare/master_prepare_desktop_wsl.in` & `iprPy-0.11.6/bin/prepare/master_prepare_desktop_wsl.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/bin/prepare_relax_dynamic_at_temp.py` & `iprPy-0.11.6/bin/prepare_relax_dynamic_at_temp.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/Settings.py` & `iprPy-0.11.6/iprPy/Settings.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/__init__.py` & `iprPy-0.11.6/iprPy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # coding: utf-8
 
 # Standard Python libraries
 from importlib import resources
 
 # Read version from VERSION file
-__version__ = resources.read_text('iprPy', 'VERSION').strip()
+if hasattr(resources, 'files'):
+    __version__ = resources.files('iprPy').joinpath('VERSION').read_text(encoding='UTF-8')
+else:
+    __version__ = resources.read_text('iprPy', 'VERSION', encoding='UTF-8').strip()
 
 # iprPy imports
 from . import tools
 from .Settings import settings
 from .load_run_directory import load_run_directory
 from .fix_lammps_versions import fix_lammps_versions
 from . import input
@@ -26,12 +29,12 @@
 from .command_line import command_line
 
 from . import analysis
 
 __all__ = ['__version__', 'tools', 'settings', 'input',
            'load_run_directory', 'fix_lammps_versions',
            'record', 'load_record', 'recordmanager',
-           'calculation_subset',
+           'calculation_subset', 'analysis',
            'calculation', 'load_calculation', 'calculationmanager',
            'database', 'load_database', 'databasemanager',
            'check_modules', 'command_line', 'reset_orphans']
 __all__.sort()
```

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/__init__.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/__init__.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_crystal.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_crystal.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_diatom.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_diatom.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_elastic.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_elastic.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_empty.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_empty.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_evsr.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_evsr.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_phonon.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_phonon.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_point.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_point.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_stacking.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_stacking.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/PropertyProcessor/_surface.py` & `iprPy-0.11.6/iprPy/analysis/PropertyProcessor/_surface.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/get_isolated_atom_energies.py` & `iprPy-0.11.6/iprPy/analysis/get_isolated_atom_energies.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/match_reference_prototype.py` & `iprPy-0.11.6/iprPy/analysis/match_reference_prototype.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/process_relaxations.py` & `iprPy-0.11.6/iprPy/analysis/process_relaxations.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/thermo/AnalyzeFE.py` & `iprPy-0.11.6/iprPy/analysis/thermo/AnalyzeFE.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/thermo/AnalyzeMD.py` & `iprPy-0.11.6/iprPy/analysis/thermo/AnalyzeMD.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/analysis/thermo/AnalyzeQHA.py` & `iprPy-0.11.6/iprPy/analysis/thermo/AnalyzeQHA.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/Calculation.py` & `iprPy-0.11.6/iprPy/calculation/Calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,19 @@
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         database : atomman.library.Database or Database, optional
             A Database object to associate with the calculation record.  Some
             calculation styles may have options where additional data can be
             accessed from other records in a database.  Specifying a database
@@ -86,15 +91,15 @@
         # Initialize subsets list
         if subsets is not None:
             self.__subsets = tuple(subsets)
         else:
             self.__subsets = ()
 
         # Call Record's init
-        super().__init__(model=model, name=name, **kwargs)
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
         # Load parameters if given
         if params is not None:
             self.load_parameters(params, key=kwargs.get('key', None))
 
     @property
     def maindoc(self) -> str:
```

### Comparing `iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/EvsRScan.py` & `iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/EvsRScan.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,33 @@
     """Class for managing energy versus r volumetric scans for crystals"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -72,15 +78,15 @@
         self.energy_values = None
         self.min_cells = None
 
         # Define calc shortcut
         self.calc = e_vs_r_scan
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'e_vs_r_scan.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/README.md` & `iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan.xsl` & `iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan.xsl`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan_short.xsl` & `iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/calculation_E_vs_r_scan_short.xsl`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/e_vs_r_scan.py` & `iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/e_vs_r_scan.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/E_vs_r_scan/theory.md` & `iprPy-0.11.6/iprPy/calculation/E_vs_r_scan/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/__init__.py` & `iprPy-0.11.6/iprPy/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bain_transformation_map/Bain.ipynb` & `iprPy-0.11.6/iprPy/calculation/bain_transformation_map/Bain.ipynb`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bain_transformation_map/Bain.py` & `iprPy-0.11.6/iprPy/calculation/bain_transformation_map/Bain.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bain_transformation_map/BainTransformationMap.py` & `iprPy-0.11.6/iprPy/calculation/bain_transformation_map/BainTransformationMap.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calc_bain_transformation_map.py` & `iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calc_bain_transformation_map.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/CalculationBainTransformationMap.py` & `iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/CalculationBainTransformationMap.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/README.md` & `iprPy-0.11.6/iprPy/calculation/bain_transformation_map/calculation_bain_transformation_map/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bain_transformation_map/data_model.py` & `iprPy-0.11.6/iprPy/calculation/bain_transformation_map/data_model.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bond_angle_scan/BondAngleScan.py` & `iprPy-0.11.6/iprPy/calculation/bond_angle_scan/BondAngleScan.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,27 +25,33 @@
     """Class for managing 3-body (bond angle) energy scan calculations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -69,15 +75,15 @@
         self.results_length_unit = None
         self.results_energy_unit = None
 
         # Define calc shortcut
         self.calc = bond_angle_scan
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'bond_angle_scan.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/bond_angle_scan/README.md` & `iprPy-0.11.6/iprPy/calculation/bond_angle_scan/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bond_angle_scan/bond_angle_scan.py` & `iprPy-0.11.6/iprPy/calculation/bond_angle_scan/bond_angle_scan.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bond_angle_scan/bond_scan.template` & `iprPy-0.11.6/iprPy/calculation/bond_angle_scan/bond_scan.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bond_angle_scan/prepare_bond_angle_scan.py` & `iprPy-0.11.6/iprPy/calculation/bond_angle_scan/prepare_bond_angle_scan.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/bond_angle_scan/theory.md` & `iprPy-0.11.6/iprPy/calculation/bond_angle_scan/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/crystal_space_group/CrystalSpaceGroup.py` & `iprPy-0.11.6/iprPy/calculation/crystal_space_group/CrystalSpaceGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,33 @@
     """Class for managing space group analysis of crystals"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -67,15 +73,15 @@
         self.__wyckoff_fingerprint = None
         self.__spg_ucell = None
 
         # Define calc shortcut
         self.calc = crystal_space_group
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'crystal_space_group.py'
```

### Comparing `iprPy-0.11.5/iprPy/calculation/crystal_space_group/README.md` & `iprPy-0.11.6/iprPy/calculation/crystal_space_group/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/crystal_space_group/crystal_space_group.py` & `iprPy-0.11.6/iprPy/calculation/crystal_space_group/crystal_space_group.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/diatom_scan/DiatomScan.py` & `iprPy-0.11.6/iprPy/calculation/diatom_scan/DiatomScan.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,33 @@
     """Class for managing diatom energy scan calculations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -65,15 +71,15 @@
         self.r_values = None
         self.energy_values = None
 
         # Define calc shortcut
         self.calc = diatom_scan
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'diatom_scan.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/diatom_scan/README.md` & `iprPy-0.11.6/iprPy/calculation/diatom_scan/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/diatom_scan/calculation_diatom_scan.xsl` & `iprPy-0.11.6/iprPy/calculation/diatom_scan/calculation_diatom_scan.xsl`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/diatom_scan/calculation_diatom_scan_short.xsl` & `iprPy-0.11.6/iprPy/calculation/diatom_scan/calculation_diatom_scan_short.xsl`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/diatom_scan/diatom_scan.py` & `iprPy-0.11.6/iprPy/calculation/diatom_scan/diatom_scan.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/diatom_scan/theory.md` & `iprPy-0.11.6/iprPy/calculation/diatom_scan/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/DislocationSDVPN.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/DislocationSDVPN.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,33 @@
     """Class for managing semi-discrete variational Peierls-Nabarro calcuations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -83,15 +89,15 @@
         self.__energies = None
         self.__disregistries = None
 
         # Define calc shortcut
         self.calc = sdvpn
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'dislocation_SDVPN.py'
```

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/README.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN/dislocation_SDVPN.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN/dislocation_SDVPN.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/README.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/__init__.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/__init__.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calc_dislocation_Peierls_Nabarro_stress.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calc_dislocation_Peierls_Nabarro_stress.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calc_dislocation_Peierls_Nabarro_stress.template` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calc_dislocation_Peierls_Nabarro_stress.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/README.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/buildmodel.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/buildmodel.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/compare_terms.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/compare_terms.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/schema.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/schema.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/todict.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/calculation_dislocation_SDVPN_stress/todict.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/dislocation_Peierls_Nabarro_stress_template.ipynb` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/dislocation_Peierls_Nabarro_stress_template.ipynb`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_SDVPN_stress/prepare_dislocation_Peierls_Nabarro_stress.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_SDVPN_stress/prepare_dislocation_Peierls_Nabarro_stress.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole/DislocationMonopole.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole/DislocationMonopole.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,33 @@
     """Class for managing dislocation monopole constructions and relaxation"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -78,15 +84,15 @@
         self.__preln = None
         self.__K_tensor = None
 
         # Define calc shortcut
         self.calc = dislocation_monopole
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'dislocation_monopole.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole/README.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole/dislocation_monopole.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole/dislocation_monopole.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole/theory.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/calc_crss.template` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/calc_crss.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/calc_dislocation_monopole_crss.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/calc_dislocation_monopole_crss.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/data_model.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/data_model.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/prepare.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/prepare.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/read_input.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/read_input.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_monopole_crss/strain_system.template` & `iprPy-0.11.6/iprPy/calculation/dislocation_monopole_crss/strain_system.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/DislocationPeriodicArray.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/DislocationPeriodicArray.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,33 @@
     """Class for managing periodic array of dislocations constructions and relaxations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -79,15 +85,15 @@
         self.__preln = None
         self.__K_tensor = None
 
         # Define calc shortcut
         self.calc = dislocation_array
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'dislocation_periodic_array.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/README.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/dislocation_periodic_array.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/dislocation_periodic_array.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array/theory.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/DislocationPeriodicArrayStress.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/DislocationPeriodicArrayStress.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/README.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calc_dislocation_periodic_array_stress.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calc_dislocation_periodic_array_stress.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calc_dislocation_periodic_array_stress.template` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calc_dislocation_periodic_array_stress.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/CalculationDislocationPeriodicArrayStress.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/CalculationDislocationPeriodicArrayStress.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/README.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/calculation_dislocation_periodic_array_stress/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/dislarray_free_stress.template` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/dislarray_free_stress.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/dislarray_rigid_stress.template` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/dislarray_rigid_stress.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_periodic_array_stress/theory.md` & `iprPy-0.11.6/iprPy/calculation/dislocation_periodic_array_stress/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/522c8437-eceb-480d-8f0c-77f83cdb3125.json` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/522c8437-eceb-480d-8f0c-77f83cdb3125.json`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/base.dat` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/base.dat`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc/110-edge.json` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc/110-edge.json`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc/111-screw.json` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc/111-screw.json`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc/112-edge.json` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc/112-edge.json`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/bcc.json` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/bcc.json`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.in` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.template` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/calc_dislocation_vacancy.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/create_sys.in` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/create_sys.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl.dat` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl.dat`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl.dump` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl.dump`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax.in` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax.template` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax_script.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/disl_relax_script.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/fcc.json` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/fcc.json`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/log.lammps` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/log.lammps`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/calc_files/results.json` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/calc_files/results.json`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/data_model.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/data_model.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/prepare.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/prepare.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/dislocation_vacancy/read_input.py` & `iprPy-0.11.6/iprPy/calculation/dislocation_vacancy/read_input.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/__init__.py` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.in` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.in`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.py` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.template` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/calc_dynamic_elastic.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_dynamic/full_relax.template` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_dynamic/full_relax.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_static/ElasticConstantsStatic.py` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_static/ElasticConstantsStatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,33 @@
     """Class for managing static elastic constants calculations from small strains"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -68,15 +74,15 @@
         self.__raw_Cij_positive = None
         self.__raw_Cij_negative = None
 
         # Define calc shortcut
         self.calc = elastic_constants_static
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'elastic_constants_static.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_static/README.md` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_static/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_static/cij.template` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_static/cij.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_static/elastic_constants_static.py` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_static/elastic_constants_static.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/elastic_constants_static/theory.md` & `iprPy-0.11.6/iprPy/calculation/elastic_constants_static/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/energy_check/EnergyCheck.py` & `iprPy-0.11.6/iprPy/calculation/energy_check/EnergyCheck.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,33 @@
     """Class for managing potential energy checks of structures"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -55,15 +61,15 @@
         # Initialize unique calculation attributes
         self.__potential_energy = None
 
         # Define calc shortcut
         self.calc = energy_check
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'energy_check.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/energy_check/README.md` & `iprPy-0.11.6/iprPy/calculation/energy_check/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/energy_check/energy_check.py` & `iprPy-0.11.6/iprPy/calculation/energy_check/energy_check.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy/FreeEnergy.py` & `iprPy-0.11.6/iprPy/calculation/free_energy/FreeEnergy.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,27 +29,33 @@
     """Class for managing dynamic relaxations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -80,15 +86,15 @@
         self.__helmholtz = None
         self.__gibbs = None
 
         # Define calc shortcut
         self.calc = free_energy
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'free_energy.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy/README.md` & `iprPy-0.11.6/iprPy/calculation/free_energy/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy/free_energy.py` & `iprPy-0.11.6/iprPy/calculation/free_energy/free_energy.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy/free_energy.template` & `iprPy-0.11.6/iprPy/calculation/free_energy/free_energy.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy/msd.template` & `iprPy-0.11.6/iprPy/calculation/free_energy/msd.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy/theory.md` & `iprPy-0.11.6/iprPy/calculation/free_energy/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy_liquid/FreeEnergyLiquid.py` & `iprPy-0.11.6/iprPy/calculation/free_energy_liquid/FreeEnergyLiquid.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,33 @@
     """Class for managing dynamic relaxations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -76,15 +82,15 @@
         self.__helmholtz = None
         self.__gibbs = None
 
         # Define calc shortcut
         self.calc = free_energy_liquid
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'free_energy_liquid.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy_liquid/README.md` & `iprPy-0.11.6/iprPy/calculation/free_energy_liquid/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy_liquid/UhlenbeckFordModel.py` & `iprPy-0.11.6/iprPy/calculation/free_energy_liquid/UhlenbeckFordModel.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy_liquid/free_energy_liquid.py` & `iprPy-0.11.6/iprPy/calculation/free_energy_liquid/free_energy_liquid.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy_liquid/free_energy_liquid.template` & `iprPy-0.11.6/iprPy/calculation/free_energy_liquid/free_energy_liquid.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/free_energy_liquid/theory.md` & `iprPy-0.11.6/iprPy/calculation/free_energy_liquid/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/__init__.py` & `iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/__init__.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/calc_bcc_grain_boundary.py` & `iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/calc_bcc_grain_boundary.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/calc_bcc_grain_boundary.template` & `iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/calc_bcc_grain_boundary.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/grain_boundary_bcc/grain_boundary.template` & `iprPy-0.11.6/iprPy/calculation/grain_boundary_bcc/grain_boundary.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/grain_boundary_search/README.md` & `iprPy-0.11.6/iprPy/calculation/grain_boundary_search/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/grain_boundary_search/compare_terms.py` & `iprPy-0.11.6/iprPy/calculation/grain_boundary_search/compare_terms.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/grain_boundary_search/todict.py` & `iprPy-0.11.6/iprPy/calculation/grain_boundary_search/todict.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/isolated_atom/IsolatedAtom.py` & `iprPy-0.11.6/iprPy/calculation/isolated_atom/IsolatedAtom.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,27 +20,33 @@
     """Class for managing isolated atom energy calculations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -53,15 +59,15 @@
         # Initialize unique calculation attributes
         self.__isolated_atom_energy = {}
 
         # Define calc shortcut
         self.calc = isolated_atom
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'isolated_atom.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/isolated_atom/README.md` & `iprPy-0.11.6/iprPy/calculation/isolated_atom/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/isolated_atom/calculation_isolated_atom.xsl` & `iprPy-0.11.6/iprPy/calculation/isolated_atom/calculation_isolated_atom.xsl`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/isolated_atom/isolated_atom.py` & `iprPy-0.11.6/iprPy/calculation/isolated_atom/isolated_atom.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/isolated_atom/theory.md` & `iprPy-0.11.6/iprPy/calculation/isolated_atom/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/phonon/Phonon.py` & `iprPy-0.11.6/iprPy/calculation/phonon/Phonon.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,33 @@
     """Class for managing phonon and quasiharmonic calculations using phonopy"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -78,15 +84,15 @@
         self.__phonons = None
         self.__qha = None
 
         # Define calc shortcut
         self.calc = phonon_quasiharmonic
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'calc_phonon.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/phonon/README.md` & `iprPy-0.11.6/iprPy/calculation/phonon/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/phonon/calc_phonon.py` & `iprPy-0.11.6/iprPy/calculation/phonon/calc_phonon.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/phonon/theory.md` & `iprPy-0.11.6/iprPy/calculation/phonon/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/PointDefectDiffusion.py` & `iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/PointDefectDiffusion.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/README.md` & `iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/diffusion.template` & `iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/diffusion.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/point_defect_diffusion.py` & `iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/point_defect_diffusion.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_diffusion/theory.md` & `iprPy-0.11.6/iprPy/calculation/point_defect_diffusion/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_static/PointDefectStatic.py` & `iprPy-0.11.6/iprPy/calculation/point_defect_static/PointDefectStatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,33 @@
     """Class for managing point defect formation calculations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -79,15 +85,15 @@
         self.__position_shift = None
         self.__db_vect_shift = None
 
         # Define calc shortcut
         self.calc = calc
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'point_defect_static.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_static/README.md` & `iprPy-0.11.6/iprPy/calculation/point_defect_static/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_static/point_defect_static.py` & `iprPy-0.11.6/iprPy/calculation/point_defect_static/point_defect_static.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/point_defect_static/theory.md` & `iprPy-0.11.6/iprPy/calculation/point_defect_static/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_box/README.md` & `iprPy-0.11.6/iprPy/calculation/relax_box/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_box/RelaxBox.py` & `iprPy-0.11.6/iprPy/calculation/relax_box/RelaxBox.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,33 @@
     """Class for managing box-only relaxations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -75,15 +81,15 @@
         self.__measured_pressure_xz = None
         self.__measured_pressure_yz = None
 
         # Define calc shortcut
         self.calc = relax_box
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'relax_box.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_box/cij_run0.template` & `iprPy-0.11.6/iprPy/calculation/relax_box/cij_run0.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_box/relax_box.py` & `iprPy-0.11.6/iprPy/calculation/relax_box/relax_box.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_box/theory.md` & `iprPy-0.11.6/iprPy/calculation/relax_box/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_dynamic/README.md` & `iprPy-0.11.6/iprPy/calculation/relax_dynamic/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_dynamic/RelaxDynamic.py` & `iprPy-0.11.6/iprPy/calculation/relax_dynamic/RelaxDynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,33 @@
     """Class for managing dynamic relaxations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -112,15 +118,15 @@
         self.__measured_temperature = None
         self.__measured_temperature_std = None
 
         # Define calc shortcut
         self.calc = relax_dynamic
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'relax_dynamic.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_dynamic/full_relax.template` & `iprPy-0.11.6/iprPy/calculation/relax_dynamic/full_relax.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_dynamic/full_relax_restart.template` & `iprPy-0.11.6/iprPy/calculation/relax_dynamic/full_relax_restart.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_dynamic/relax_dynamic.py` & `iprPy-0.11.6/iprPy/calculation/relax_dynamic/relax_dynamic.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_dynamic/theory.md` & `iprPy-0.11.6/iprPy/calculation/relax_dynamic/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_liquid/README.md` & `iprPy-0.11.6/iprPy/calculation/relax_liquid/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Introduction
 
 The relax_liquid calculation style is designed to generate and characterize a liquid phase configuration for an atomic potential based on an initial configuration, target temperature and target pressure.  The calculation involves multiple stages of relaxation and computes the mean squared displacement and radial distribution functions on the final liquid.
 
 ### Version notes
 
-- 2022-10-??: Calculation created
+- 2022-10-12: Calculation created
 
 ### Additional dependencies
 
 ### Disclaimers
 
 - [NIST disclaimers](http://www.nist.gov/public_affairs/disclaimer.cfm)
 - No active checks are performed by this calculation to ensure that the system is liquid. Be sure to check the final atomic configurations. The thermo output can also provide a rough guideline in that you should see convergence of volume but not of the individual lx, ly, lz dimensions for a liquid phase.
```

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_liquid/RelaxLiquid.py` & `iprPy-0.11.6/iprPy/calculation/relax_liquid/RelaxLiquid.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,33 @@
     """Class for managing dynamic relaxations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -69,14 +75,15 @@
 
         self.meltsteps = 50000
         self.coolsteps = 10000
         self.equilvolumesteps = 50000
         self.equilenergysteps = 10000
         self.runsteps = 50000
         self.dumpsteps = None
+        self.restartsteps = None
 
         self.equilvolumesamples = 300
         self.equilenergysamples = 100
         self.equilenergystyle = 'pe'
 
         self.rdfcutoff = None
 
@@ -98,15 +105,15 @@
         self.__msd_values = None
         self.__lammps_output = None
 
         # Define calc shortcut
         self.calc = relax_liquid
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'relax_liquid.py',
@@ -197,14 +204,31 @@
             self.__dumpsteps = None
         else:
             val = int(val)
             assert val >= 0
             self.__dumpsteps = val
 
     @property
+    def restartsteps(self) -> int:
+        """int: How often to dump restart files during the final run."""
+        if self.__restartsteps is None:
+            return self.meltsteps + self.coolsteps + self.equilvolumesteps + self.equilenergysteps + self.runsteps
+        else:
+            return self.__restartsteps
+
+    @restartsteps.setter
+    def restartsteps(self, val: Optional[int]):
+        if val is None:
+            self.__restartsteps = None
+        else:
+            val = int(val)
+            assert val >= 0
+            self.__restartsteps = val
+
+    @property
     def meltsteps(self) -> int:
         """int: Number of MD steps during the melting stage"""
         return self.__meltsteps
 
     @meltsteps.setter
     def meltsteps(self, val: int):
         val = int(val)
@@ -485,14 +509,17 @@
             energy.
         runsteps : int or None, optional
             The number of nve integration steps to perform on the system to
             obtain measurements of MSD and RDF of the liquid.
         dumpsteps : int or None, optional
             Dump files will be saved every this many steps during the runsteps
             simulation.
+        restartsteps : int or None, optional
+            Dump files will be saved every this many steps during the runsteps
+            simulation.
         randomseed : int or None, optional
             Random number seed used by LAMMPS in creating velocities and with
             the Langevin thermostat.
         **kwargs : any, optional
             Any keyword parameters supported by the set_values() methods of
             the parent Calculation class and the subset classes.
         """
@@ -520,14 +547,16 @@
             self.equilenergysteps = kwargs['equilenergysteps']
         if 'thermosteps' in kwargs:
             self.thermosteps = kwargs['thermosteps']
         if 'runsteps' in kwargs:
             self.runsteps = kwargs['runsteps']
         if 'dumpsteps' in kwargs:
             self.dumpsteps = kwargs['dumpsteps']
+        if 'restartsteps' in kwargs:
+            self.restartsteps = kwargs['restartsteps']
         if 'equilvolumesamples' in kwargs:
             self.equilvolumesamples = kwargs['equilvolumesamples']
         if 'equilenergysamples' in kwargs:
             self.equilenergysamples = kwargs['equilenergysamples']
         if 'equilenergystyle' in kwargs:
             self.equilenergystyle = kwargs['equilenergystyle']
 
@@ -567,14 +596,15 @@
         self.coolsteps = int(input_dict.get('coolsteps', 10000))
         self.equilvolumesteps = int(input_dict.get('equilvolumesteps', 50000))
         self.equilvolumesamples = int(input_dict.get('equilvolumesamples', 300))
         self.equilenergysteps = int(input_dict.get('equilenergysteps', 10000))
         self.equilenergysamples = int(input_dict.get('equilenergysamples', 100))
         self.runsteps = int(input_dict.get('runsteps', 50000))
         self.dumpsteps = input_dict.get('dumpsteps', None)
+        self.restartsteps = input_dict.get('restartsteps', None)
         self.randomseed = input_dict.get('randomseed', None)
 
         # Load calculation-specific unitless floats
         self.temperature = float(input_dict['temperature'])
         self.temperature_melt = float(input_dict.get('temperature_melt', 3000.0))
 
         # Load calculation-specific floats with units
@@ -771,14 +801,18 @@
                 "The number of nve integration steps to perform on the system to",
                 "obtain measurements of MSD and RDF of the liquid. Default value is",
                 "50000."]),
             'dumpsteps': ' '.join([
                 "Dump files will be saved every this many steps during the runsteps",
                 "simulation. Default is None, which sets dumpsteps equal to the sum",
                 "of all other steps values so only the final configuration is saved."]),
+            'restartsteps': ' '.join([
+                "Restart files will be saved every this many steps. Default is None",
+                "which sets restartsteps equal to the sum",
+                "of all other steps values so only the final configuration is saved."]),
             'randomseed': ' '.join([
                 "Random number seed used by LAMMPS in creating velocities and with",
                 "the Langevin thermostat.  Default is None which will select a",
                 "random int between 1 and 900000000."]),
         }
 
     @property
@@ -842,14 +876,15 @@
                     'equilvolumesteps',
                     'equilvolumesamples',
                     'equilenergysteps',
                     'equilenergysamples',
                     'equilenergystyle',
                     'runsteps',
                     'dumpsteps',
+                    'restartsteps',
                     'randomseed',
                 ]
             ]
         )
         return keys
 
 ########################### Data model interactions ###########################
@@ -1104,14 +1139,15 @@
         input_dict['equilvolumesteps'] = self.equilvolumesteps
         input_dict['equilvolumesamples'] = self.equilvolumesamples
         input_dict['equilenergysteps'] = self.equilenergysteps
         input_dict['equilenergysamples'] = self.equilenergysamples
         input_dict['equilenergystyle'] = self.equilenergystyle
         input_dict['runsteps'] = self.runsteps
         input_dict['dumpsteps'] = self.dumpsteps
+        input_dict['restartsteps'] = self.restartsteps
         input_dict['randomseed'] = self.randomseed
 
         # Return input_dict
         return input_dict
 
     def process_results(self, results_dict: dict):
         """
```

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_liquid/liquid_ave_pe.template` & `iprPy-0.11.6/iprPy/calculation/relax_liquid/liquid_ave_pe.template`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 
 variable ghostcutoff equal <rdfcutoff>+2.01
 comm_modify cutoff ${ghostcutoff}
 
 # Dump configurations
 dump dumpit all custom <dumpsteps> *.dump <dump_keys>
 dump_modify dumpit format <dump_modify_format>
+restart <restartsteps> *.restart
 
 # Change thermo to report msd
 thermo 100
 thermo_style custom step temp pe ke etotal pxx pyy pzz c_msd[1] c_msd[2] c_msd[3] c_msd[4]
 thermo_modify format float %.13e
 
 fix nve all nve
```

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_liquid/liquid_ave_te.template` & `iprPy-0.11.6/iprPy/calculation/relax_liquid/liquid_ave_te.template`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 
 variable ghostcutoff equal <rdfcutoff>+2.01
 comm_modify cutoff ${ghostcutoff}
 
 # Dump configurations
 dump dumpit all custom <dumpsteps> *.dump <dump_keys>
 dump_modify dumpit format <dump_modify_format>
+restart <restartsteps> *.restart
 
 # Change thermo to report msd
 thermo 100
 thermo_style custom step temp pe ke etotal pxx pyy pzz c_msd[1] c_msd[2] c_msd[3] c_msd[4]
 thermo_modify format float %.13e
 
 fix nve all nve
```

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_liquid/relax_liquid.py` & `iprPy-0.11.6/iprPy/calculation/relax_liquid/relax_liquid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding: utf-8
 
 # Python script created by Lucas Hale
 
 # Standard library imports
-from distutils.command.config import dump_file
 from pathlib import Path
 import datetime
 import random
 from typing import Optional
 
 # https://github.com/usnistgov/atomman 
 import atomman as am
@@ -33,14 +32,15 @@
                  equilvolumesteps: int = 50000,
                  equilvolumesamples: int = 300,
                  equilenergysteps: int = 10000,
                  equilenergysamples: int = 100,
                  equilenergystyle: str = 'pe',
                  runsteps: int = 50000,
                  dumpsteps: Optional[int] = None,
+                 restartsteps: Optional[int] = None,
                  createvelocities: bool = True,
                  randomseed: Optional[int] = None) -> dict:
     """
     Performs a multi-stage simulation to obtain a liquid phase configuration 
     at a given temperature. Radial displacement functions and mean squared
     displacements are automatically computed for the system.
     
@@ -102,14 +102,18 @@
         The number of nve integration steps to perform on the system to
         obtain measurements of MSD and RDF of the liquid. Default value is
         50000.
     dumpsteps : int or None, optional
         Dump files will be saved every this many steps during the runsteps
         simulation. Default is None, which sets dumpsteps equal to the sum of
         all "steps" terms above so that only the final configuration is saved.
+    restartsteps : int or None, optional
+        Restart files will be saved every this many steps.  Default is None,
+        which sets dumpsteps equal to the sum of all "steps" terms above so
+        that only the final configuration is saved.
     createvelocities : bool, optional
         If True (default), velocities will be created for the atoms prior to
         running the simulations.  Setting this to False can be useful if the
         initial system already has velocity information.
     randomseed : int or None, optional
         Random number seed used by LAMMPS in creating velocities and with
         the Langevin thermostat.  Default is None which will select a
@@ -145,57 +149,64 @@
         - **'measured_press_stderr'** (*float*) - The standard error in the measured
           pressure values of the nve stage.
         - **'time_values'** (*numpy.array of float*) - The values of time that
           correspond to the mean squared displacement values.
         - **'msd_x_values'** (*numpy.array of float*) - The mean squared displacement
           values only in the x direction.
         - **'msd_y_values'** (*numpy.array of float*) - The mean squared displacement
-         values only in the y direction.
+          values only in the y direction.
         - **'msd_z_values'** (*numpy.array of float*) - The mean squared displacement
-         values only in the z direction.
+          values only in the z direction.
         - **'msd_values'** (*numpy.array of float*) - The total mean squared
-           displacement values.
+          displacement values.
         - **'lammps_output'** (*atomman.lammps.Log*) - The LAMMPS logfile output.
           Can be useful for checking the thermo data at each simulation stage.
+    
     """
-  
+
     if equilenergystyle not in ['pe', 'te']:
         raise ValueError('invalid equilenergystyle option: must be "pe" or "te"')
 
     # Get lammps units
     lammps_units = lmp.style.unit(potential.units)
-    
+
     #Get lammps version date
     lammps_date = lmp.checkversion(lammps_command)['date']
     
     # Handle default values
     if dumpsteps is None:
         dumpsteps = meltsteps + coolsteps + equilvolumesteps + equilenergysteps + runsteps
-    
+    if restartsteps is None:
+        restartsteps = meltsteps + coolsteps + equilvolumesteps + equilenergysteps + runsteps
+
     # Check volrelax and temprelax settings
     if equilvolumesamples > equilvolumesteps / 100:
         raise ValueError('invalid values: equilvolumesamples must be <= equilvolumesteps / 100')
     if equilenergysamples > equilenergysteps / 100:
         raise ValueError('invalid values: equilenergysamples must be <= equilenergysteps / 100')
 
     # Set default rdfcutoff
     if rdfcutoff is None:
         rdfcutoff = 4 * system.r0()
 
     # Define lammps variables
     lammps_variables = {}
-    
+
     lammps_variables['boltzmann'] = uc.get_in_units(uc.unit['kB'],
                                                     lammps_units['energy'])
-    
+
     # Dump initial system as data and build LAMMPS inputs
     system_info = system.dump('atom_data', f='init.dat',
                               potential=potential)
     lammps_variables['atomman_system_pair_info'] = system_info
 
+    # Generate LAMMPS inputs for restarting
+    system_info2 = potential.pair_restart_info('*.restart', system.symbols)
+    lammps_variables['atomman_pair_restart_info'] = system_info2
+
     # Phase settings
     lammps_variables['temperature'] = temperature
     lammps_variables['temperature_melt'] = temperature_melt
     lammps_variables['pressure'] = pressure
 
     # Set timestep dependent parameters
     timestep = lmp.style.timestep(potential.units)
@@ -206,14 +217,15 @@
     # Number of run/dump steps
     lammps_variables['meltsteps'] = meltsteps
     lammps_variables['coolsteps'] = coolsteps
     lammps_variables['equilvolumesteps'] = equilvolumesteps
     lammps_variables['equilenergysteps'] = equilenergysteps
     lammps_variables['runsteps'] = runsteps
     lammps_variables['dumpsteps'] = dumpsteps
+    lammps_variables['restartsteps'] = restartsteps
 
     # Number of samples
     lammps_variables['equilvolumesamples'] = equilvolumesamples
     lammps_variables['equilenergysamples'] = equilenergysamples
     
     lammps_variables['rdfcutoff'] = rdfcutoff
 
@@ -241,45 +253,71 @@
     if lammps_date < datetime.date(2016, 8, 3):
         if potential.atom_style in ['charge']:
             lammps_variables['dump_modify_format'] = f'"%d %d{8 * " %.13e"}"'
         else:
             lammps_variables['dump_modify_format'] = f'"%d %d{7 * " %.13e"}"'
     else:
         lammps_variables['dump_modify_format'] = 'float %.13e'
-    
+
     # Write lammps input script
     lammps_script = 'liquid.in'
     lammps_template = f'liquid_ave_{equilenergystyle}.template'
     template = read_calc_file('iprPy.calculation.relax_liquid', lammps_template)
-    with open(lammps_script, 'w') as f:
+    with open(lammps_script, 'w', encoding='UTF-8') as f:
         f.write(filltemplate(template, lammps_variables, '<', '>'))
-    
-    # Run lammps 
+
+    # Write lammps restart input script
+    restart_script = 'liquid_restart.in'
+    lammps_template = 'liquid_restart.template'
+    template = read_calc_file('iprPy.calculation.relax_liquid', lammps_template)
+    with open(restart_script, 'w', encoding='UTF-8') as f:
+        f.write(filltemplate(template, lammps_variables, '<', '>'))
+
+    # Fix for restart runs: only use restart script if restart file(s) exist
+    if Path('log.lammps').exists() and len(list(Path('.').glob('*.restart'))) == 0:
+        Path('log.lammps').unlink()
+
+    # Uniquely rename rdf.txt on restarts to prevent overwrite
+    elif Path('rdf.txt').exists():
+        maxrdfid = 0
+        for oldrdf in Path('.').glob('rdf-*.txt'):
+            rdfid = int(oldrdf.stem.split('-')[-1])
+            if rdfid > maxrdfid:
+                maxrdfid = rdfid
+        Path('rdf.txt').rename(f'rdf-{maxrdfid+1}.txt')
+
+    # Run lammps
     output = lmp.run(lammps_command, script_name=lammps_script,
+                     restart_script_name=restart_script,
                      mpi_command=mpi_command, screen=False)
-    
-    # Extract LAMMPS thermo data. 
-    #thermo_melt = output.simulations[0].thermo
-    #thermo_cool = output.simulations[1].thermo
-    thermo_vol_equil = output.simulations[2].thermo
-    thermo_temp_equil = output.simulations[3].thermo
-    thermo_nve = output.simulations[4].thermo
+
+    # Extract LAMMPS thermo data.
+    run1steps = meltsteps
+    run2steps = run1steps + coolsteps
+    run3steps = run2steps + equilvolumesteps
+    run4steps = run3steps + equilenergysteps
+    thermo = output.flatten()['thermo']
+    #thermo_melt = thermo[thermo.Step < run1steps]
+    #thermo_cool = thermo[(thermo.Step < run2steps) & (thermo.Step >= run1steps)]
+    thermo_vol_equil = thermo[(thermo.Step < run3steps) & (thermo.Step >= run2steps)]
+    thermo_temp_equil = thermo[(thermo.Step < run4steps) & (thermo.Step >= run3steps)]
+    thermo_nve = thermo[thermo.Step >= run4steps]
 
     results = {}
-    
+
     # Set final dumpfile info
     last_dump_number = 0
     for dump_file in Path('.').glob('*.dump'):
         dump_number = int(dump_file.name[:-5])
         if dump_number > last_dump_number:
             last_dump_number = dump_number
     last_dump_file = f'{last_dump_number}.dump'
     results['dumpfile_final'] = last_dump_file
     results['symbols_final'] = system.symbols
-    
+
     natoms = system.natoms
 
     # Get equilibrated volume 
     volume_unit = f"{lammps_units['length']}^3"
     samplestart = len(thermo_vol_equil) - equilvolumesamples
     results['volume'] = uc.set_in_units(thermo_temp_equil.Volume.values[-1], volume_unit) / natoms
     results['volume_stderr'] = uc.set_in_units(thermo_vol_equil.Volume[samplestart:].std(), volume_unit) / natoms / (equilvolumesamples)**0.5
@@ -294,20 +332,20 @@
     # Get measured temperature and pressure during the nve run
     nsamples = len(thermo_nve)
     results['measured_temp'] = thermo_nve.Temp.values.mean()
     results['measured_temp_stderr'] = thermo_nve.Temp.values.std() / (nsamples)**0.5
     pressure = (thermo_nve.Pxx.values + thermo_nve.Pyy.values + thermo_nve.Pzz.values) / 3
     results['measured_press'] = uc.set_in_units(pressure.mean(), lammps_units['pressure'])
     results['measured_press_stderr'] = uc.set_in_units(pressure.std(), lammps_units['pressure']) / (nsamples)**0.5
-    
+
     # Get MSD values
     msd_unit = f"{lammps_units['length']}^2"
     time = (thermo_nve.Step.values - thermo_nve.Step.values[0]) * timestep
     results['time_values'] = uc.set_in_units(time, lammps_units['time'])
     results['msd_x_values'] = uc.set_in_units(thermo_nve['c_msd[1]'].values, msd_unit)
     results['msd_y_values'] = uc.set_in_units(thermo_nve['c_msd[2]'].values, msd_unit)
     results['msd_z_values'] = uc.set_in_units(thermo_nve['c_msd[3]'].values, msd_unit)
     results['msd_values'] = uc.set_in_units(thermo_nve['c_msd[4]'].values, msd_unit)
 
     results['lammps_output'] = output
 
-    return results
+    return results
```

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_liquid/theory.md` & `iprPy-0.11.6/iprPy/calculation/relax_liquid/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_static/README.md` & `iprPy-0.11.6/iprPy/calculation/relax_static/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_static/RelaxStatic.py` & `iprPy-0.11.6/iprPy/calculation/relax_static/RelaxStatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,27 +23,33 @@
     """Class for managing static relaxations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -80,15 +86,15 @@
         self.__measured_pressure_xz = None
         self.__measured_pressure_yz = None
 
         # Define calc shortcut
         self.calc = relax_static
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'relax_static.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_static/minbox.template` & `iprPy-0.11.6/iprPy/calculation/relax_static/minbox.template`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_static/relax_static.py` & `iprPy-0.11.6/iprPy/calculation/relax_static/relax_static.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/relax_static/theory.md` & `iprPy-0.11.6/iprPy/calculation/relax_static/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/README.md` & `iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/StackingFaultMap2D.py` & `iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/StackingFaultMap2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,27 +114,33 @@
     """Class for managing 2D maps of stacking fault energy calculations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -156,15 +162,15 @@
         self.__paths = None
         self.__E_isf = None
 
         # Define calc shortcut
         self.calc = stackingfaultmap
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'stacking_fault_map_2D.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/stacking_fault_map_2D.py` & `iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/stacking_fault_map_2D.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/stacking_fault_map_2D/theory.md` & `iprPy-0.11.6/iprPy/calculation/stacking_fault_map_2D/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/stacking_fault_static/README.md` & `iprPy-0.11.6/iprPy/calculation/stacking_fault_static/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/stacking_fault_static/StackingFaultStatic.py` & `iprPy-0.11.6/iprPy/calculation/stacking_fault_static/StackingFaultStatic.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,27 +22,33 @@
     """Class for managing stacking fault energy calculations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -66,15 +72,15 @@
         self.__gsf_energy = None
         self.__gsf_displacement = None
 
         # Define calc shortcut
         self.calc = stackingfault
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'stacking_fault_static.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/stacking_fault_static/stacking_fault_static.py` & `iprPy-0.11.6/iprPy/calculation/stacking_fault_static/stacking_fault_static.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/stacking_fault_static/theory.md` & `iprPy-0.11.6/iprPy/calculation/stacking_fault_static/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/surface_energy_static/README.md` & `iprPy-0.11.6/iprPy/calculation/surface_energy_static/README.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/surface_energy_static/SurfaceEnergyStatic.py` & `iprPy-0.11.6/iprPy/calculation/surface_energy_static/SurfaceEnergyStatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,33 @@
     """Class for managing free surface energy calculations"""
 
 ############################# Core properties #################################
 
     def __init__(self,
                  model: Union[str, Path, IOBase, DM, None]=None,
                  name: Optional[str]=None,
+                 database = None,
                  params: Union[str, Path, IOBase, dict] = None,
                  **kwargs: any):
         """
         Initializes a Calculation object for a given style.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             Record content in data model format to read in.  Cannot be given
             with params.
         name : str, optional
             The name to use for saving the record.  By default, this should be
             the calculation's key.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         params : str, file-like object or dict, optional
             Calculation input parameters or input parameter file.  Cannot be
             given with model.
         **kwargs : any
             Any other core Calculation record attributes to set.  Cannot be
             given with model.
         """
@@ -64,15 +70,15 @@
         self.__potential_energy = None
         self.__surface_energy = None
 
         # Define calc shortcut
         self.calc = surface_energy_static
 
         # Call parent constructor
-        super().__init__(model=model, name=name, params=params,
+        super().__init__(model=model, name=name, database=database, params=params,
                          subsets=subsets, **kwargs)
 
     @property
     def filenames(self) -> list:
         """list: the names of each file used by the calculation."""
         return [
             'surface_energy_static.py',
```

### Comparing `iprPy-0.11.5/iprPy/calculation/surface_energy_static/surface_energy_static.py` & `iprPy-0.11.6/iprPy/calculation/surface_energy_static/surface_energy_static.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation/surface_energy_static/theory.md` & `iprPy-0.11.6/iprPy/calculation/surface_energy_static/theory.md`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/AtommanElasticConstants.py` & `iprPy-0.11.6/iprPy/calculation_subset/AtommanElasticConstants.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/AtommanGammaSurface.py` & `iprPy-0.11.6/iprPy/calculation_subset/AtommanGammaSurface.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/AtommanSystemLoad.py` & `iprPy-0.11.6/iprPy/calculation_subset/AtommanSystemLoad.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/AtommanSystemManipulate.py` & `iprPy-0.11.6/iprPy/calculation_subset/AtommanSystemManipulate.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/CalculationSubset.py` & `iprPy-0.11.6/iprPy/calculation_subset/CalculationSubset.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/Dislocation.py` & `iprPy-0.11.6/iprPy/calculation_subset/Dislocation.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/FreeSurface.py` & `iprPy-0.11.6/iprPy/calculation_subset/FreeSurface.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/LammpsCommands.py` & `iprPy-0.11.6/iprPy/calculation_subset/LammpsCommands.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/LammpsMinimize.py` & `iprPy-0.11.6/iprPy/calculation_subset/LammpsMinimize.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/LammpsPotential.py` & `iprPy-0.11.6/iprPy/calculation_subset/LammpsPotential.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/PointDefect.py` & `iprPy-0.11.6/iprPy/calculation_subset/PointDefect.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/StackingFault.py` & `iprPy-0.11.6/iprPy/calculation_subset/StackingFault.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/Units.py` & `iprPy-0.11.6/iprPy/calculation_subset/Units.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/calculation_subset/__init__.py` & `iprPy-0.11.6/iprPy/calculation_subset/__init__.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/command_line.py` & `iprPy-0.11.6/iprPy/command_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 # Standard Python libraries
 import argparse
 
+import atomman as am
+
 # https://github.com/usnistgov/iprPy
 from . import (load_database, load_run_directory, load_calculation,
                check_modules, settings)
 from .calculation import run_calculation
 from .database import reset_orphans
 from .tools import filltemplate
 
@@ -108,46 +110,50 @@
     # Actions for subcommand templatedoc
     elif args.action == 'templatedoc':
         calculation = load_calculation(args.calculation)
         print(calculation.templatedoc)
 
     # Actions for subcommand retrieve
     elif args.action == 'retrieve':
-        database = load_database(args.database)
+
+        potdb = am.library.Database(remote_name=args.remote_database,
+                                    local_name=args.local_database)
+
         style = args.record_style
         if args.compact is True:
             indent = None
         else:
             indent = 4
 
         # Call style-specific retrieve for extra functionality
         if style in ['potential_LAMMPS', 'potential_LAMMPS_KIM']:
+
             if args.getfiles is True:
                 pot_dir_style = 'id'
                 getfiles = True
             else:
-                pot_dir_style = 'local'
+                pot_dir_style = 'working'
                 getfiles = False
 
-            database.potdb.retrieve_lammps_potential(name=args.record_name,
-                                                     getfiles=getfiles,
-                                                     format=args.format,
-                                                     indent=indent,
-                                                     pot_dir_style=pot_dir_style,
-                                                     verbose=True)
+            potdb.retrieve_lammps_potential(name=args.record_name,
+                                            getfiles=getfiles,
+                                            format=args.format,
+                                            indent=indent,
+                                            pot_dir_style=pot_dir_style,
+                                            verbose=True)
         elif style == 'Citation':
-            database.potdb.retrieve_citation(name=args.record_name,
-                                             format=args.format, indent=indent,
-                                             verbose=True)
+            potdb.retrieve_citation(name=args.record_name,
+                                    format=args.format, indent=indent,
+                                    verbose=True)
 
         # Call generic retrieve
         else:
-            database.potdb.retrieve_record(style=style, name=args.record_name,
-                                           format=args.format, indent=indent,
-                                           verbose=True)
+            potdb.retrieve_record(style=style, name=args.record_name,
+                                  format=args.format, indent=indent,
+                                  verbose=True)
 
     # Actions for subcommand run
     elif args.action == 'run':
         run_calculation(args.filename, calc_style=args.calc_style,
                         raise_error=args.raise_error)
 
     # Actions for subcommand runner
@@ -347,26 +353,28 @@
                         help="view the documentation for a calculation's methods and theory")
     subparser.add_argument('calculation',
                         help='calculation name')
 
     # Define subparser for retrieve
     subparser = subparsers.add_parser('retrieve',
                         help="copy/download a record to the working directory")
-    subparser.add_argument('database',
-                        help='database name')
     subparser.add_argument('record_style',
                         help='style of the record to retrieve')
     subparser.add_argument('record_name',
                         help='the name of the record in the database to retrieve')
+    subparser.add_argument('-l', '--local_database', default=None,
+                        help='specify the local database name to search for the matching record')
+    subparser.add_argument('-r', '--remote_database', default=None,
+                        help='specify the remote database name to search for the matching record')
     subparser.add_argument('-f', '--format', default='json', type=str,
                         help='the format to save the record as')
     subparser.add_argument('-c', '--compact', action='store_true',
                         help='indicates if the record is saved in compact format')
     subparser.add_argument('-g', '--getfiles', action='store_true',
-                        help='if used, any files associated with the record will also be retrieved')
+                        help='can be used with potential_LAMMPS records to automatically download any parameter files')
 
     # Define subparser for run
     subparser = subparsers.add_parser('run',
                         help='run a single calculation from a parameter file')
     subparser.add_argument('filename',
                         help='path to a parameter file')
     subparser.add_argument('calc_style', nargs='?', default=None,
```

### Comparing `iprPy-0.11.5/iprPy/database/IprPyDatabase.py` & `iprPy-0.11.6/iprPy/database/IprPyDatabase.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/database/MongoDatabase.py` & `iprPy-0.11.6/iprPy/database/MongoDatabase.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/database/__init__.py` & `iprPy-0.11.6/iprPy/database/__init__.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/database/load_database.py` & `iprPy-0.11.6/iprPy/database/load_database.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/database/master_prepare.py` & `iprPy-0.11.6/iprPy/database/master_prepare.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/database/prepare.py` & `iprPy-0.11.6/iprPy/database/prepare.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/database/reset_orphans.py` & `iprPy-0.11.6/iprPy/database/reset_orphans.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/database/runner.py` & `iprPy-0.11.6/iprPy/database/runner.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/fix_lammps_versions.py` & `iprPy-0.11.6/iprPy/fix_lammps_versions.py`

 * *Files 23% similar despite different names*

```diff
@@ -91,14 +91,28 @@
     """This is a list of all potentials that only work for older LAMMPS."""
     return [
         '1987--Ackland-G-J--Mo--LAMMPS--ipr1',
         '1987--Ackland-G-J--Mo--LAMMPS--ipr2',
         '2011--Bonny-G--Fe-Cr--LAMMPS--ipr1',
         '2013--Bonny-G--Fe-Cr-W--LAMMPS--ipr1',
         '2013--Smirnova-D-E--U-Mo-Xe--LAMMPS--ipr1',
+        '2016--Zhou-X-W--Al-Cu--LAMMPS--ipr1',
+
+        '2011--Bonny-G--Fe-Cr--LAMMPS--ipr2',
+        '2011--Bonny-G--Fe-Ni-Cr--LAMMPS--ipr1',
+        '2013--Bonny-G--Fe-Cr-W--LAMMPS--ipr2',
+        '2013--Gao-H--AgTaO3--LAMMPS--ipr2',
+        '2014--Nouranian-S--CH--ipr1',
+        '2015--Asadi-E--Fe--LAMMPS--ipr1',
+        '2015--Asadi-E--Ni--LAMMPS--ipr1',
+        '2018--Etesami-S-A--Cu--LAMMPS--ipr1',
+        '2018--Etesami-S-A--Ni--LAMMPS--ipr1',
+        '2018--Etesami-S-A--Fe--LAMMPS--ipr1',
+        '2018--Etesami-S-A--Pb-Sn--LAMMPS--ipr1',
+        '2021--Huang-X--Hf-Nb-Ta-Ti-Zr--LAMMPS--ipr1'
     ]
 
 def aenet_pots():
     """This is a list of aenet potentials (unofficial pair_style)."""
     return ['2020--Mori-H--Fe--LAMMPS--ipr1']
 
 def pinn_pots():
```

### Comparing `iprPy-0.11.5/iprPy/input/boolean.py` & `iprPy-0.11.6/iprPy/input/boolean.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos.py` & `iprPy-0.11.6/iprPy/input/buildcombos.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos_functions/README.rst` & `iprPy-0.11.6/iprPy/input/buildcombos_functions/README.rst`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos_functions/atomicarchive.py` & `iprPy-0.11.6/iprPy/input/buildcombos_functions/atomicarchive.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos_functions/atomicparent.py` & `iprPy-0.11.6/iprPy/input/buildcombos_functions/atomicparent.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos_functions/atomicreference.py` & `iprPy-0.11.6/iprPy/input/buildcombos_functions/atomicreference.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos_functions/crystalprototype.py` & `iprPy-0.11.6/iprPy/input/buildcombos_functions/crystalprototype.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos_functions/defect.py` & `iprPy-0.11.6/iprPy/input/buildcombos_functions/defect.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos_functions/diatom.py` & `iprPy-0.11.6/iprPy/input/buildcombos_functions/diatom.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/buildcombos_functions/lammpspotential.py` & `iprPy-0.11.6/iprPy/input/buildcombos_functions/lammpspotential.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/parse.py` & `iprPy-0.11.6/iprPy/input/parse.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/termtodict.py` & `iprPy-0.11.6/iprPy/input/termtodict.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/input/value.py` & `iprPy-0.11.6/iprPy/input/value.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/load_run_directory.py` & `iprPy-0.11.6/iprPy/load_run_directory.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialProperties.py` & `iprPy-0.11.6/iprPy/record/PotentialProperties.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,27 +20,33 @@
     """
     Class for representing PotentialProperties records that contain the data
     necessary to generate the properties pages for an interatomic potential.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs: any):
         """
         Initialize a PotentialProperties object.  Calculation-specific content
         is managed by PotentialPropertiesSubsets.
 
         Parameters
         ----------
         model : str, file-like object, DataModelDict
             The contents of the record.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         potential : BaseLAMMPSPotential, optional
             A record entry for a LAMMPS-compatible potential that the computed
             properties being compiled here are for.  Cannot be given with model
             or the other potential_ parameters as they provide the same
             information.
         potential_key : str, optional
             The UUID key of the potential that the computed properties being
@@ -85,15 +91,15 @@
             self.freesurfaces,
             self.stackingfaults,
             self.pointdefects,
             self.phonons
         ]
 
         # Call parent init
-        super().__init__(model=model, name=name, **kwargs)
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'PotentialProperties'
 
     @property
```

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/CrystalStructure.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/CrystalStructure.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/DiatomScan.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/DiatomScan.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/ElasticConstants.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/ElasticConstants.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/EvsRScan.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/EvsRScan.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/FreeSurface.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/FreeSurface.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/Phonon.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/Phonon.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/PointDefect.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/PointDefect.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/PotentialsPropertiesSubset.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/PotentialsPropertiesSubset.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/record/PotentialPropertiesSubsets/StackingFault.py` & `iprPy-0.11.6/iprPy/record/PotentialPropertiesSubsets/StackingFault.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/tools/__init__.py` & `iprPy-0.11.6/iprPy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/tools/dict_insert.py` & `iprPy-0.11.6/iprPy/tools/dict_insert.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/tools/dynamic_import.py` & `iprPy-0.11.6/iprPy/tools/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/tools/num_deriv_3_point.py` & `iprPy-0.11.6/iprPy/tools/num_deriv_3_point.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy/tools/read_calc_file.py` & `iprPy-0.11.6/iprPy/tools/read_calc_file.py`

 * *Files identical despite different names*

### Comparing `iprPy-0.11.5/iprPy.egg-info/PKG-INFO` & `iprPy-0.11.6/iprPy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: iprPy
-Version: 0.11.5
+Version: 0.11.6
 Summary: Interatomic Potential Repository Python Property Calculations and Tools
 Home-page: https://github.com/usnistgov/iprPy
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: atom,atomic,atomistic,molecular dynamics,high-throughput,interatomic potential
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.TXT
```

### Comparing `iprPy-0.11.5/iprPy.egg-info/SOURCES.txt` & `iprPy-0.11.6/iprPy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
 iprPy/calculation/relax_dynamic/theory.md
 iprPy/calculation/relax_liquid/README.md
 iprPy/calculation/relax_liquid/RelaxLiquid.py
 iprPy/calculation/relax_liquid/__init__.py
 iprPy/calculation/relax_liquid/calculation_relax_liquid.xsd
 iprPy/calculation/relax_liquid/liquid_ave_pe.template
 iprPy/calculation/relax_liquid/liquid_ave_te.template
+iprPy/calculation/relax_liquid/liquid_restart.template
 iprPy/calculation/relax_liquid/relax_liquid.py
 iprPy/calculation/relax_liquid/theory.md
 iprPy/calculation/relax_static/README.md
 iprPy/calculation/relax_static/RelaxStatic.py
 iprPy/calculation/relax_static/__init__.py
 iprPy/calculation/relax_static/calculation_relax_static.xsd
 iprPy/calculation/relax_static/minbox.template
```

### Comparing `iprPy-0.11.5/setup.py` & `iprPy-0.11.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,14 @@
       version = getversion(),
       description = 'Interatomic Potential Repository Python Property Calculations and Tools',
       long_description = getreadme(),
       classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Physics'
       ],
       keywords = [
@@ -40,20 +39,20 @@
       packages = find_packages(),
       install_requires = [
         'DataModelDict',
         'numpy', 
         'matplotlib',
         'scipy',
         'pandas',
-        'atomman==1.4.9',
+        'atomman>=1.4.10',
         'requests',
         'bokeh',
         'plotly',
         'kaleido'
       ],
       entry_points = {
         'console_scripts': [
           'iprPy = iprPy.command_line:command_line'
         ]
       },
       include_package_data = True,
-      zip_safe = False)
+      zip_safe = False)
```


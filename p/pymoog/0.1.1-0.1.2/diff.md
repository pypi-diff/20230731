# Comparing `tmp/pymoog-0.1.1.tar.gz` & `tmp/pymoog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoog-0.1.1.tar", last modified: Tue Feb 21 15:02:08 2023, max compression
+gzip compressed data, was "pymoog-0.1.2.tar", last modified: Mon Jul 31 15:00:10 2023, max compression
```

## Comparing `pymoog-0.1.1.tar` & `pymoog-0.1.2.tar`

### file list

```diff
@@ -1,302 +1,302 @@
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.737274 pymoog-0.1.1/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1102 2022-11-24 11:38:18.000000 pymoog-0.1.1/LICENCE
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)       99 2022-12-30 20:51:51.000000 pymoog-0.1.1/MANIFEST.in
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1959 2023-02-21 15:02:08.737274 pymoog-0.1.1/PKG-INFO
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1360 2023-02-04 10:21:56.000000 pymoog-0.1.1/README.md
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.725274 pymoog-0.1.1/pymoog/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      238 2023-02-21 14:42:23.000000 pymoog-0.1.1/pymoog/__init__.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10201 2023-02-04 10:21:56.000000 pymoog-0.1.1/pymoog/abfind.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        0 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/binary.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12214 2023-02-04 10:21:56.000000 pymoog-0.1.1/pymoog/blends.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16618 2023-02-04 10:21:56.000000 pymoog-0.1.1/pymoog/cog.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    15267 2022-11-24 12:54:27.000000 pymoog-0.1.1/pymoog/contri_func.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1341 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/deprecated.py
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.725274 pymoog-0.1.1/pymoog/files/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1149 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/atoms.csv
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      180 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/dissociation_energy_list.csv
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   212671 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/grid_points_kurucz.csv
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.725274 pymoog-0.1.1/pymoog/files/moog_nosm/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2548 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/README.md
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.725274 pymoog-0.1.1/pymoog/files/moog_nosm/manual/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1185 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.aux
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2582 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.log
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    38624 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.pdf
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1983 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.synctex.gz
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      882 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.tex
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.729274 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5581 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abfind.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7453 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abpop.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7793 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abunplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2990 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Atmos.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   710511 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Barklem.dat
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   591918 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/BarklemUV.dat
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    41530 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Batom.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3706 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Begin.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5478 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binary.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     9917 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5378 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binplotprep.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      393 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Blankstring.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10280 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Blends.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12350 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Bmolec.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1468 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Boxit.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1399 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Calmod.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2117 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cdcalc.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     8495 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Chabund.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2796 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cog.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3477 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cogplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2473 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cogsyn.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4005 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Correl.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1268 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Crosscorr.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2303 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Curve.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      649 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Dampdat.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7071 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Damping.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      849 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Defcolor.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1103 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Discov.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2505 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Doflux.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1552 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Drawcurs.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      449 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Dummy.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13047 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Eqlib.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1057 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Equivs.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2118 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Estim.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6777 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ewfind.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2659 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ewweighted.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1208 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Factor.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2518 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Fakeline.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      846 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Findtic.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1479 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Finish.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2711 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Fluxplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3067 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gammabark.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1158 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getasci.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      588 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getcount.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      723 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getnum.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4246 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getsyns.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2534 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gridplo.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4280 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gridsyn.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3288 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Infile.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     9656 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Inlines.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    17083 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Inmodel.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2602 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Invert.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3223 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Jexpint.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      830 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Kappa.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3213 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Lineabund.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12439 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Lineinfo.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2648 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Linex.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4975 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Linlimit.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2274 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.macdesk
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2446 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.macdesksilent
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2266 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.maclap
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2438 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.maclapsilent
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2247 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2208 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh64
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2264 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh64silent
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2334 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rhsilent
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3821 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makeplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      310 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Minimax.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1517 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Mol.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2573 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Molquery.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3967 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moog.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3936 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moog_bak.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3832 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moogsilent.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3801 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moogsilent_bak.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1259 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Multimod.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      753 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Multistar.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      389 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Mydriver.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4079 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Nansi.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5734 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Nearly.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1149 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Number.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3673 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Obshead.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      463 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Obspars.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6520 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Oneline.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1079 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/OpacHelium.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10823 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/OpacHydrogen.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4626 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opaccouls.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4771 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacit.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    17268 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacmetals.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2710 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacscat.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    28257 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Params.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1134 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Partfn.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1319 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Partnew.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2444 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotit.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3490 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotremember.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      250 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotval.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1814 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltabun.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2032 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltcog.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1143 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltflux.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12304 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltspec.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      665 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pointcurs.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1170 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Prinfo.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3607 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pstuff.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      525 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Putasci.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      532 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Quants.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4960 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Readobs.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1656 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Rinteg.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16887 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Smooth.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10139 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Specplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3134 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Stats.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      885 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Sunder.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     8885 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synpop.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5905 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synspec.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4500 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synth.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6986 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Tablepop.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1784 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Taukap.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1829 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Total.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6132 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Trudamp.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1994 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ucalc.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6306 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Vargauss.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5664 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Vmacro.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3451 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Voigt.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1528 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Wavecalc.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5961 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Weedout.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      839 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Writenumber.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      472 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/install.sh
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.733274 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16384 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/.Params.f.swp
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        0 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/.smhist
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5581 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abfind.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7412 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abpop.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7696 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abunplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2990 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Atmos.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   710511 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Barklem.dat
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   591918 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/BarklemUV.dat
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    41648 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Batom.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3704 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Begin.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5478 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binary.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     9800 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5378 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binplotprep.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      393 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Blankstring.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10448 2023-01-27 21:34:56.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Blends.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13497 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Bmolec.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1468 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Boxit.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1399 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Calmod.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2117 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cdcalc.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     8495 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Chabund.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2796 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cog.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3446 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cogplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2473 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cogsyn.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4005 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Correl.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1268 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Crosscorr.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2303 2023-01-01 20:42:48.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Curve.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      649 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Dampdat.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7070 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Damping.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      849 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Defcolor.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1103 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Discov.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2505 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Doflux.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1526 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Drawcurs.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      449 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Dummy.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13219 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Eqlib.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1057 2022-11-24 11:54:55.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Equivs.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7379 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ewfind.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2659 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ewweighted.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1208 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Factor.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2518 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Fakeline.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      846 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Findtic.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1479 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Finish.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2686 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Fluxplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3026 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gammabark.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1158 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getasci.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      588 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getcount.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      723 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getnum.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4246 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getsyns.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2534 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gridplo.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4280 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gridsyn.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3288 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Infile.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     9656 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inlines.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    15736 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inmodel.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    19092 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inmodel.new
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2602 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Invert.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3223 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Jexpint.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      830 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Kappa.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3213 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Lineabund.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13337 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Lineinfo.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2648 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Linex.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4975 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Linlimit.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2093 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.macdesk
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2259 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.macdesksilent
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1897 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.maclap
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1943 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.maclapsilent
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2120 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2022 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh64
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2076 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh64silent
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2199 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rhsilent
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3802 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makeplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2026 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Mol.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2573 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Molquery.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3856 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moog.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3816 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moog_bak.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3845 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moogsilent.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3805 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moogsilent_bak.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1259 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Multimod.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      753 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Multistar.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      389 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Mydriver.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4079 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Nansi.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6303 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Nearly.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1149 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Number.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3673 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Obshead.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      463 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Obspars.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6520 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Oneline.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1079 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/OpacHelium.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10845 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/OpacHydrogen.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4626 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opaccouls.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4771 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacit.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    17268 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacmetals.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2710 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacscat.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    28257 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Params.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1134 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Partfn.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1319 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Partnew.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2444 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotit.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3490 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotremember.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      250 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotval.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1817 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltabun.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2036 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltcog.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1146 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltflux.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12310 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltspec.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      655 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pointcurs.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1170 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Prinfo.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3607 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pstuff.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      525 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Putasci.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      532 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Quants.com
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4960 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Readobs.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1656 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Rinteg.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2691 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Setmols.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16889 2022-11-24 11:54:55.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Smooth.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10139 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Specplot.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3134 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Stats.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      777 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Sunder.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     8885 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synpop.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5905 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synspec.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4459 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synth.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6704 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Tablepop.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1784 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Taukap.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1829 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Total.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6133 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Trudamp.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1994 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ucalc.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6306 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Vargauss.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5664 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Vmacro.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3451 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Voigt.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1528 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Wavecalc.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5961 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Weedout.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      839 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Writenumber.f
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      887 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/install.sh
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.737274 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      235 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/PKG-INFO
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        0 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/SOURCES.txt
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        1 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/dependency_links.txt
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        1 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/not-zip-safe
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        8 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/top_level.txt
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16715 2022-12-30 22:35:46.000000 pymoog-0.1.1/pymoog/internal.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12803 2023-02-04 10:21:56.000000 pymoog-0.1.1/pymoog/line_data.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    33609 2023-02-04 10:21:56.000000 pymoog-0.1.1/pymoog/model.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    23965 2023-02-04 10:21:56.000000 pymoog-0.1.1/pymoog/mpfit.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      459 2023-02-21 14:58:12.000000 pymoog-0.1.1/pymoog/private.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2239 2023-02-21 14:59:03.000000 pymoog-0.1.1/pymoog/rundir_num.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16733 2023-02-04 10:21:56.000000 pymoog-0.1.1/pymoog/synth.py
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13092 2023-02-04 10:21:56.000000 pymoog-0.1.1/pymoog/weedout.py
-drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-02-21 15:02:08.725274 pymoog-0.1.1/pymoog.egg-info/
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1959 2023-02-21 15:02:08.000000 pymoog-0.1.1/pymoog.egg-info/PKG-INFO
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    14255 2023-02-21 15:02:08.000000 pymoog-0.1.1/pymoog.egg-info/SOURCES.txt
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        1 2023-02-21 15:02:08.000000 pymoog-0.1.1/pymoog.egg-info/dependency_links.txt
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        1 2022-11-24 11:38:18.000000 pymoog-0.1.1/pymoog.egg-info/not-zip-safe
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      114 2023-02-21 15:02:08.000000 pymoog-0.1.1/pymoog.egg-info/requires.txt
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        7 2023-02-21 15:02:08.000000 pymoog-0.1.1/pymoog.egg-info/top_level.txt
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)       38 2023-02-21 15:02:08.737274 pymoog-0.1.1/setup.cfg
--rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5732 2023-02-21 14:57:28.000000 pymoog-0.1.1/setup.py
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:10.001978 pymoog-0.1.2/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1069 2023-07-31 14:57:20.000000 pymoog-0.1.2/LICENCE
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)       99 2022-12-30 20:51:51.000000 pymoog-0.1.2/MANIFEST.in
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1959 2023-07-31 15:00:10.001978 pymoog-0.1.2/PKG-INFO
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1360 2023-02-04 10:21:56.000000 pymoog-0.1.2/README.md
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:09.989978 pymoog-0.1.2/pymoog/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      238 2023-07-31 14:56:59.000000 pymoog-0.1.2/pymoog/__init__.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10201 2023-02-04 10:21:56.000000 pymoog-0.1.2/pymoog/abfind.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        0 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/binary.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12214 2023-02-04 10:21:56.000000 pymoog-0.1.2/pymoog/blends.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16618 2023-02-04 10:21:56.000000 pymoog-0.1.2/pymoog/cog.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    15267 2022-11-24 12:54:27.000000 pymoog-0.1.2/pymoog/contri_func.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1341 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/deprecated.py
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:09.989978 pymoog-0.1.2/pymoog/files/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1149 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/atoms.csv
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      180 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/dissociation_energy_list.csv
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   212671 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/grid_points_kurucz.csv
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:09.989978 pymoog-0.1.2/pymoog/files/moog_nosm/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2548 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/README.md
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:09.989978 pymoog-0.1.2/pymoog/files/moog_nosm/manual/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1185 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.aux
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2582 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.log
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    38624 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.pdf
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1983 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.synctex.gz
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      882 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.tex
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:09.993978 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5581 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abfind.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7453 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abpop.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7793 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abunplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2990 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Atmos.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   710511 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Barklem.dat
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   591918 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/BarklemUV.dat
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    41530 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Batom.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3706 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Begin.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5478 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binary.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     9917 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5378 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binplotprep.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      393 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Blankstring.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10280 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Blends.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12350 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Bmolec.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1468 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Boxit.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1399 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Calmod.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2117 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cdcalc.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     8495 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Chabund.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2796 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cog.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3477 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cogplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2473 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cogsyn.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4005 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Correl.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1268 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Crosscorr.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2303 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Curve.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      649 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Dampdat.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7071 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Damping.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      849 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Defcolor.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1103 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Discov.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2505 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Doflux.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1552 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Drawcurs.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      449 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Dummy.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13047 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Eqlib.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1057 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Equivs.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2118 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Estim.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6777 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ewfind.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2659 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ewweighted.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1208 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Factor.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2518 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Fakeline.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      846 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Findtic.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1479 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Finish.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2711 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Fluxplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3067 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gammabark.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1158 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getasci.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      588 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getcount.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      723 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getnum.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4246 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getsyns.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2534 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gridplo.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4280 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gridsyn.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3288 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Infile.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     9656 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Inlines.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    17083 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Inmodel.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2602 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Invert.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3223 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Jexpint.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      830 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Kappa.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3213 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Lineabund.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12439 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Lineinfo.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2648 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Linex.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4975 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Linlimit.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2274 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.macdesk
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2446 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.macdesksilent
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2266 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.maclap
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2438 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.maclapsilent
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2247 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2208 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh64
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2264 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh64silent
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2334 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rhsilent
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3821 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makeplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      310 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Minimax.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1517 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Mol.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2573 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Molquery.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3967 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moog.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3936 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moog_bak.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3832 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moogsilent.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3801 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moogsilent_bak.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1259 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Multimod.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      753 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Multistar.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      389 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Mydriver.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4079 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Nansi.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5734 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Nearly.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1149 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Number.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3673 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Obshead.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      463 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Obspars.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6520 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Oneline.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1079 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/OpacHelium.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10823 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/OpacHydrogen.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4626 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opaccouls.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4771 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacit.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    17268 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacmetals.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2710 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacscat.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    28257 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Params.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1134 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Partfn.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1319 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Partnew.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2444 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotit.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3490 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotremember.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      250 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotval.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1814 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltabun.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2032 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltcog.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1143 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltflux.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12304 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltspec.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      665 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pointcurs.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1170 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Prinfo.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3607 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pstuff.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      525 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Putasci.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      532 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Quants.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4960 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Readobs.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1656 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Rinteg.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16887 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Smooth.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10139 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Specplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3134 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Stats.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      885 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Sunder.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     8885 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synpop.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5905 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synspec.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4500 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synth.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6986 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Tablepop.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1784 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Taukap.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1829 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Total.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6132 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Trudamp.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1994 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ucalc.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6306 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Vargauss.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5664 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Vmacro.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3451 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Voigt.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1528 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Wavecalc.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5961 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Weedout.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      839 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Writenumber.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      472 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/install.sh
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:10.001978 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16384 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/.Params.f.swp
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        0 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/.smhist
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5581 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abfind.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7412 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abpop.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7696 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abunplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2990 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Atmos.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   710511 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Barklem.dat
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)   591918 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/BarklemUV.dat
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    41648 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Batom.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3704 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Begin.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5478 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binary.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     9800 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5378 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binplotprep.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      393 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Blankstring.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10448 2023-01-27 21:34:56.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Blends.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13497 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Bmolec.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1468 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Boxit.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1399 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Calmod.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2117 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cdcalc.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     8495 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Chabund.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2796 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cog.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3446 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cogplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2473 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cogsyn.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4005 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Correl.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1268 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Crosscorr.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2303 2023-01-01 20:42:48.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Curve.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      649 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Dampdat.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7070 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Damping.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      849 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Defcolor.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1103 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Discov.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2505 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Doflux.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1526 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Drawcurs.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      449 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Dummy.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13219 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Eqlib.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1057 2022-11-24 11:54:55.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Equivs.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     7379 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ewfind.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2659 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ewweighted.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1208 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Factor.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2518 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Fakeline.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      846 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Findtic.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1479 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Finish.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2686 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Fluxplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3026 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gammabark.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1158 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getasci.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      588 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getcount.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      723 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getnum.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4246 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getsyns.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2534 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gridplo.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4280 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gridsyn.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3288 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Infile.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     9656 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inlines.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    15736 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inmodel.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    19092 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inmodel.new
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2602 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Invert.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3223 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Jexpint.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      830 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Kappa.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3213 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Lineabund.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13337 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Lineinfo.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2648 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Linex.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4975 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Linlimit.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2093 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.macdesk
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2259 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.macdesksilent
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1897 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.maclap
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1943 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.maclapsilent
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2120 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2022 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh64
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2076 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh64silent
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2199 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rhsilent
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3802 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makeplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2026 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Mol.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2573 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Molquery.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3856 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moog.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3816 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moog_bak.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3845 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moogsilent.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3805 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moogsilent_bak.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1259 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Multimod.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      753 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Multistar.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      389 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Mydriver.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4079 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Nansi.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6303 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Nearly.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1149 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Number.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3673 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Obshead.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      463 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Obspars.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6520 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Oneline.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1079 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/OpacHelium.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10845 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/OpacHydrogen.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4626 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opaccouls.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4771 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacit.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    17268 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacmetals.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2710 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacscat.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    28257 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Params.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1134 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Partfn.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1319 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Partnew.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2444 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotit.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3490 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotremember.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      250 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotval.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1817 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltabun.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2036 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltcog.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1146 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltflux.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    12310 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltspec.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      655 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pointcurs.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1170 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Prinfo.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3607 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pstuff.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      525 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Putasci.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      532 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Quants.com
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4960 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Readobs.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1656 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Rinteg.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2691 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Setmols.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16889 2022-11-24 11:54:55.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Smooth.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    10139 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Specplot.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3134 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Stats.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      777 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Sunder.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     8885 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synpop.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5905 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synspec.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     4459 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synth.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6704 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Tablepop.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1784 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Taukap.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1829 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Total.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6133 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Trudamp.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1994 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ucalc.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     6306 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Vargauss.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5664 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Vmacro.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     3451 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Voigt.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1528 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Wavecalc.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5961 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Weedout.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      839 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Writenumber.f
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      887 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/install.sh
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:10.001978 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      235 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/PKG-INFO
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        0 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        1 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        1 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/not-zip-safe
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        8 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/rulerwd.egg-info/top_level.txt
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16715 2022-12-30 22:35:46.000000 pymoog-0.1.2/pymoog/internal.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16567 2023-07-31 14:56:45.000000 pymoog-0.1.2/pymoog/line_data.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    33609 2023-02-04 10:21:56.000000 pymoog-0.1.2/pymoog/model.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    23965 2023-02-04 10:21:56.000000 pymoog-0.1.2/pymoog/mpfit.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      459 2023-02-21 14:58:12.000000 pymoog-0.1.2/pymoog/private.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     2239 2023-02-21 14:59:03.000000 pymoog-0.1.2/pymoog/rundir_num.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    16733 2023-02-04 10:21:56.000000 pymoog-0.1.2/pymoog/synth.py
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    13092 2023-02-04 10:21:56.000000 pymoog-0.1.2/pymoog/weedout.py
+drwxrwxr-x   0 mingjie   (1000) mingjie   (1000)        0 2023-07-31 15:00:09.989978 pymoog-0.1.2/pymoog.egg-info/
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     1959 2023-07-31 15:00:09.000000 pymoog-0.1.2/pymoog.egg-info/PKG-INFO
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)    14255 2023-07-31 15:00:09.000000 pymoog-0.1.2/pymoog.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        1 2023-07-31 15:00:09.000000 pymoog-0.1.2/pymoog.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        1 2022-11-24 11:38:18.000000 pymoog-0.1.2/pymoog.egg-info/not-zip-safe
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)      114 2023-07-31 15:00:09.000000 pymoog-0.1.2/pymoog.egg-info/requires.txt
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)        7 2023-07-31 15:00:09.000000 pymoog-0.1.2/pymoog.egg-info/top_level.txt
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)       38 2023-07-31 15:00:10.001978 pymoog-0.1.2/setup.cfg
+-rw-rw-r--   0 mingjie   (1000) mingjie   (1000)     5927 2023-07-31 14:57:45.000000 pymoog-0.1.2/setup.py
```

### Comparing `pymoog-0.1.1/LICENCE` & `pymoog-0.1.2/LICENCE`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020, Mingjie Jian, Pranav Satheesh, Kruthi Krishna
+Copyright (c) 2023, Mingjie Jian
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymoog-0.1.1/PKG-INFO` & `pymoog-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymoog
-Version: 0.1.1
+Version: 0.1.2
 Summary: The python wrapper to run LTE spectra synthesis code MOOG.
 Home-page: https://github.com/MingjieJian/pymoog
 Author: Mingjie Jian
 Author-email: ssaajianmingjie@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: IPython
```

### Comparing `pymoog-0.1.1/README.md` & `pymoog-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/abfind.py` & `pymoog-0.1.2/pymoog/abfind.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/blends.py` & `pymoog-0.1.2/pymoog/blends.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/cog.py` & `pymoog-0.1.2/pymoog/cog.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/contri_func.py` & `pymoog-0.1.2/pymoog/contri_func.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/deprecated.py` & `pymoog-0.1.2/pymoog/deprecated.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/atoms.csv` & `pymoog-0.1.2/pymoog/files/atoms.csv`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/grid_points_kurucz.csv` & `pymoog-0.1.2/pymoog/files/grid_points_kurucz.csv`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/README.md` & `pymoog-0.1.2/pymoog/files/moog_nosm/README.md`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.aux` & `pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.aux`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.log` & `pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.log`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.pdf` & `pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.pdf`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.synctex.gz` & `pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.synctex.gz`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/manual/MOOG Manual.tex` & `pymoog-0.1.2/pymoog/files/moog_nosm/manual/MOOG Manual.tex`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abfind.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abfind.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abpop.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abpop.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abunplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Abunplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Atmos.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Atmos.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Barklem.dat` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Barklem.dat`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/BarklemUV.dat` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/BarklemUV.dat`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Batom.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Batom.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Begin.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Begin.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binary.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binary.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binplotprep.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Binplotprep.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Blends.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Blends.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Bmolec.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Bmolec.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Boxit.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Boxit.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Calmod.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Calmod.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cdcalc.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cdcalc.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Chabund.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Chabund.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cog.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cog.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cogplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cogplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cogsyn.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Cogsyn.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Correl.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Correl.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Crosscorr.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Crosscorr.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Curve.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Curve.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Dampdat.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Dampdat.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Damping.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Damping.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Defcolor.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Defcolor.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Discov.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Discov.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Doflux.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Doflux.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Drawcurs.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Drawcurs.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Eqlib.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Eqlib.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Equivs.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Equivs.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Estim.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Estim.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ewfind.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ewfind.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ewweighted.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ewweighted.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Factor.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Factor.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Fakeline.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Fakeline.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Findtic.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Findtic.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Finish.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Finish.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Fluxplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Fluxplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gammabark.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gammabark.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getasci.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getasci.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getcount.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getcount.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getnum.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getnum.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getsyns.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Getsyns.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gridplo.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gridplo.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gridsyn.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Gridsyn.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Infile.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Infile.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Inlines.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Inlines.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Inmodel.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Inmodel.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Invert.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Invert.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Jexpint.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Jexpint.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Kappa.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Kappa.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Lineabund.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Lineabund.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Lineinfo.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Lineinfo.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Linex.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Linex.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Linlimit.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Linlimit.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.macdesk` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.macdesk`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.macdesksilent` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.macdesksilent`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.maclap` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.maclap`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.maclapsilent` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.maclapsilent`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh64` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh64`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh64silent` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rh64silent`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rhsilent` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makefile.rhsilent`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makeplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Makeplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Mol.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Mol.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Molquery.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Molquery.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moog.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moog.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moog_bak.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moog_bak.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moogsilent.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moogsilent.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moogsilent_bak.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Moogsilent_bak.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Multimod.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Multimod.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Multistar.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Multistar.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Nansi.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Nansi.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Nearly.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Nearly.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Number.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Number.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Obshead.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Obshead.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Oneline.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Oneline.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/OpacHelium.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/OpacHelium.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/OpacHydrogen.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/OpacHydrogen.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opaccouls.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opaccouls.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacit.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacit.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacmetals.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacmetals.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacscat.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Opacscat.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Params.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Params.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Partfn.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Partfn.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Partnew.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Partnew.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotit.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotit.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotremember.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Plotremember.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltabun.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltabun.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltcog.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltcog.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltflux.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltflux.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltspec.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pltspec.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pointcurs.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pointcurs.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Prinfo.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Prinfo.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pstuff.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Pstuff.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Putasci.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Putasci.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Quants.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Quants.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Readobs.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Readobs.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Rinteg.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Rinteg.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Smooth.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Smooth.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Specplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Specplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Stats.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Stats.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Sunder.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Sunder.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synpop.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synpop.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synspec.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synspec.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synth.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Synth.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Tablepop.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Tablepop.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Taukap.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Taukap.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Total.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Total.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Trudamp.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Trudamp.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ucalc.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Ucalc.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Vargauss.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Vargauss.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Vmacro.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Vmacro.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Voigt.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Voigt.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Wavecalc.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Wavecalc.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Weedout.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Weedout.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_FEB2017/Writenumber.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_FEB2017/Writenumber.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/.Params.f.swp` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/.Params.f.swp`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abfind.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abfind.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abpop.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abpop.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abunplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Abunplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Atmos.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Atmos.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Barklem.dat` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Barklem.dat`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/BarklemUV.dat` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/BarklemUV.dat`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Batom.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Batom.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Begin.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Begin.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binary.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binary.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binplotprep.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Binplotprep.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Blends.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Blends.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Bmolec.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Bmolec.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Boxit.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Boxit.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Calmod.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Calmod.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cdcalc.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cdcalc.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Chabund.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Chabund.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cog.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cog.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cogplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cogplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cogsyn.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Cogsyn.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Correl.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Correl.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Crosscorr.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Crosscorr.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Curve.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Curve.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Dampdat.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Dampdat.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Damping.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Damping.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Defcolor.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Defcolor.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Discov.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Discov.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Doflux.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Doflux.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Drawcurs.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Drawcurs.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Eqlib.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Eqlib.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Equivs.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Equivs.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ewfind.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ewfind.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ewweighted.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ewweighted.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Factor.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Factor.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Fakeline.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Fakeline.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Findtic.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Findtic.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Finish.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Finish.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Fluxplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Fluxplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gammabark.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gammabark.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getasci.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getasci.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getcount.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getcount.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getnum.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getnum.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getsyns.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Getsyns.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gridplo.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gridplo.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gridsyn.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Gridsyn.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Infile.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Infile.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inlines.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inlines.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inmodel.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inmodel.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inmodel.new` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Inmodel.new`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Invert.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Invert.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Jexpint.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Jexpint.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Kappa.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Kappa.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Lineabund.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Lineabund.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Lineinfo.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Lineinfo.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Linex.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Linex.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Linlimit.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Linlimit.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.macdesk` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.macdesk`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.macdesksilent` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.macdesksilent`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.maclap` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.maclap`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.maclapsilent` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.maclapsilent`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh64` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh64`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh64silent` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rh64silent`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rhsilent` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makefile.rhsilent`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makeplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Makeplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Mol.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Mol.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Molquery.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Molquery.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moog.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moog.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moog_bak.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moog_bak.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moogsilent.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moogsilent.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moogsilent_bak.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Moogsilent_bak.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Multimod.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Multimod.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Multistar.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Multistar.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Nansi.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Nansi.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Nearly.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Nearly.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Number.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Number.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Obshead.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Obshead.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Oneline.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Oneline.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/OpacHelium.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/OpacHelium.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/OpacHydrogen.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/OpacHydrogen.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opaccouls.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opaccouls.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacit.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacit.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacmetals.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacmetals.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacscat.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Opacscat.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Params.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Params.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Partfn.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Partfn.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Partnew.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Partnew.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotit.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotit.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotremember.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Plotremember.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltabun.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltabun.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltcog.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltcog.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltflux.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltflux.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltspec.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pltspec.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pointcurs.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pointcurs.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Prinfo.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Prinfo.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pstuff.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Pstuff.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Putasci.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Putasci.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Quants.com` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Quants.com`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Readobs.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Readobs.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Rinteg.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Rinteg.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Setmols.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Setmols.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Smooth.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Smooth.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Specplot.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Specplot.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Stats.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Stats.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Sunder.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Sunder.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synpop.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synpop.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synspec.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synspec.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synth.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Synth.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Tablepop.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Tablepop.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Taukap.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Taukap.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Total.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Total.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Trudamp.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Trudamp.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ucalc.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Ucalc.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Vargauss.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Vargauss.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Vmacro.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Vmacro.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Voigt.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Voigt.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Wavecalc.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Wavecalc.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Weedout.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Weedout.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/Writenumber.f` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/Writenumber.f`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/files/moog_nosm/moog_nosm_NOV2019/install.sh` & `pymoog-0.1.2/pymoog/files/moog_nosm/moog_nosm_NOV2019/install.sh`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/internal.py` & `pymoog-0.1.2/pymoog/internal.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/line_data.py` & `pymoog-0.1.2/pymoog/line_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -262,8 +262,96 @@
         # No line is found
         dominant_line = pd.DataFrame(np.array([np.nan]*8)).T
         dominant_line.columns = ['wavelength', 'id', 'EP', 'loggf', 'C6', 'D0', 'EW', 'r_blend_depth']
 
     if include_strong_linelist:
         return dominant_line, linelist_keep
     else:
-        return dominant_line
+        return dominant_line
+
+def cal_d_blending_ratio(teff, logg, m_h, start_wav, end_wav, resolution, linelist_all='vald_3000_24000', weedout_switch=0.01,  abun_change=None):
+    '''
+    Calculate the depth blending ratio of the lines in the line list.
+    The depth blending ratio is defined as d(other lines) / d(other lines + target line).  
+
+    Parameters
+    ----------
+    teff : float
+        The effective temperature of the model
+    logg : float
+        logg value of the model
+    m_h : float
+        [M/H] value (overall metallicity) of the model
+    start_wav : float
+        The start wavelength of the line list
+    end_wav : float
+        The end wavelength of the line list
+    resolution : float
+        Resolution of the synthetic spectra; this will passed to MOOG and convolute with initial spectra.
+    line_list : str or pd.DataFrame, default vald_3000_24000 
+        The name of the linelist file.
+    weedout_switch : bool or float, default 0.01
+        The switch for running weedout driver before synth. If False then weedout is not run; if True the weedout is run with kappa_ratio=0.01, and if a float (> 0 and < 1) is given then weedout is run with the kappa_ratio set as the number.
+    abun_change : dict of pairs {int:float, ...}
+            Abundance change, have to be a dict of pairs of atomic number and [X/Fe] values.
+
+    Returns
+    ----------
+    linelist_all : pandas.DataFrame, optional
+        The line list with blending ratio stored in d_blend_ratio.
+    '''
+
+    # Establish the linelist
+    if isinstance(linelist_all, str):
+        linelist_all = read_linelist(linelist_all)
+    elif isinstance(linelist_all, private.pd.DataFrame):
+        pass
+    else:
+        raise TypeError('Type of input linelist have to be either str or pandas.DataFrame.')
+    
+    linelist_all = linelist_all[(linelist_all['wavelength'] >= start_wav) & (linelist_all['wavelength'] <= end_wav)]
+
+    # Calculate the blending ratio
+    s = synth.synth(teff, logg, m_h, start_wav, end_wav, resolution, line_list=linelist_all)
+    s.prepare_file(abun_change=abun_change)
+    # Whole spectra 
+    s.run_moog()
+    s.read_spectra()
+    wav_all, flux_all = s.wav, s.flux
+
+    # weedout lines
+    if weedout_switch != False:
+        w = weedout.weedout(teff, logg, m_h, start_wav, end_wav, line_list=linelist_all, kappa_ratio=weedout_switch)
+        w.prepare_file()
+        w.run_moog()
+
+    # Target line exclude
+    if weedout_switch:
+        w.read_linelist()
+        linelist_keep = w.keep_list
+        line_index_keep = find_lines(linelist_keep, linelist_all)
+    else:
+        line_index_keep = linelist_all.index
+
+    d_blend_ratio_list = []
+    for line_index in linelist_all.index:
+        
+        if line_index in line_index_keep:
+            target_wav = linelist_all.loc[line_index, 'wavelength']
+            linelist_exclude = linelist_all.drop(line_index).reset_index(drop=True)
+            s = synth.synth(teff, logg, m_h, target_wav-1, target_wav+1, resolution, line_list=linelist_exclude)
+            s.prepare_file(abun_change=abun_change)
+            s.run_moog()
+            s.read_spectra(remove=False)
+            wav_exclude, flux_exclude = s.wav, s.flux
+            
+            # Calculate the blending fraction
+            r_blend_ratio = (1-flux_exclude[np.argmin(np.abs(wav_exclude-target_wav))]) / (1-flux_all[np.argmin(np.abs(wav_all-target_wav))])
+            if r_blend_ratio > 1 and np.abs((1-flux_exclude[np.argmin(np.abs(wav_exclude-target_wav))])-(1-flux_all[np.argmin(np.abs(wav_all-target_wav))])) < 0.001:
+                r_blend_ratio = 1
+            d_blend_ratio_list.append(r_blend_ratio)
+        else:
+            d_blend_ratio_list.append(np.nan)
+
+    linelist_all['d_blend_ratio'] = d_blend_ratio_list
+
+    return linelist_all
```

### Comparing `pymoog-0.1.1/pymoog/model.py` & `pymoog-0.1.2/pymoog/model.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/mpfit.py` & `pymoog-0.1.2/pymoog/mpfit.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/rundir_num.py` & `pymoog-0.1.2/pymoog/rundir_num.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/synth.py` & `pymoog-0.1.2/pymoog/synth.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog/weedout.py` & `pymoog-0.1.2/pymoog/weedout.py`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/pymoog.egg-info/PKG-INFO` & `pymoog-0.1.2/pymoog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymoog
-Version: 0.1.1
+Version: 0.1.2
 Summary: The python wrapper to run LTE spectra synthesis code MOOG.
 Home-page: https://github.com/MingjieJian/pymoog
 Author: Mingjie Jian
 Author-email: ssaajianmingjie@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: IPython
```

### Comparing `pymoog-0.1.1/pymoog.egg-info/SOURCES.txt` & `pymoog-0.1.2/pymoog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymoog-0.1.1/setup.py` & `pymoog-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 import subprocess
 import os
 import setuptools
+import atexit
 
-if os.environ.get('READTHEDOCS') != 'True':
-    # Define MOOGMODELING_path. This path will store the code of moog and any other temporary files in the calculation.
-    MOOGMODELING_path = '{}/.pymoog/'.format(os.environ['HOME'])
-
-    # Create the folder according to MOOGMODELING_path
-    if not(os.path.isdir(MOOGMODELING_path)):
-        os.mkdir(MOOGMODELING_path)
-        
-    # Copy the files folder into working directory
-    if not(os.path.isdir(MOOGMODELING_path + 'files')):
-        os.mkdir(MOOGMODELING_path + 'files')
-    cp_status = subprocess.run(['cp', '-r', 'pymoog/files', MOOGMODELING_path], stdout=subprocess.PIPE)
+def download_lfs_at_exit():
 
-    # Download large files from Zenodo 
+    # Download large files from Zenodo. This need to be done at exti, after zenodo_get is installed. 
     zenodo_status = subprocess.run(['zenodo_get', '10.5281/zenodo.7495246', '-o', os.path.expanduser('~') + '/.pymoog/files/'])
     # Find the latest version of pymoog_lf
     version_list = [i for i in os.listdir(os.path.expanduser('~') + '/.pymoog/files/') if '.tar.gz' in i]
     remove_list = [i for i in version_list if i[-7:] != '.tar.gz']
     version_list = [i for i in version_list if i[-7:] == '.tar.gz']
     version_split_list = [i.split('_')[2].split('.')[0:3] for i in version_list]
 
@@ -32,14 +22,29 @@
     latest_version = 'pymoog_lf_v{}.{}.{}.tar.gz'.format(*version_list_temp[0])
     # Clear old lf versions
     for version in remove_list:
         rm_status = subprocess.run(['rm', MOOGMODELING_path + '/files/' + version], stdout=subprocess.PIPE)
     # unzip latest version
     tar_status = subprocess.run(['tar', '-xzvf', MOOGMODELING_path + 'files/' + latest_version, '-C', MOOGMODELING_path + 'files/'], stdout=subprocess.PIPE)
 
+    print("Large files download/renew finished.")
+
+if os.environ.get('READTHEDOCS') != 'True':
+    # Define MOOGMODELING_path. This path will store the code of moog and any other temporary files in the calculation.
+    MOOGMODELING_path = '{}/.pymoog/'.format(os.environ['HOME'])
+
+    # Create the folder according to MOOGMODELING_path
+    if not(os.path.isdir(MOOGMODELING_path)):
+        os.mkdir(MOOGMODELING_path)
+        
+    # Copy the files folder into working directory
+    if not(os.path.isdir(MOOGMODELING_path + 'files')):
+        os.mkdir(MOOGMODELING_path + 'files')
+    cp_status = subprocess.run(['cp', '-r', 'pymoog/files', MOOGMODELING_path], stdout=subprocess.PIPE)
+
     # Copy the moog_nosm folder to MOOGMODELING_path; if the folder already exist it will be removed first.
     if os.path.isdir(MOOGMODELING_path + '/moog_nosm'):
         rm_status = subprocess.run(['rm', '-r', MOOGMODELING_path + 'moog_nosm'], stdout=subprocess.PIPE)
     mv_status = subprocess.run(['mv', MOOGMODELING_path + 'files/moog_nosm', MOOGMODELING_path + 'moog_nosm'], stdout=subprocess.PIPE)
 
     # Check the permission of ./install
     chmod_subp = subprocess.run(['chmod', '775', './install.sh'], cwd=MOOGMODELING_path+'moog_nosm/moog_nosm_NOV2019/', stdout=subprocess.PIPE)
@@ -53,21 +58,23 @@
 
     # Check if MOOG and MOOGSILENT is in the folder
     if not(os.path.isfile(MOOGMODELING_path+'moog_nosm/moog_nosm_NOV2019/MOOG')) or not(os.path.isfile(MOOGMODELING_path+'moog_nosm/moog_nosm_NOV2019/MOOGSILENT')):
         raise ValueError("MOOG is not installed correctly!")
     else:
         print('Successfully installed MOOG!')
     
+atexit.register(download_lfs_at_exit)
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 if os.environ.get('READTHEDOCS') != 'True':
     setuptools.setup(
         name='pymoog',
-        version='0.1.1',
+        version='0.1.2',
         description='The python wrapper to run LTE spectra synthesis code MOOG.',
         long_description=long_description,
         long_description_content_type="text/markdown",
         url='https://github.com/MingjieJian/pymoog',
         author='Mingjie Jian',
         author_email='ssaajianmingjie@gmail.com',
         classifiers=[
```


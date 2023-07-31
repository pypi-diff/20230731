# Comparing `tmp/phasepy-0.0.8.tar.gz` & `tmp/phasepy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\phasepy-0.0.8.tar", last modified: Thu Mar 21 17:47:22 2019, max compression
+gzip compressed data, was "dist\phasepy-0.0.9.tar", last modified: Tue Apr 16 02:36:06 2019, max compression
```

## Comparing `phasepy-0.0.8.tar` & `phasepy-0.0.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:22.000000 phasepy-0.0.8/
--rw-rw-rw-   0        0        0     1101 2019-02-19 13:16:58.000000 phasepy-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      185 2019-03-02 21:11:36.000000 phasepy-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1309 2019-03-21 17:47:22.000000 phasepy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3003 2019-03-02 21:09:19.000000 phasepy-0.0.8/README.rst
--rw-rw-rw-   0        0        0      735 2019-03-02 21:09:26.000000 phasepy-0.0.8/long_description.rst
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:21.000000 phasepy-0.0.8/phasepy/
--rw-rw-rw-   0        0        0     1345 2019-03-02 20:33:15.000000 phasepy-0.0.8/phasepy/__init__.py
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:21.000000 phasepy-0.0.8/phasepy/actmodels/
--rw-rw-rw-   0        0        0      277 2019-03-02 20:39:17.000000 phasepy-0.0.8/phasepy/actmodels/__init__.py
--rw-rw-rw-   0        0        0     1583 2019-03-14 19:09:31.000000 phasepy-0.0.8/phasepy/actmodels/nrtl.py
--rw-rw-rw-   0        0        0     1565 2019-03-02 20:39:26.000000 phasepy-0.0.8/phasepy/actmodels/redlichkister.py
--rw-rw-rw-   0        0        0     1720 2019-03-02 20:39:31.000000 phasepy-0.0.8/phasepy/actmodels/unifac.py
--rw-rw-rw-   0        0        0     3988 2019-03-02 20:39:37.000000 phasepy-0.0.8/phasepy/actmodels/virial.py
--rw-rw-rw-   0        0        0     2195 2019-03-02 20:39:42.000000 phasepy-0.0.8/phasepy/actmodels/virialgama.py
--rw-rw-rw-   0        0        0      736 2019-03-02 20:39:51.000000 phasepy-0.0.8/phasepy/actmodels/wilson.py
--rw-rw-rw-   0        0        0      302 2019-03-02 20:33:24.000000 phasepy-0.0.8/phasepy/constants.py
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:21.000000 phasepy-0.0.8/phasepy/cubic/
--rw-rw-rw-   0        0        0      690 2019-03-02 20:36:36.000000 phasepy-0.0.8/phasepy/cubic/__init__.py
--rw-rw-rw-   0        0        0      502 2019-03-02 20:36:44.000000 phasepy-0.0.8/phasepy/cubic/alphas.py
--rw-rw-rw-   0        0        0     3445 2019-03-02 20:34:28.000000 phasepy-0.0.8/phasepy/cubic/cubic.py
--rw-rw-rw-   0        0        0    19720 2019-03-21 17:43:53.000000 phasepy-0.0.8/phasepy/cubic/cubicmix.py
--rw-rw-rw-   0        0        0    11058 2019-03-02 20:37:00.000000 phasepy-0.0.8/phasepy/cubic/cubicpure.py
--rw-rw-rw-   0        0        0     6487 2019-03-05 17:56:32.000000 phasepy-0.0.8/phasepy/cubic/mhv.py
--rw-rw-rw-   0        0        0     1890 2019-03-02 20:39:06.000000 phasepy-0.0.8/phasepy/cubic/psatpure.py
--rw-rw-rw-   0        0        0      943 2019-03-05 17:54:32.000000 phasepy-0.0.8/phasepy/cubic/qmr.py
--rw-rw-rw-   0        0        0    12066 2019-03-19 17:22:04.000000 phasepy-0.0.8/phasepy/cubic/vdwmix.py
--rw-rw-rw-   0        0        0     8821 2019-03-02 20:37:35.000000 phasepy-0.0.8/phasepy/cubic/vdwpure.py
--rw-rw-rw-   0        0        0     1897 2019-03-05 19:21:53.000000 phasepy-0.0.8/phasepy/cubic/wongsandler.py
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:21.000000 phasepy-0.0.8/phasepy/database/
--rw-rw-rw-   0        0        0    50941 2018-09-04 12:45:47.000000 phasepy-0.0.8/phasepy/database/dortmund.xlsx
--rw-rw-rw-   0        0        0    17186 2018-09-02 20:22:25.000000 phasepy-0.0.8/phasepy/database/unifac.xlsx
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:21.000000 phasepy-0.0.8/phasepy/equilibrium/
--rw-rw-rw-   0        0        0     1913 2019-03-21 16:47:35.000000 phasepy-0.0.8/phasepy/equilibrium/__init__.py
--rw-rw-rw-   0        0        0     6759 2019-03-02 20:35:14.000000 phasepy-0.0.8/phasepy/equilibrium/bubble.py
--rw-rw-rw-   0        0        0     6759 2019-03-02 20:35:19.000000 phasepy-0.0.8/phasepy/equilibrium/dew.py
--rw-rw-rw-   0        0        0     2146 2019-03-02 20:35:25.000000 phasepy-0.0.8/phasepy/equilibrium/ell.py
--rw-rw-rw-   0        0        0      616 2019-03-02 20:35:31.000000 phasepy-0.0.8/phasepy/equilibrium/equilibriumresult.py
--rw-rw-rw-   0        0        0     4498 2019-03-02 20:35:35.000000 phasepy-0.0.8/phasepy/equilibrium/flash.py
--rw-rw-rw-   0        0        0     2780 2019-03-02 20:35:45.000000 phasepy-0.0.8/phasepy/equilibrium/hazb.py
--rw-rw-rw-   0        0        0     5397 2019-03-02 20:35:50.000000 phasepy-0.0.8/phasepy/equilibrium/hazt.py
--rw-rw-rw-   0        0        0     5641 2019-03-02 20:35:55.000000 phasepy-0.0.8/phasepy/equilibrium/multiflash.py
--rw-rw-rw-   0        0        0     7124 2019-03-02 20:35:59.000000 phasepy-0.0.8/phasepy/equilibrium/stability.py
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:21.000000 phasepy-0.0.8/phasepy/fit/
--rw-rw-rw-   0        0        0      261 2019-03-02 20:33:55.000000 phasepy-0.0.8/phasepy/fit/__init__.py
--rw-rw-rw-   0        0        0     5998 2019-03-02 20:34:02.000000 phasepy-0.0.8/phasepy/fit/binaryfit.py
--rw-rw-rw-   0        0        0      990 2019-03-02 20:34:09.000000 phasepy-0.0.8/phasepy/fit/fitcii.py
--rw-rw-rw-   0        0        0     3578 2019-03-10 13:05:21.000000 phasepy-0.0.8/phasepy/fit/fitmulticomponent.py
--rw-rw-rw-   0        0        0     1516 2019-03-02 20:34:35.000000 phasepy-0.0.8/phasepy/fit/fitpsat.py
--rw-rw-rw-   0        0        0     2838 2019-03-02 20:34:46.000000 phasepy-0.0.8/phasepy/fit/ternaryfit.py
--rw-rw-rw-   0        0        0      958 2019-03-02 20:33:32.000000 phasepy-0.0.8/phasepy/math.py
--rw-rw-rw-   0        0        0    15659 2019-03-05 19:04:23.000000 phasepy-0.0.8/phasepy/mixtures.py
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:22.000000 phasepy-0.0.8/phasepy/sgt/
--rw-rw-rw-   0        0        0      348 2019-03-02 20:32:25.000000 phasepy-0.0.8/phasepy/sgt/__init__.py
--rw-rw-rw-   0        0        0     3970 2019-03-20 17:52:04.000000 phasepy-0.0.8/phasepy/sgt/coloc_z.py
--rw-rw-rw-   0        0        0     4743 2019-03-02 20:32:16.000000 phasepy-0.0.8/phasepy/sgt/linear_spot.py
--rw-rw-rw-   0        0        0     3610 2019-03-02 20:32:10.000000 phasepy-0.0.8/phasepy/sgt/path_hk.py
--rw-rw-rw-   0        0        0     2387 2019-03-02 20:31:50.000000 phasepy-0.0.8/phasepy/sgt/path_sk.py
--rw-rw-rw-   0        0        0     2240 2019-03-02 20:31:26.000000 phasepy-0.0.8/phasepy/sgt/reference_component.py
--rw-rw-rw-   0        0        0     1978 2019-03-02 20:31:16.000000 phasepy-0.0.8/phasepy/sgt/sgtpuros.py
--rw-rw-rw-   0        0        0      608 2019-03-02 20:31:34.000000 phasepy-0.0.8/phasepy/sgt/tensionresult.py
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:22.000000 phasepy-0.0.8/phasepy/src/
--rw-rw-rw-   0        0        0   845042 2019-02-20 14:44:57.000000 phasepy-0.0.8/phasepy/src/actmodels_cy.c
--rw-rw-rw-   0        0        0     4100 2019-02-20 14:41:50.000000 phasepy-0.0.8/phasepy/src/actmodels_cy.pyx
--rw-rw-rw-   0        0        0   755022 2019-02-18 15:16:04.000000 phasepy-0.0.8/phasepy/src/cijmix_cy.c
--rw-rw-rw-   0        0        0      436 2019-02-18 14:25:53.000000 phasepy-0.0.8/phasepy/src/cijmix_cy.pyx
--rw-rw-rw-   0        0        0   883946 2019-02-19 12:01:01.000000 phasepy-0.0.8/phasepy/src/coloc_cy.c
--rw-rw-rw-   0        0        0     4852 2019-02-19 12:00:49.000000 phasepy-0.0.8/phasepy/src/coloc_cy.pyx
-drwxrwxrwx   0        0        0        0 2019-03-21 17:47:21.000000 phasepy-0.0.8/phasepy.egg-info/
--rw-rw-rw-   0        0        0     1309 2019-03-21 17:47:20.000000 phasepy-0.0.8/phasepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2019-03-21 17:47:20.000000 phasepy-0.0.8/phasepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-03-21 17:47:20.000000 phasepy-0.0.8/phasepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-02-19 14:20:38.000000 phasepy-0.0.8/phasepy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2019-03-21 17:47:20.000000 phasepy-0.0.8/phasepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2019-03-21 17:47:20.000000 phasepy-0.0.8/phasepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-03-21 17:47:22.000000 phasepy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1690 2019-03-21 17:46:48.000000 phasepy-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:06.000000 phasepy-0.0.9/
+-rw-rw-rw-   0        0        0     1101 2019-02-19 13:16:58.000000 phasepy-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      185 2019-03-02 21:11:36.000000 phasepy-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1309 2019-04-16 02:36:06.000000 phasepy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3003 2019-03-02 21:09:19.000000 phasepy-0.0.9/README.rst
+-rw-rw-rw-   0        0        0      735 2019-03-02 21:09:26.000000 phasepy-0.0.9/long_description.rst
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:05.000000 phasepy-0.0.9/phasepy/
+-rw-rw-rw-   0        0        0     1345 2019-03-02 20:33:15.000000 phasepy-0.0.9/phasepy/__init__.py
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:05.000000 phasepy-0.0.9/phasepy/actmodels/
+-rw-rw-rw-   0        0        0      277 2019-03-02 20:39:17.000000 phasepy-0.0.9/phasepy/actmodels/__init__.py
+-rw-rw-rw-   0        0        0     1583 2019-03-14 19:09:31.000000 phasepy-0.0.9/phasepy/actmodels/nrtl.py
+-rw-rw-rw-   0        0        0     1565 2019-03-02 20:39:26.000000 phasepy-0.0.9/phasepy/actmodels/redlichkister.py
+-rw-rw-rw-   0        0        0     1720 2019-03-02 20:39:31.000000 phasepy-0.0.9/phasepy/actmodels/unifac.py
+-rw-rw-rw-   0        0        0     3988 2019-03-02 20:39:37.000000 phasepy-0.0.9/phasepy/actmodels/virial.py
+-rw-rw-rw-   0        0        0     2195 2019-03-02 20:39:42.000000 phasepy-0.0.9/phasepy/actmodels/virialgama.py
+-rw-rw-rw-   0        0        0      736 2019-03-02 20:39:51.000000 phasepy-0.0.9/phasepy/actmodels/wilson.py
+-rw-rw-rw-   0        0        0      302 2019-03-02 20:33:24.000000 phasepy-0.0.9/phasepy/constants.py
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:06.000000 phasepy-0.0.9/phasepy/cubic/
+-rw-rw-rw-   0        0        0      690 2019-03-02 20:36:36.000000 phasepy-0.0.9/phasepy/cubic/__init__.py
+-rw-rw-rw-   0        0        0      502 2019-03-02 20:36:44.000000 phasepy-0.0.9/phasepy/cubic/alphas.py
+-rw-rw-rw-   0        0        0     3445 2019-03-02 20:34:28.000000 phasepy-0.0.9/phasepy/cubic/cubic.py
+-rw-rw-rw-   0        0        0    19720 2019-03-21 17:43:53.000000 phasepy-0.0.9/phasepy/cubic/cubicmix.py
+-rw-rw-rw-   0        0        0    11058 2019-03-02 20:37:00.000000 phasepy-0.0.9/phasepy/cubic/cubicpure.py
+-rw-rw-rw-   0        0        0     6487 2019-03-05 17:56:32.000000 phasepy-0.0.9/phasepy/cubic/mhv.py
+-rw-rw-rw-   0        0        0     1890 2019-03-02 20:39:06.000000 phasepy-0.0.9/phasepy/cubic/psatpure.py
+-rw-rw-rw-   0        0        0      943 2019-03-05 17:54:32.000000 phasepy-0.0.9/phasepy/cubic/qmr.py
+-rw-rw-rw-   0        0        0    12066 2019-03-19 17:22:04.000000 phasepy-0.0.9/phasepy/cubic/vdwmix.py
+-rw-rw-rw-   0        0        0     8821 2019-03-02 20:37:35.000000 phasepy-0.0.9/phasepy/cubic/vdwpure.py
+-rw-rw-rw-   0        0        0     1897 2019-03-05 19:21:53.000000 phasepy-0.0.9/phasepy/cubic/wongsandler.py
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:06.000000 phasepy-0.0.9/phasepy/database/
+-rw-rw-rw-   0        0        0    50941 2018-09-04 12:45:47.000000 phasepy-0.0.9/phasepy/database/dortmund.xlsx
+-rw-rw-rw-   0        0        0    17186 2018-09-02 20:22:25.000000 phasepy-0.0.9/phasepy/database/unifac.xlsx
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:06.000000 phasepy-0.0.9/phasepy/equilibrium/
+-rw-rw-rw-   0        0        0     1913 2019-03-21 16:47:35.000000 phasepy-0.0.9/phasepy/equilibrium/__init__.py
+-rw-rw-rw-   0        0        0     6759 2019-03-02 20:35:14.000000 phasepy-0.0.9/phasepy/equilibrium/bubble.py
+-rw-rw-rw-   0        0        0     6759 2019-03-02 20:35:19.000000 phasepy-0.0.9/phasepy/equilibrium/dew.py
+-rw-rw-rw-   0        0        0     2146 2019-03-02 20:35:25.000000 phasepy-0.0.9/phasepy/equilibrium/ell.py
+-rw-rw-rw-   0        0        0      616 2019-03-02 20:35:31.000000 phasepy-0.0.9/phasepy/equilibrium/equilibriumresult.py
+-rw-rw-rw-   0        0        0     4498 2019-03-02 20:35:35.000000 phasepy-0.0.9/phasepy/equilibrium/flash.py
+-rw-rw-rw-   0        0        0     2780 2019-03-02 20:35:45.000000 phasepy-0.0.9/phasepy/equilibrium/hazb.py
+-rw-rw-rw-   0        0        0     5397 2019-03-02 20:35:50.000000 phasepy-0.0.9/phasepy/equilibrium/hazt.py
+-rw-rw-rw-   0        0        0     5641 2019-03-02 20:35:55.000000 phasepy-0.0.9/phasepy/equilibrium/multiflash.py
+-rw-rw-rw-   0        0        0     7124 2019-03-02 20:35:59.000000 phasepy-0.0.9/phasepy/equilibrium/stability.py
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:06.000000 phasepy-0.0.9/phasepy/fit/
+-rw-rw-rw-   0        0        0      261 2019-03-02 20:33:55.000000 phasepy-0.0.9/phasepy/fit/__init__.py
+-rw-rw-rw-   0        0        0     5998 2019-03-02 20:34:02.000000 phasepy-0.0.9/phasepy/fit/binaryfit.py
+-rw-rw-rw-   0        0        0      990 2019-03-02 20:34:09.000000 phasepy-0.0.9/phasepy/fit/fitcii.py
+-rw-rw-rw-   0        0        0     3578 2019-03-10 13:05:21.000000 phasepy-0.0.9/phasepy/fit/fitmulticomponent.py
+-rw-rw-rw-   0        0        0     1516 2019-03-02 20:34:35.000000 phasepy-0.0.9/phasepy/fit/fitpsat.py
+-rw-rw-rw-   0        0        0     2836 2019-04-15 19:55:11.000000 phasepy-0.0.9/phasepy/fit/ternaryfit.py
+-rw-rw-rw-   0        0        0      958 2019-03-02 20:33:32.000000 phasepy-0.0.9/phasepy/math.py
+-rw-rw-rw-   0        0        0    15659 2019-04-15 20:06:01.000000 phasepy-0.0.9/phasepy/mixtures.py
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:06.000000 phasepy-0.0.9/phasepy/sgt/
+-rw-rw-rw-   0        0        0      348 2019-03-02 20:32:25.000000 phasepy-0.0.9/phasepy/sgt/__init__.py
+-rw-rw-rw-   0        0        0     3970 2019-03-20 17:52:04.000000 phasepy-0.0.9/phasepy/sgt/coloc_z.py
+-rw-rw-rw-   0        0        0     4743 2019-03-02 20:32:16.000000 phasepy-0.0.9/phasepy/sgt/linear_spot.py
+-rw-rw-rw-   0        0        0     3610 2019-03-02 20:32:10.000000 phasepy-0.0.9/phasepy/sgt/path_hk.py
+-rw-rw-rw-   0        0        0     2387 2019-03-02 20:31:50.000000 phasepy-0.0.9/phasepy/sgt/path_sk.py
+-rw-rw-rw-   0        0        0     2240 2019-03-02 20:31:26.000000 phasepy-0.0.9/phasepy/sgt/reference_component.py
+-rw-rw-rw-   0        0        0     1978 2019-03-02 20:31:16.000000 phasepy-0.0.9/phasepy/sgt/sgtpuros.py
+-rw-rw-rw-   0        0        0      608 2019-03-02 20:31:34.000000 phasepy-0.0.9/phasepy/sgt/tensionresult.py
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:06.000000 phasepy-0.0.9/phasepy/src/
+-rw-rw-rw-   0        0        0   845042 2019-02-20 14:44:57.000000 phasepy-0.0.9/phasepy/src/actmodels_cy.c
+-rw-rw-rw-   0        0        0     4100 2019-02-20 14:41:50.000000 phasepy-0.0.9/phasepy/src/actmodels_cy.pyx
+-rw-rw-rw-   0        0        0   755022 2019-02-18 15:16:04.000000 phasepy-0.0.9/phasepy/src/cijmix_cy.c
+-rw-rw-rw-   0        0        0      436 2019-02-18 14:25:53.000000 phasepy-0.0.9/phasepy/src/cijmix_cy.pyx
+-rw-rw-rw-   0        0        0   883946 2019-02-19 12:01:01.000000 phasepy-0.0.9/phasepy/src/coloc_cy.c
+-rw-rw-rw-   0        0        0     4852 2019-02-19 12:00:49.000000 phasepy-0.0.9/phasepy/src/coloc_cy.pyx
+drwxrwxrwx   0        0        0        0 2019-04-16 02:36:05.000000 phasepy-0.0.9/phasepy.egg-info/
+-rw-rw-rw-   0        0        0     1309 2019-04-16 02:36:05.000000 phasepy-0.0.9/phasepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2019-04-16 02:36:05.000000 phasepy-0.0.9/phasepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-04-16 02:36:05.000000 phasepy-0.0.9/phasepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-02-19 14:20:38.000000 phasepy-0.0.9/phasepy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2019-04-16 02:36:05.000000 phasepy-0.0.9/phasepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2019-04-16 02:36:05.000000 phasepy-0.0.9/phasepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2019-04-16 02:36:06.000000 phasepy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1690 2019-04-16 02:35:44.000000 phasepy-0.0.9/setup.py
```

### Comparing `phasepy-0.0.8/LICENSE.txt` & `phasepy-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/PKG-INFO` & `phasepy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: phasepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multiphase multicomponent Equilibria
 Home-page: https://github.com/gustavochm/phasepy
 Author: Gustavo Chaparro Maldonado, Andrés Mejía Matallana
 Author-email: gustavochaparro@udec.cl
 License: MIT
 Download-URL: https://github.com/gustavochm/phasepy.git
 Description: Phasepy is a open-source scientific python package for fluid phase equilibria computation.
```

### Comparing `phasepy-0.0.8/README.rst` & `phasepy-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/long_description.rst` & `phasepy-0.0.9/long_description.rst`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/__init__.py` & `phasepy-0.0.9/phasepy/__init__.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/actmodels/nrtl.py` & `phasepy-0.0.9/phasepy/actmodels/nrtl.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/actmodels/redlichkister.py` & `phasepy-0.0.9/phasepy/actmodels/redlichkister.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/actmodels/unifac.py` & `phasepy-0.0.9/phasepy/actmodels/unifac.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/actmodels/virial.py` & `phasepy-0.0.9/phasepy/actmodels/virial.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/actmodels/virialgama.py` & `phasepy-0.0.9/phasepy/actmodels/virialgama.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/actmodels/wilson.py` & `phasepy-0.0.9/phasepy/actmodels/wilson.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/__init__.py` & `phasepy-0.0.9/phasepy/cubic/__init__.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/cubic.py` & `phasepy-0.0.9/phasepy/cubic/cubic.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/cubicmix.py` & `phasepy-0.0.9/phasepy/cubic/cubicmix.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/cubicpure.py` & `phasepy-0.0.9/phasepy/cubic/cubicpure.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/mhv.py` & `phasepy-0.0.9/phasepy/cubic/mhv.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/psatpure.py` & `phasepy-0.0.9/phasepy/cubic/psatpure.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/qmr.py` & `phasepy-0.0.9/phasepy/cubic/qmr.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/vdwmix.py` & `phasepy-0.0.9/phasepy/cubic/vdwmix.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/vdwpure.py` & `phasepy-0.0.9/phasepy/cubic/vdwpure.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/cubic/wongsandler.py` & `phasepy-0.0.9/phasepy/cubic/wongsandler.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/database/dortmund.xlsx` & `phasepy-0.0.9/phasepy/database/dortmund.xlsx`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/database/unifac.xlsx` & `phasepy-0.0.9/phasepy/database/unifac.xlsx`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/__init__.py` & `phasepy-0.0.9/phasepy/equilibrium/__init__.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/bubble.py` & `phasepy-0.0.9/phasepy/equilibrium/bubble.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/dew.py` & `phasepy-0.0.9/phasepy/equilibrium/dew.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/ell.py` & `phasepy-0.0.9/phasepy/equilibrium/ell.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/equilibriumresult.py` & `phasepy-0.0.9/phasepy/equilibrium/equilibriumresult.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/flash.py` & `phasepy-0.0.9/phasepy/equilibrium/flash.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/hazb.py` & `phasepy-0.0.9/phasepy/equilibrium/hazb.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/hazt.py` & `phasepy-0.0.9/phasepy/equilibrium/hazt.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/multiflash.py` & `phasepy-0.0.9/phasepy/equilibrium/multiflash.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/equilibrium/stability.py` & `phasepy-0.0.9/phasepy/equilibrium/stability.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/fit/binaryfit.py` & `phasepy-0.0.9/phasepy/fit/binaryfit.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/fit/fitcii.py` & `phasepy-0.0.9/phasepy/fit/fitcii.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/fit/fitmulticomponent.py` & `phasepy-0.0.9/phasepy/fit/fitmulticomponent.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/fit/fitpsat.py` & `phasepy-0.0.9/phasepy/fit/fitpsat.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/fit/ternaryfit.py` & `phasepy-0.0.9/phasepy/fit/ternaryfit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import division, print_function, absolute_import
 import numpy as np
-from ..equilibrium import hazt
+from ..equilibrium import haz
 from ..actmodels import virialgama, nrtlter
 from .fitmulticomponent import fobj_elv, fobj_ell, fobj_hazt
 
 def fobj_nrtlrkt(D,Xexp,Wexp,Yexp,Texp,Pexp,mezcla, good_initial = True):
     
     n = len(Pexp)
     mezcla.rkt(D)
     
     vg = virialgama(mezcla, actmodel = nrtlter)
     x = np.zeros_like(Xexp)
     w = np.zeros_like(Wexp)
     y = np.zeros_like(Yexp)
     
     for i in range(n):
-        x[:,i], w[:,i], y[:,i] = hazt(Xexp[:,i],Wexp[:,i],Yexp[:,i],
+        x[:,i], w[:,i], y[:,i] = haz(Xexp[:,i],Wexp[:,i],Yexp[:,i],
                              Texp[i],Pexp[i],
                              vg, good_initial)
     
         
     error = ((np.nan_to_num(x)-Xexp)**2).sum()
     error += ((np.nan_to_num(w)-Wexp)**2).sum()
     error += ((np.nan_to_num(y)-Yexp)**2).sum()
```

### Comparing `phasepy-0.0.8/phasepy/math.py` & `phasepy-0.0.9/phasepy/math.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/mixtures.py` & `phasepy-0.0.9/phasepy/mixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         Parameters
         ----------
         D: array_like
             ternary interaction parameters values
 
         '''
         self.rkternario = D        
-        self.actmodelp = (self.g, self.alpha, self.g1, self.rkternario)
+        self.actmodelp = (self.alpha, self.g, self.g1, self.rkternario)
     
     def wilson(self,A):
         '''
         Method that adds wilson model parameters to the mixture
         Matrix A main diagonal must be zero. Values in K.
         
         Parameters
```

### Comparing `phasepy-0.0.8/phasepy/sgt/coloc_z.py` & `phasepy-0.0.9/phasepy/sgt/coloc_z.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/sgt/linear_spot.py` & `phasepy-0.0.9/phasepy/sgt/linear_spot.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/sgt/path_hk.py` & `phasepy-0.0.9/phasepy/sgt/path_hk.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/sgt/path_sk.py` & `phasepy-0.0.9/phasepy/sgt/path_sk.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/sgt/reference_component.py` & `phasepy-0.0.9/phasepy/sgt/reference_component.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/sgt/sgtpuros.py` & `phasepy-0.0.9/phasepy/sgt/sgtpuros.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/sgt/tensionresult.py` & `phasepy-0.0.9/phasepy/sgt/tensionresult.py`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/src/actmodels_cy.c` & `phasepy-0.0.9/phasepy/src/actmodels_cy.c`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/src/actmodels_cy.pyx` & `phasepy-0.0.9/phasepy/src/actmodels_cy.pyx`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/src/cijmix_cy.c` & `phasepy-0.0.9/phasepy/src/cijmix_cy.c`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/src/coloc_cy.c` & `phasepy-0.0.9/phasepy/src/coloc_cy.c`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy/src/coloc_cy.pyx` & `phasepy-0.0.9/phasepy/src/coloc_cy.pyx`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/phasepy.egg-info/PKG-INFO` & `phasepy-0.0.9/phasepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: phasepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multiphase multicomponent Equilibria
 Home-page: https://github.com/gustavochm/phasepy
 Author: Gustavo Chaparro Maldonado, Andrés Mejía Matallana
 Author-email: gustavochaparro@udec.cl
 License: MIT
 Download-URL: https://github.com/gustavochm/phasepy.git
 Description: Phasepy is a open-source scientific python package for fluid phase equilibria computation.
```

### Comparing `phasepy-0.0.8/phasepy.egg-info/SOURCES.txt` & `phasepy-0.0.9/phasepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phasepy-0.0.8/setup.py` & `phasepy-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ext_modules +=  [Extension('phasepy.coloc_cy', ['phasepy/src/coloc_cy.c']),
                    Extension('phasepy.actmodels.actmodels_cy', ['phasepy/src/actmodels_cy.c']),
                     Extension('phasepy.sgt.cijmix_cy', ['phasepy/src/cijmix_cy.c'])]
 
 setup(
   name = 'phasepy',
   license='MIT',
-  version = '0.0.8',
+  version = '0.0.9',
   description = 'Multiphase multicomponent Equilibria',
   author = 'Gustavo Chaparro Maldonado, Andrés Mejía Matallana',
   author_email = 'gustavochaparro@udec.cl',
   url = 'https://github.com/gustavochm/phasepy',
   download_url = 'https://github.com/gustavochm/phasepy.git',
   long_description = open('long_description.rst').read(),
   packages = ['phasepy', 'phasepy.cubic', 'phasepy.equilibrium','phasepy.fit', 'phasepy.sgt', 'phasepy.actmodels'],
```


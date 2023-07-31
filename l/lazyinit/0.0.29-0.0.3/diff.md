# Comparing `tmp/lazyinit-0.0.29.tar.gz` & `tmp/lazyinit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.29.tar", last modified: Mon Jul 31 02:24:50 2023, max compression
+gzip compressed data, was "lazyinit-0.0.3.tar", last modified: Mon Jul 31 02:35:28 2023, max compression
```

## Comparing `lazyinit-0.0.29.tar` & `lazyinit-0.0.3.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.127593 lazyinit-0.0.29/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.087204 lazyinit-0.0.29/.git/
--rw-r--r--   0 dengyifan   (501) staff       (20)        3 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/COMMIT_EDITMSG
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:24.000000 lazyinit-0.0.29/.git/FETCH_HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-29 00:34:01.000000 lazyinit-0.0.29/.git/ORIG_HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)      345 2023-07-26 04:10:40.000000 lazyinit-0.0.29/.git/config
--rw-r--r--   0 dengyifan   (501) staff       (20)       73 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/description
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.089633 lazyinit-0.0.29/.git/hooks/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      478 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      896 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4726 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      189 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/post-update.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      424 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1643 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      416 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1374 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/pre-push.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4898 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      544 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1492 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     2783 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     3650 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/hooks/update.sample
--rw-r--r--   0 dengyifan   (501) staff       (20)     4270 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/index
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.089768 lazyinit-0.0.29/.git/info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      240 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/info/exclude
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.089897 lazyinit-0.0.29/.git/logs/
--rw-r--r--   0 dengyifan   (501) staff       (20)     2143 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/logs/HEAD
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.075133 lazyinit-0.0.29/.git/logs/refs/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.090026 lazyinit-0.0.29/.git/logs/refs/heads/
--rw-r--r--   0 dengyifan   (501) staff       (20)     2143 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/logs/refs/heads/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.075186 lazyinit-0.0.29/.git/logs/refs/remotes/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.090404 lazyinit-0.0.29/.git/logs/refs/remotes/origin/
--rw-r--r--   0 dengyifan   (501) staff       (20)     6751 2023-07-29 00:34:13.000000 lazyinit-0.0.29/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)     2105 2023-07-29 00:34:10.000000 lazyinit-0.0.29/.git/logs/refs/remotes/origin/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.084038 lazyinit-0.0.29/.git/objects/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.090568 lazyinit-0.0.29/.git/objects/00/
--r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-25 11:33:45.000000 lazyinit-0.0.29/.git/objects/00/41c04b20be6b4bbd75a815bebf7084805f8712
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.090712 lazyinit-0.0.29/.git/objects/01/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/01/cab3024759cc906cee0a6a3429918f5b63fabc
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.091004 lazyinit-0.0.29/.git/objects/04/
--r--r--r--   0 dengyifan   (501) staff       (20)      553 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063
--r--r--r--   0 dengyifan   (501) staff       (20)     1851 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.091286 lazyinit-0.0.29/.git/objects/05/
--r--r--r--   0 dengyifan   (501) staff       (20)      223 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/05/1acb58a6d6c6dbb4150bf9221569e1912eb5bc
--r--r--r--   0 dengyifan   (501) staff       (20)    42257 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.091477 lazyinit-0.0.29/.git/objects/08/
--r--r--r--   0 dengyifan   (501) staff       (20)     1694 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/08/ea4e268e6f806a7f000c9ae9f7d48f4a770cd9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.091617 lazyinit-0.0.29/.git/objects/0a/
--r--r--r--   0 dengyifan   (501) staff       (20)     2023 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.091754 lazyinit-0.0.29/.git/objects/0b/
--r--r--r--   0 dengyifan   (501) staff       (20)     4720 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/0b/9c91dcf98edb3b3bf9ab9474944a29b6868823
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.091892 lazyinit-0.0.29/.git/objects/0c/
--r--r--r--   0 dengyifan   (501) staff       (20)      126 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/0c/1fe034db405fb5c649a2e85afc24dcd8dafa78
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.092300 lazyinit-0.0.29/.git/objects/0e/
--r--r--r--   0 dengyifan   (501) staff       (20)      261 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/0e/24281e6a23a799bba50234909a4eefc062407f
--r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/0e/3fb35ffbadaf084a2915cfc29e9f63d8dc0b80
--r--r--r--   0 dengyifan   (501) staff       (20)     2330 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.092471 lazyinit-0.0.29/.git/objects/11/
--r--r--r--   0 dengyifan   (501) staff       (20)      119 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/11/f13a31edccde503893c6083b99d6243e26f111
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.092726 lazyinit-0.0.29/.git/objects/12/
--r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/12/c371931538565d632db7e70841c6dd81e6a5e6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.092940 lazyinit-0.0.29/.git/objects/14/
--r--r--r--   0 dengyifan   (501) staff       (20)      146 2023-07-26 06:54:32.000000 lazyinit-0.0.29/.git/objects/14/2068ef3450523a0e5f073bd62eec3746405639
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.093129 lazyinit-0.0.29/.git/objects/17/
--r--r--r--   0 dengyifan   (501) staff       (20)      152 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/17/00d635be40b3166177cbcddfaf61289d501fe6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.093475 lazyinit-0.0.29/.git/objects/1c/
--r--r--r--   0 dengyifan   (501) staff       (20)     1604 2023-07-26 08:16:23.000000 lazyinit-0.0.29/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.093690 lazyinit-0.0.29/.git/objects/1f/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/1f/bc66f0cf2ebf60d3c3d235e0e619a1f6622dbe
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.094076 lazyinit-0.0.29/.git/objects/22/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 14:00:51.000000 lazyinit-0.0.29/.git/objects/22/1b9304fb057784a1c767bdf222a4fd449db92f
--r--r--r--   0 dengyifan   (501) staff       (20)      283 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/22/28de42f4fd7fd7e337c26be6c47fa320f3555f
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.094249 lazyinit-0.0.29/.git/objects/24/
--r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/24/0d08419d20e2d7cb6985f76926f93b83a8daa7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.094426 lazyinit-0.0.29/.git/objects/27/
--r--r--r--   0 dengyifan   (501) staff       (20)     2565 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/27/1af1abadcaf261f7305ee5239e60d63a2a49ac
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.094598 lazyinit-0.0.29/.git/objects/28/
--r--r--r--   0 dengyifan   (501) staff       (20)      358 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/28/5445a221c929c5f5f87e202f37320844e8f6d0
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.094773 lazyinit-0.0.29/.git/objects/2a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1878 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.094955 lazyinit-0.0.29/.git/objects/2b/
--r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/2b/c85ce5ce789ef99ce23645128dcbaad1ff3835
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.095135 lazyinit-0.0.29/.git/objects/2d/
--r--r--r--   0 dengyifan   (501) staff       (20)      372 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/2d/d1db85bd19ef19b8f7730625f1740902a4f846
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.095314 lazyinit-0.0.29/.git/objects/2e/
--r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.095487 lazyinit-0.0.29/.git/objects/31/
--r--r--r--   0 dengyifan   (501) staff       (20)      545 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/31/93627be78d312d8aca9e6da7d9d2aad6a5b1d3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.095831 lazyinit-0.0.29/.git/objects/32/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/32/025d715d168680f84c440a9eaa445bcfe82201
--r--r--r--   0 dengyifan   (501) staff       (20)     2217 2023-07-25 11:33:45.000000 lazyinit-0.0.29/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.096005 lazyinit-0.0.29/.git/objects/33/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 14:00:51.000000 lazyinit-0.0.29/.git/objects/33/1de14f34212468dbd7962fcd3aa2c27159be15
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.096176 lazyinit-0.0.29/.git/objects/38/
--r--r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/38/d0b85fd4bdd1685656cd6027825010486286ab
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.096522 lazyinit-0.0.29/.git/objects/39/
--r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/39/c27ee30de9577fb056d6adf1a75b5040624f1a
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:41:16.000000 lazyinit-0.0.29/.git/objects/39/df26c768c14049a07f62ddef6c9d8fe3635b43
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.096760 lazyinit-0.0.29/.git/objects/3c/
--r--r--r--   0 dengyifan   (501) staff       (20)       46 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/3c/8b0c9f1be9bc778fa8c70f9b1e297d343e7140
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.097148 lazyinit-0.0.29/.git/objects/3d/
--r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/3d/5d200d32889f9867e73ddd61f8de5d54006cca
--r--r--r--   0 dengyifan   (501) staff       (20)     1867 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.097321 lazyinit-0.0.29/.git/objects/40/
--r--r--r--   0 dengyifan   (501) staff       (20)      513 2023-07-25 11:41:16.000000 lazyinit-0.0.29/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.097491 lazyinit-0.0.29/.git/objects/41/
--r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 06:54:32.000000 lazyinit-0.0.29/.git/objects/41/483d9c24d49b463a3afea6c339c9444c92f01d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.097656 lazyinit-0.0.29/.git/objects/43/
--r--r--r--   0 dengyifan   (501) staff       (20)      291 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/43/3b5b7262dcbe0429a0a8e7ed7aee7ed4793ed4
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.097827 lazyinit-0.0.29/.git/objects/4d/
--r--r--r--   0 dengyifan   (501) staff       (20)     1995 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.097986 lazyinit-0.0.29/.git/objects/52/
--r--r--r--   0 dengyifan   (501) staff       (20)     2033 2023-07-25 11:41:16.000000 lazyinit-0.0.29/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.098147 lazyinit-0.0.29/.git/objects/55/
--r--r--r--   0 dengyifan   (501) staff       (20)      145 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/55/3ee9d39a64d1c55b084c4821a83d6574cee6da
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.098316 lazyinit-0.0.29/.git/objects/56/
--r--r--r--   0 dengyifan   (501) staff       (20)     3553 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.098485 lazyinit-0.0.29/.git/objects/5a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1979 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.098658 lazyinit-0.0.29/.git/objects/5e/
--r--r--r--   0 dengyifan   (501) staff       (20)     1486 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.099038 lazyinit-0.0.29/.git/objects/5f/
--r--r--r--   0 dengyifan   (501) staff       (20)      125 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/5f/21b1e6c2be3514a4d5118cd8db61899648080a
--r--r--r--   0 dengyifan   (501) staff       (20)      549 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.099358 lazyinit-0.0.29/.git/objects/60/
--r--r--r--   0 dengyifan   (501) staff       (20)      514 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 06:54:32.000000 lazyinit-0.0.29/.git/objects/60/41ee332e98835ce7e3ed8b3ae41f91352bec33
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.099503 lazyinit-0.0.29/.git/objects/61/
--r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/61/627626599ca0c79132f84fb7f4a958bcea0351
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.100053 lazyinit-0.0.29/.git/objects/63/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/63/29d30bc981284e510de0c1938ade4c16e7bde9
--r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/63/3cf9d6946c15485dcb3cf3889f6b34de0c0bcd
--r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/63/58ed86fda8471ab44b0366d535c7e7d5c4b449
--r--r--r--   0 dengyifan   (501) staff       (20)     2007 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.100651 lazyinit-0.0.29/.git/objects/64/
--r--r--r--   0 dengyifan   (501) staff       (20)     2420 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.100933 lazyinit-0.0.29/.git/objects/65/
--r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/65/1f8be5881c19639f37ff5dea35133eab4d8250
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.101091 lazyinit-0.0.29/.git/objects/67/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/67/bf3997c2bc19d4034bd741ab9808c86b52376b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.101837 lazyinit-0.0.29/.git/objects/69/
--r--r--r--   0 dengyifan   (501) staff       (20)      930 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.102897 lazyinit-0.0.29/.git/objects/6a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1554 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.103380 lazyinit-0.0.29/.git/objects/6b/
--r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.103764 lazyinit-0.0.29/.git/objects/6c/
--r--r--r--   0 dengyifan   (501) staff       (20)     1966 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66
--r--r--r--   0 dengyifan   (501) staff       (20)      233 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/6c/f23ede6f0221263856d80f2287298ce360df0d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.103902 lazyinit-0.0.29/.git/objects/6d/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/6d/8911d55f9896b814e9db65f2edc1da1524c03b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.104081 lazyinit-0.0.29/.git/objects/6e/
--r--r--r--   0 dengyifan   (501) staff       (20)       37 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/6e/30ca1116ed7b5e804a19fc761a7a2d58c0e1dd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.104401 lazyinit-0.0.29/.git/objects/6f/
--r--r--r--   0 dengyifan   (501) staff       (20)      496 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/6f/9a4b893df9fff8b3995e4014388ba30f129cd2
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/6f/cdcf4e30a9697c1f5aceaf1dc7d39d98739f51
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.104739 lazyinit-0.0.29/.git/objects/73/
--r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/73/58417a5d41c0ae3f227f79be64cff1341921f3
--r--r--r--   0 dengyifan   (501) staff       (20)      737 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/73/ddeb46272ee036799c78fb7748411ffef6da2a
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.105173 lazyinit-0.0.29/.git/objects/74/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/74/453505ab7b002053a991e77614b41494aefd94
--r--r--r--   0 dengyifan   (501) staff       (20)      180 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/74/94617eb236a96a42041354b497fb373ff69e2a
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/74/e45b20bcfa13204500b46f9b3f794a2eedd610
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.105440 lazyinit-0.0.29/.git/objects/7e/
--r--r--r--   0 dengyifan   (501) staff       (20)      336 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/7e/c698da62500825d9d6cba8fec1d0179d3c5de9
--r--r--r--   0 dengyifan   (501) staff       (20)      499 2023-07-25 11:33:45.000000 lazyinit-0.0.29/.git/objects/7e/cdeefbee966a2c48b1f3e93aef8772a83a927b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.105586 lazyinit-0.0.29/.git/objects/7f/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/7f/3aff99db09db5b9be0eb49dfbb83e5a2b2dfe6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.105723 lazyinit-0.0.29/.git/objects/80/
--r--r--r--   0 dengyifan   (501) staff       (20)      561 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.106000 lazyinit-0.0.29/.git/objects/83/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:41:16.000000 lazyinit-0.0.29/.git/objects/83/410ee7dbb23a43716f77560dfb52b6dbab167b
--r--r--r--   0 dengyifan   (501) staff       (20)     7437 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.106136 lazyinit-0.0.29/.git/objects/84/
--r--r--r--   0 dengyifan   (501) staff       (20)      281 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/84/32f5170b60379a5440d18af5c42da0c20bab36
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.106286 lazyinit-0.0.29/.git/objects/86/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 08:16:23.000000 lazyinit-0.0.29/.git/objects/86/305819935ba7c71d91c90bb164a58e855e7d1e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.106435 lazyinit-0.0.29/.git/objects/87/
--r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 08:16:23.000000 lazyinit-0.0.29/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.106591 lazyinit-0.0.29/.git/objects/88/
--r--r--r--   0 dengyifan   (501) staff       (20)     3155 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.106751 lazyinit-0.0.29/.git/objects/89/
--r--r--r--   0 dengyifan   (501) staff       (20)       34 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/89/fe87522f1d1d21fb72f29e4a3f3044b32cc64c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.106911 lazyinit-0.0.29/.git/objects/8b/
--r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 08:16:23.000000 lazyinit-0.0.29/.git/objects/8b/538f3380f85f22fc479f2298de08af638d91f6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.107070 lazyinit-0.0.29/.git/objects/8f/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/8f/821694556aac2a278c288de223659193dd2489
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.107223 lazyinit-0.0.29/.git/objects/91/
--r--r--r--   0 dengyifan   (501) staff       (20)     2328 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.107544 lazyinit-0.0.29/.git/objects/96/
--r--r--r--   0 dengyifan   (501) staff       (20)     3726 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/96/7c51d6a0690049febfd310c0257eb795caeaef
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.107779 lazyinit-0.0.29/.git/objects/99/
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/99/aee23747e74ecbb3e8ebdc64b65c85c55f51dd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.108280 lazyinit-0.0.29/.git/objects/9c/
--r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef
--r--r--r--   0 dengyifan   (501) staff       (20)     2012 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/9c/a267b4612588367daa875d4f23cb8458c21e03
--r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/9c/fa0e1bf241048b8a143c7fef01067d5f9c3ac7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.108819 lazyinit-0.0.29/.git/objects/9d/
--r--r--r--   0 dengyifan   (501) staff       (20)      150 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/9d/1f61df1650e8ae0165c5d3e1f47e8384a76e25
--r--r--r--   0 dengyifan   (501) staff       (20)     2983 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.109310 lazyinit-0.0.29/.git/objects/a0/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/a0/2c8ecffe863e22a9a7510d5af5f8472da012c4
--r--r--r--   0 dengyifan   (501) staff       (20)      494 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/a0/8ceea5fa60b6a189bf2ca3e11a3e82d84375ea
--r--r--r--   0 dengyifan   (501) staff       (20)     1903 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.109583 lazyinit-0.0.29/.git/objects/a1/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:33:45.000000 lazyinit-0.0.29/.git/objects/a1/e2f9a9114e1b772f7fb22f7c2a26fc8fcf25ac
--r--r--r--   0 dengyifan   (501) staff       (20)     2165 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.109718 lazyinit-0.0.29/.git/objects/a3/
--r--r--r--   0 dengyifan   (501) staff       (20)      555 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.109995 lazyinit-0.0.29/.git/objects/a8/
--r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:33:45.000000 lazyinit-0.0.29/.git/objects/a8/8453b2586a082782d165b46444353c6fda84f5
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.110408 lazyinit-0.0.29/.git/objects/a9/
--r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-28 04:10:06.000000 lazyinit-0.0.29/.git/objects/a9/7852c14503686493d3218632fbbb52dd42628b
--r--r--r--   0 dengyifan   (501) staff       (20)      557 2023-07-28 04:10:06.000000 lazyinit-0.0.29/.git/objects/a9/95569e1ac0accec5b1acc68f0ab077023bc4f4
--r--r--r--   0 dengyifan   (501) staff       (20)     1465 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.110816 lazyinit-0.0.29/.git/objects/aa/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/aa/2f814ba87b54003ea2facaf8a8ac437b174212
--r--r--r--   0 dengyifan   (501) staff       (20)      920 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487
--r--r--r--   0 dengyifan   (501) staff       (20)     1811 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.110952 lazyinit-0.0.29/.git/objects/ad/
--r--r--r--   0 dengyifan   (501) staff       (20)     3750 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.111230 lazyinit-0.0.29/.git/objects/ae/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/ae/99dcc87c6ca438bd127b06eee3ccc47f4ffd6c
--r--r--r--   0 dengyifan   (501) staff       (20)      215 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/ae/ca62bc1646058816f9a5bddd5681d0fb939b24
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.111671 lazyinit-0.0.29/.git/objects/af/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/af/272c05462dae29b6aadb455022bdbbf9f531e7
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/af/38c03c42f711bbfe4db00e49e92fb5761c80d7
--r--r--r--   0 dengyifan   (501) staff       (20)     1602 2023-07-26 06:54:32.000000 lazyinit-0.0.29/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.111952 lazyinit-0.0.29/.git/objects/b0/
--r--r--r--   0 dengyifan   (501) staff       (20)     4121 2023-07-26 05:00:09.000000 lazyinit-0.0.29/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/b0/8c7ef81a8076086a4529e40583d52ff2e03d24
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.112083 lazyinit-0.0.29/.git/objects/b1/
--r--r--r--   0 dengyifan   (501) staff       (20)      729 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.112222 lazyinit-0.0.29/.git/objects/b4/
--r--r--r--   0 dengyifan   (501) staff       (20)      124 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/b4/31ec69865aa69f6bbac9893d5f3266ecd13273
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.112523 lazyinit-0.0.29/.git/objects/b6/
--r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/b6/9f632da541ff48fd18a636d74fca4d80935113
--r--r--r--   0 dengyifan   (501) staff       (20)       20 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/b6/fc4c620b67d95f953a5c1c1230aaab5db5a1b0
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.112667 lazyinit-0.0.29/.git/objects/b7/
--r--r--r--   0 dengyifan   (501) staff       (20)      500 2023-07-25 11:16:46.000000 lazyinit-0.0.29/.git/objects/b7/8ccba97db82f1ca4c6db7e0b5cd1bd8af07780
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.112802 lazyinit-0.0.29/.git/objects/b9/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/b9/0686ac668cc417b91f372b51c3a15920445b29
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.112936 lazyinit-0.0.29/.git/objects/bb/
--r--r--r--   0 dengyifan   (501) staff       (20)       31 2023-07-26 06:54:32.000000 lazyinit-0.0.29/.git/objects/bb/b84aa70c64fb0114dfa2f1df1cfffbc0123de9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.113582 lazyinit-0.0.29/.git/objects/bc/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/bc/771507d6ab55b2ca55d1b567dc38064561aa6f
--r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01
--r--r--r--   0 dengyifan   (501) staff       (20)     2346 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385
--r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-25 11:41:16.000000 lazyinit-0.0.29/.git/objects/bc/e5df5b3fb9303de75d9ba662475c2e0940387e
--r--r--r--   0 dengyifan   (501) staff       (20)      200 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/bc/ed2eb0d31276a7b1ddfe5855190dc53fec2a91
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.113711 lazyinit-0.0.29/.git/objects/c1/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/c1/b6c43ce95f33b1c96bb259fd2c2facd4406ef8
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.114053 lazyinit-0.0.29/.git/objects/c4/
--r--r--r--   0 dengyifan   (501) staff       (20)     2032 2023-07-25 11:33:45.000000 lazyinit-0.0.29/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.114324 lazyinit-0.0.29/.git/objects/c5/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/c5/4ad76a5bccb99831a7a16f98637da3903c2cec
--r--r--r--   0 dengyifan   (501) staff       (20)      450 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/c5/f23c1c12745e22b14c79b57d397ae6685cf564
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.114464 lazyinit-0.0.29/.git/objects/c7/
--r--r--r--   0 dengyifan   (501) staff       (20)     1654 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.114910 lazyinit-0.0.29/.git/objects/c9/
--r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.115065 lazyinit-0.0.29/.git/objects/ca/
--r--r--r--   0 dengyifan   (501) staff       (20)     1263 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.115881 lazyinit-0.0.29/.git/objects/cc/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/cc/3a12d725fdd1884f2f104e1c11d8b87c1367cc
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/cc/46e850693cec9659b52d57dd78d6f60c242ebb
--r--r--r--   0 dengyifan   (501) staff       (20)      716 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.116195 lazyinit-0.0.29/.git/objects/cd/
--r--r--r--   0 dengyifan   (501) staff       (20)     5189 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591
--r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 06:54:32.000000 lazyinit-0.0.29/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.116355 lazyinit-0.0.29/.git/objects/ce/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/ce/3694e653f842cc70a8c5ef32cd9f75639bb14a
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.116503 lazyinit-0.0.29/.git/objects/d2/
--r--r--r--   0 dengyifan   (501) staff       (20)      163 2023-07-28 04:10:06.000000 lazyinit-0.0.29/.git/objects/d2/99be9b16073ba179c8b1558984116cd0eb9f3b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.116670 lazyinit-0.0.29/.git/objects/d9/
--r--r--r--   0 dengyifan   (501) staff       (20)     5194 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.117013 lazyinit-0.0.29/.git/objects/da/
--r--r--r--   0 dengyifan   (501) staff       (20)      116 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/da/34810fd3a6a883dbaf24d1123d0c38468460a5
--r--r--r--   0 dengyifan   (501) staff       (20)      491 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/da/9fd18a499c0821bea6c2313d252a1d4bcf5846
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.117231 lazyinit-0.0.29/.git/objects/de/
--r--r--r--   0 dengyifan   (501) staff       (20)      100 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/de/8f446f94a50f937fed1c254a966f3ed6088e81
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.117397 lazyinit-0.0.29/.git/objects/df/
--r--r--r--   0 dengyifan   (501) staff       (20)     1977 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.117583 lazyinit-0.0.29/.git/objects/e4/
--r--r--r--   0 dengyifan   (501) staff       (20)      149 2023-07-25 14:00:51.000000 lazyinit-0.0.29/.git/objects/e4/632035cac16d026cc02de90ae31aef87867116
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.117751 lazyinit-0.0.29/.git/objects/e6/
--r--r--r--   0 dengyifan   (501) staff       (20)       15 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.118189 lazyinit-0.0.29/.git/objects/e8/
--r--r--r--   0 dengyifan   (501) staff       (20)      556 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b
--r--r--r--   0 dengyifan   (501) staff       (20)     1289 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.118519 lazyinit-0.0.29/.git/objects/eb/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/eb/758cdc0fe911d913b208b48ee0ac14886927eb
--r--r--r--   0 dengyifan   (501) staff       (20)      566 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.118725 lazyinit-0.0.29/.git/objects/ec/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/ec/47fd64ca8d46a3a1c345708cf6dd4b19e2d7a6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.119063 lazyinit-0.0.29/.git/objects/ef/
--r--r--r--   0 dengyifan   (501) staff       (20)      219 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/ef/0a2b00e7e0280dfe13a94d5abfeeba9aafabae
--r--r--r--   0 dengyifan   (501) staff       (20)      517 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/ef/cd52b6011e351ce3a00aa0473feeb8b10fe43d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.119356 lazyinit-0.0.29/.git/objects/f0/
--r--r--r--   0 dengyifan   (501) staff       (20)     8516 2023-07-26 04:07:28.000000 lazyinit-0.0.29/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c
--r--r--r--   0 dengyifan   (501) staff       (20)      433 2023-07-24 06:27:07.000000 lazyinit-0.0.29/.git/objects/f0/b6b75cf9a30d91dab0d80449c7c76a0191d8a7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.119495 lazyinit-0.0.29/.git/objects/f1/
--r--r--r--   0 dengyifan   (501) staff       (20)      559 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.119639 lazyinit-0.0.29/.git/objects/f2/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/f2/f3ccb260633b09276ccaaa358ce7df1a0025f6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.119774 lazyinit-0.0.29/.git/objects/f5/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 14:32:29.000000 lazyinit-0.0.29/.git/objects/f5/96444b272664dff576dc8ac874152f461a4f6e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.119949 lazyinit-0.0.29/.git/objects/f6/
--r--r--r--   0 dengyifan   (501) staff       (20)     2002 2023-07-26 03:36:35.000000 lazyinit-0.0.29/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.084258 lazyinit-0.0.29/.git/refs/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.120126 lazyinit-0.0.29/.git/refs/heads/
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-29 00:34:07.000000 lazyinit-0.0.29/.git/refs/heads/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.084318 lazyinit-0.0.29/.git/refs/remotes/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.120449 lazyinit-0.0.29/.git/refs/remotes/origin/
--rw-r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-29 00:34:13.000000 lazyinit-0.0.29/.git/refs/remotes/origin/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-29 00:34:10.000000 lazyinit-0.0.29/.git/refs/remotes/origin/master
--rw-r--r--   0 dengyifan   (501) staff       (20)       17 2023-07-26 05:01:41.000000 lazyinit-0.0.29/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      425 2023-07-31 02:24:50.127380 lazyinit-0.0.29/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      184 2023-07-29 00:34:01.000000 lazyinit-0.0.29/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.121434 lazyinit-0.0.29/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.29/lazyinit/__init__.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.122612 lazyinit-0.0.29/lazyinit/__pycache__/
--rw-r--r--   0 dengyifan   (501) staff       (20)      179 2023-07-27 12:30:23.000000 lazyinit-0.0.29/lazyinit/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dengyifan   (501) staff       (20)    10748 2023-07-27 12:30:23.000000 lazyinit-0.0.29/lazyinit/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 dengyifan   (501) staff       (20)     3763 2023-07-25 04:13:11.000000 lazyinit-0.0.29/lazyinit/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.29/lazyinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     8549 2023-07-29 00:29:14.000000 lazyinit-0.0.29/lazyinit/init.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.123276 lazyinit-0.0.29/lazyinit/lazydl/
--rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-07-23 08:07:15.000000 lazyinit-0.0.29/lazyinit/lazydl/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.123383 lazyinit-0.0.29/lazyinit/lazydl/configs/
--rw-r--r--   0 dengyifan   (501) staff       (20)     1375 2023-07-29 00:33:21.000000 lazyinit-0.0.29/lazyinit/lazydl/configs/default_config.yaml
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.084859 lazyinit-0.0.29/lazyinit/lazydl/configs/exps/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.123650 lazyinit-0.0.29/lazyinit/lazydl/configs/exps/exp1/
--rw-r--r--   0 dengyifan   (501) staff       (20)     3903 2023-07-25 13:51:05.000000 lazyinit-0.0.29/lazyinit/lazydl/configs/exps/exp1/baseline.yaml
--rw-r--r--   0 dengyifan   (501) staff       (20)     1152 2023-07-29 00:31:59.000000 lazyinit-0.0.29/lazyinit/lazydl/configs/exps/exp1/exp_plan.yaml
--rw-r--r--   0 dengyifan   (501) staff       (20)     1179 2023-07-23 08:16:18.000000 lazyinit-0.0.29/lazyinit/lazydl/minist.py
--rw-r--r--   0 dengyifan   (501) staff       (20)       16 2023-07-23 08:07:15.000000 lazyinit-0.0.29/lazyinit/lazydl/requirements.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     2727 2023-07-23 08:07:15.000000 lazyinit-0.0.29/lazyinit/lazydl/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-24 14:38:46.000000 lazyinit-0.0.29/lazyinit/lazydl/start.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.124906 lazyinit-0.0.29/lazyinit/ranger/
--rw-r--r--   0 dengyifan   (501) staff       (20)     6148 2023-07-24 04:18:46.000000 lazyinit-0.0.29/lazyinit/ranger/.DS_Store
--rwxr-xr-x   0 dengyifan   (501) staff       (20)       23 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.126147 lazyinit-0.0.29/lazyinit/ranger/colorschemes/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/colorschemes/__init__.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      139 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/colorschemes/__init__.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     5769 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/colorschemes/default.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      696 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/colorschemes/jungle.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1171 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/colorschemes/snow.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1335 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/colorschemes/snow.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4929 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/colorschemes/zenburn.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4758 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/commands.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.127085 lazyinit-0.0.29/lazyinit/ranger/plugins/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/plugins/__init__.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      134 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/plugins/__init__.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    10718 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/plugins/devicons.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     6817 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/plugins/devicons.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      479 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/plugins/devicons_linemode.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1271 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/plugins/devicons_linemode.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    23026 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/rc-sample.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    18894 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/rc.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    13012 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/rifle.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    10000 2023-07-23 10:15:36.000000 lazyinit-0.0.29/lazyinit/ranger/scope.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.29/lazyinit/redis.conf
--rw-r--r--   0 dengyifan   (501) staff       (20)      142 2023-07-27 04:35:53.000000 lazyinit-0.0.29/lazyinit/redis.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-29 00:29:59.000000 lazyinit-0.0.29/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     6724 2023-07-27 11:48:11.000000 lazyinit-0.0.29/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:24:50.122207 lazyinit-0.0.29/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      425 2023-07-31 02:24:50.000000 lazyinit-0.0.29/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)    11165 2023-07-31 02:24:50.000000 lazyinit-0.0.29/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-31 02:24:50.000000 lazyinit-0.0.29/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-31 02:24:50.000000 lazyinit-0.0.29/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-31 02:24:50.000000 lazyinit-0.0.29/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-31 02:24:50.000000 lazyinit-0.0.29/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     1059 2023-07-23 12:54:16.000000 lazyinit-0.0.29/push.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-31 02:24:50.127655 lazyinit-0.0.29/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      844 2023-07-31 02:24:48.000000 lazyinit-0.0.29/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.286318 lazyinit-0.0.3/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.232041 lazyinit-0.0.3/.git/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        3 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/COMMIT_EDITMSG
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:33:30.000000 lazyinit-0.0.3/.git/FETCH_HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-29 00:34:01.000000 lazyinit-0.0.3/.git/ORIG_HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)      345 2023-07-26 04:10:40.000000 lazyinit-0.0.3/.git/config
+-rw-r--r--   0 dengyifan   (501) staff       (20)       73 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/description
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.233993 lazyinit-0.0.3/.git/hooks/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      478 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      896 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4726 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      189 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/post-update.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      424 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1643 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      416 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1374 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4898 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      544 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1492 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     2783 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     3650 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/hooks/update.sample
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4270 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/index
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.234150 lazyinit-0.0.3/.git/info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      240 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/info/exclude
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.234300 lazyinit-0.0.3/.git/logs/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2143 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/logs/HEAD
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.219835 lazyinit-0.0.3/.git/logs/refs/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.234461 lazyinit-0.0.3/.git/logs/refs/heads/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2143 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/logs/refs/heads/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.219888 lazyinit-0.0.3/.git/logs/refs/remotes/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.234908 lazyinit-0.0.3/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6751 2023-07-29 00:34:13.000000 lazyinit-0.0.3/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2105 2023-07-29 00:34:10.000000 lazyinit-0.0.3/.git/logs/refs/remotes/origin/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.229478 lazyinit-0.0.3/.git/objects/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.235097 lazyinit-0.0.3/.git/objects/00/
+-r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-25 11:33:45.000000 lazyinit-0.0.3/.git/objects/00/41c04b20be6b4bbd75a815bebf7084805f8712
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.235287 lazyinit-0.0.3/.git/objects/01/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/01/cab3024759cc906cee0a6a3429918f5b63fabc
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.235624 lazyinit-0.0.3/.git/objects/04/
+-r--r--r--   0 dengyifan   (501) staff       (20)      553 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063
+-r--r--r--   0 dengyifan   (501) staff       (20)     1851 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.235937 lazyinit-0.0.3/.git/objects/05/
+-r--r--r--   0 dengyifan   (501) staff       (20)      223 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/05/1acb58a6d6c6dbb4150bf9221569e1912eb5bc
+-r--r--r--   0 dengyifan   (501) staff       (20)    42257 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.236126 lazyinit-0.0.3/.git/objects/08/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1694 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/08/ea4e268e6f806a7f000c9ae9f7d48f4a770cd9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.236265 lazyinit-0.0.3/.git/objects/0a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2023 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.236401 lazyinit-0.0.3/.git/objects/0b/
+-r--r--r--   0 dengyifan   (501) staff       (20)     4720 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/0b/9c91dcf98edb3b3bf9ab9474944a29b6868823
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.236551 lazyinit-0.0.3/.git/objects/0c/
+-r--r--r--   0 dengyifan   (501) staff       (20)      126 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/0c/1fe034db405fb5c649a2e85afc24dcd8dafa78
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.236945 lazyinit-0.0.3/.git/objects/0e/
+-r--r--r--   0 dengyifan   (501) staff       (20)      261 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/0e/24281e6a23a799bba50234909a4eefc062407f
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/0e/3fb35ffbadaf084a2915cfc29e9f63d8dc0b80
+-r--r--r--   0 dengyifan   (501) staff       (20)     2330 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.237127 lazyinit-0.0.3/.git/objects/11/
+-r--r--r--   0 dengyifan   (501) staff       (20)      119 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/11/f13a31edccde503893c6083b99d6243e26f111
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.237303 lazyinit-0.0.3/.git/objects/12/
+-r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/12/c371931538565d632db7e70841c6dd81e6a5e6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.237488 lazyinit-0.0.3/.git/objects/14/
+-r--r--r--   0 dengyifan   (501) staff       (20)      146 2023-07-26 06:54:32.000000 lazyinit-0.0.3/.git/objects/14/2068ef3450523a0e5f073bd62eec3746405639
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.237649 lazyinit-0.0.3/.git/objects/17/
+-r--r--r--   0 dengyifan   (501) staff       (20)      152 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/17/00d635be40b3166177cbcddfaf61289d501fe6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.237819 lazyinit-0.0.3/.git/objects/1c/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1604 2023-07-26 08:16:23.000000 lazyinit-0.0.3/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.237996 lazyinit-0.0.3/.git/objects/1f/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/1f/bc66f0cf2ebf60d3c3d235e0e619a1f6622dbe
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.238336 lazyinit-0.0.3/.git/objects/22/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 14:00:51.000000 lazyinit-0.0.3/.git/objects/22/1b9304fb057784a1c767bdf222a4fd449db92f
+-r--r--r--   0 dengyifan   (501) staff       (20)      283 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/22/28de42f4fd7fd7e337c26be6c47fa320f3555f
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.238525 lazyinit-0.0.3/.git/objects/24/
+-r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/24/0d08419d20e2d7cb6985f76926f93b83a8daa7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.238700 lazyinit-0.0.3/.git/objects/27/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2565 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/27/1af1abadcaf261f7305ee5239e60d63a2a49ac
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.238886 lazyinit-0.0.3/.git/objects/28/
+-r--r--r--   0 dengyifan   (501) staff       (20)      358 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/28/5445a221c929c5f5f87e202f37320844e8f6d0
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.239060 lazyinit-0.0.3/.git/objects/2a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1878 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.239230 lazyinit-0.0.3/.git/objects/2b/
+-r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/2b/c85ce5ce789ef99ce23645128dcbaad1ff3835
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.239401 lazyinit-0.0.3/.git/objects/2d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      372 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/2d/d1db85bd19ef19b8f7730625f1740902a4f846
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.239576 lazyinit-0.0.3/.git/objects/2e/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.239761 lazyinit-0.0.3/.git/objects/31/
+-r--r--r--   0 dengyifan   (501) staff       (20)      545 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/31/93627be78d312d8aca9e6da7d9d2aad6a5b1d3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.240110 lazyinit-0.0.3/.git/objects/32/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/32/025d715d168680f84c440a9eaa445bcfe82201
+-r--r--r--   0 dengyifan   (501) staff       (20)     2217 2023-07-25 11:33:45.000000 lazyinit-0.0.3/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.240282 lazyinit-0.0.3/.git/objects/33/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 14:00:51.000000 lazyinit-0.0.3/.git/objects/33/1de14f34212468dbd7962fcd3aa2c27159be15
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.240471 lazyinit-0.0.3/.git/objects/38/
+-r--r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/38/d0b85fd4bdd1685656cd6027825010486286ab
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.240785 lazyinit-0.0.3/.git/objects/39/
+-r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/39/c27ee30de9577fb056d6adf1a75b5040624f1a
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:41:16.000000 lazyinit-0.0.3/.git/objects/39/df26c768c14049a07f62ddef6c9d8fe3635b43
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.240933 lazyinit-0.0.3/.git/objects/3c/
+-r--r--r--   0 dengyifan   (501) staff       (20)       46 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/3c/8b0c9f1be9bc778fa8c70f9b1e297d343e7140
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.241203 lazyinit-0.0.3/.git/objects/3d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/3d/5d200d32889f9867e73ddd61f8de5d54006cca
+-r--r--r--   0 dengyifan   (501) staff       (20)     1867 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.241364 lazyinit-0.0.3/.git/objects/40/
+-r--r--r--   0 dengyifan   (501) staff       (20)      513 2023-07-25 11:41:16.000000 lazyinit-0.0.3/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.241525 lazyinit-0.0.3/.git/objects/41/
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 06:54:32.000000 lazyinit-0.0.3/.git/objects/41/483d9c24d49b463a3afea6c339c9444c92f01d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.241679 lazyinit-0.0.3/.git/objects/43/
+-r--r--r--   0 dengyifan   (501) staff       (20)      291 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/43/3b5b7262dcbe0429a0a8e7ed7aee7ed4793ed4
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.241827 lazyinit-0.0.3/.git/objects/4d/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1995 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.242030 lazyinit-0.0.3/.git/objects/52/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2033 2023-07-25 11:41:16.000000 lazyinit-0.0.3/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.242203 lazyinit-0.0.3/.git/objects/55/
+-r--r--r--   0 dengyifan   (501) staff       (20)      145 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/55/3ee9d39a64d1c55b084c4821a83d6574cee6da
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.242368 lazyinit-0.0.3/.git/objects/56/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3553 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.242540 lazyinit-0.0.3/.git/objects/5a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1979 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.242710 lazyinit-0.0.3/.git/objects/5e/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1486 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.243040 lazyinit-0.0.3/.git/objects/5f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      125 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/5f/21b1e6c2be3514a4d5118cd8db61899648080a
+-r--r--r--   0 dengyifan   (501) staff       (20)      549 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.243376 lazyinit-0.0.3/.git/objects/60/
+-r--r--r--   0 dengyifan   (501) staff       (20)      514 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 06:54:32.000000 lazyinit-0.0.3/.git/objects/60/41ee332e98835ce7e3ed8b3ae41f91352bec33
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.243542 lazyinit-0.0.3/.git/objects/61/
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/61/627626599ca0c79132f84fb7f4a958bcea0351
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.244376 lazyinit-0.0.3/.git/objects/63/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/63/29d30bc981284e510de0c1938ade4c16e7bde9
+-r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/63/3cf9d6946c15485dcb3cf3889f6b34de0c0bcd
+-r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/63/58ed86fda8471ab44b0366d535c7e7d5c4b449
+-r--r--r--   0 dengyifan   (501) staff       (20)     2007 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.244560 lazyinit-0.0.3/.git/objects/64/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2420 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.244733 lazyinit-0.0.3/.git/objects/65/
+-r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/65/1f8be5881c19639f37ff5dea35133eab4d8250
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.244900 lazyinit-0.0.3/.git/objects/67/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/67/bf3997c2bc19d4034bd741ab9808c86b52376b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.245060 lazyinit-0.0.3/.git/objects/69/
+-r--r--r--   0 dengyifan   (501) staff       (20)      930 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.245225 lazyinit-0.0.3/.git/objects/6a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1554 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.245390 lazyinit-0.0.3/.git/objects/6b/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.245713 lazyinit-0.0.3/.git/objects/6c/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1966 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66
+-r--r--r--   0 dengyifan   (501) staff       (20)      233 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/6c/f23ede6f0221263856d80f2287298ce360df0d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.245863 lazyinit-0.0.3/.git/objects/6d/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/6d/8911d55f9896b814e9db65f2edc1da1524c03b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.246020 lazyinit-0.0.3/.git/objects/6e/
+-r--r--r--   0 dengyifan   (501) staff       (20)       37 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/6e/30ca1116ed7b5e804a19fc761a7a2d58c0e1dd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.246345 lazyinit-0.0.3/.git/objects/6f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      496 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/6f/9a4b893df9fff8b3995e4014388ba30f129cd2
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/6f/cdcf4e30a9697c1f5aceaf1dc7d39d98739f51
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.246657 lazyinit-0.0.3/.git/objects/73/
+-r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/73/58417a5d41c0ae3f227f79be64cff1341921f3
+-r--r--r--   0 dengyifan   (501) staff       (20)      737 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/73/ddeb46272ee036799c78fb7748411ffef6da2a
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.247062 lazyinit-0.0.3/.git/objects/74/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/74/453505ab7b002053a991e77614b41494aefd94
+-r--r--r--   0 dengyifan   (501) staff       (20)      180 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/74/94617eb236a96a42041354b497fb373ff69e2a
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/74/e45b20bcfa13204500b46f9b3f794a2eedd610
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.247324 lazyinit-0.0.3/.git/objects/7e/
+-r--r--r--   0 dengyifan   (501) staff       (20)      336 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/7e/c698da62500825d9d6cba8fec1d0179d3c5de9
+-r--r--r--   0 dengyifan   (501) staff       (20)      499 2023-07-25 11:33:45.000000 lazyinit-0.0.3/.git/objects/7e/cdeefbee966a2c48b1f3e93aef8772a83a927b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.247467 lazyinit-0.0.3/.git/objects/7f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/7f/3aff99db09db5b9be0eb49dfbb83e5a2b2dfe6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.247618 lazyinit-0.0.3/.git/objects/80/
+-r--r--r--   0 dengyifan   (501) staff       (20)      561 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.247932 lazyinit-0.0.3/.git/objects/83/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:41:16.000000 lazyinit-0.0.3/.git/objects/83/410ee7dbb23a43716f77560dfb52b6dbab167b
+-r--r--r--   0 dengyifan   (501) staff       (20)     7437 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.248099 lazyinit-0.0.3/.git/objects/84/
+-r--r--r--   0 dengyifan   (501) staff       (20)      281 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/84/32f5170b60379a5440d18af5c42da0c20bab36
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.248256 lazyinit-0.0.3/.git/objects/86/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 08:16:23.000000 lazyinit-0.0.3/.git/objects/86/305819935ba7c71d91c90bb164a58e855e7d1e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.248405 lazyinit-0.0.3/.git/objects/87/
+-r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 08:16:23.000000 lazyinit-0.0.3/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.248549 lazyinit-0.0.3/.git/objects/88/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3155 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.248700 lazyinit-0.0.3/.git/objects/89/
+-r--r--r--   0 dengyifan   (501) staff       (20)       34 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/89/fe87522f1d1d21fb72f29e4a3f3044b32cc64c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.248855 lazyinit-0.0.3/.git/objects/8b/
+-r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 08:16:23.000000 lazyinit-0.0.3/.git/objects/8b/538f3380f85f22fc479f2298de08af638d91f6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.249008 lazyinit-0.0.3/.git/objects/8f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/8f/821694556aac2a278c288de223659193dd2489
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.249142 lazyinit-0.0.3/.git/objects/91/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2328 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.249401 lazyinit-0.0.3/.git/objects/96/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3726 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/96/7c51d6a0690049febfd310c0257eb795caeaef
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.249534 lazyinit-0.0.3/.git/objects/99/
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/99/aee23747e74ecbb3e8ebdc64b65c85c55f51dd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.249923 lazyinit-0.0.3/.git/objects/9c/
+-r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef
+-r--r--r--   0 dengyifan   (501) staff       (20)     2012 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/9c/a267b4612588367daa875d4f23cb8458c21e03
+-r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/9c/fa0e1bf241048b8a143c7fef01067d5f9c3ac7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.250196 lazyinit-0.0.3/.git/objects/9d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      150 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/9d/1f61df1650e8ae0165c5d3e1f47e8384a76e25
+-r--r--r--   0 dengyifan   (501) staff       (20)     2983 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.250594 lazyinit-0.0.3/.git/objects/a0/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/a0/2c8ecffe863e22a9a7510d5af5f8472da012c4
+-r--r--r--   0 dengyifan   (501) staff       (20)      494 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/a0/8ceea5fa60b6a189bf2ca3e11a3e82d84375ea
+-r--r--r--   0 dengyifan   (501) staff       (20)     1903 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.250934 lazyinit-0.0.3/.git/objects/a1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:33:45.000000 lazyinit-0.0.3/.git/objects/a1/e2f9a9114e1b772f7fb22f7c2a26fc8fcf25ac
+-r--r--r--   0 dengyifan   (501) staff       (20)     2165 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.251107 lazyinit-0.0.3/.git/objects/a3/
+-r--r--r--   0 dengyifan   (501) staff       (20)      555 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.251532 lazyinit-0.0.3/.git/objects/a8/
+-r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:33:45.000000 lazyinit-0.0.3/.git/objects/a8/8453b2586a082782d165b46444353c6fda84f5
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.252079 lazyinit-0.0.3/.git/objects/a9/
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-28 04:10:06.000000 lazyinit-0.0.3/.git/objects/a9/7852c14503686493d3218632fbbb52dd42628b
+-r--r--r--   0 dengyifan   (501) staff       (20)      557 2023-07-28 04:10:06.000000 lazyinit-0.0.3/.git/objects/a9/95569e1ac0accec5b1acc68f0ab077023bc4f4
+-r--r--r--   0 dengyifan   (501) staff       (20)     1465 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.252574 lazyinit-0.0.3/.git/objects/aa/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/aa/2f814ba87b54003ea2facaf8a8ac437b174212
+-r--r--r--   0 dengyifan   (501) staff       (20)      920 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487
+-r--r--r--   0 dengyifan   (501) staff       (20)     1811 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.252740 lazyinit-0.0.3/.git/objects/ad/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3750 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.253084 lazyinit-0.0.3/.git/objects/ae/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/ae/99dcc87c6ca438bd127b06eee3ccc47f4ffd6c
+-r--r--r--   0 dengyifan   (501) staff       (20)      215 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/ae/ca62bc1646058816f9a5bddd5681d0fb939b24
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.253583 lazyinit-0.0.3/.git/objects/af/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/af/272c05462dae29b6aadb455022bdbbf9f531e7
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/af/38c03c42f711bbfe4db00e49e92fb5761c80d7
+-r--r--r--   0 dengyifan   (501) staff       (20)     1602 2023-07-26 06:54:32.000000 lazyinit-0.0.3/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.253885 lazyinit-0.0.3/.git/objects/b0/
+-r--r--r--   0 dengyifan   (501) staff       (20)     4121 2023-07-26 05:00:09.000000 lazyinit-0.0.3/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/b0/8c7ef81a8076086a4529e40583d52ff2e03d24
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.254029 lazyinit-0.0.3/.git/objects/b1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      729 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.254178 lazyinit-0.0.3/.git/objects/b4/
+-r--r--r--   0 dengyifan   (501) staff       (20)      124 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/b4/31ec69865aa69f6bbac9893d5f3266ecd13273
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.256438 lazyinit-0.0.3/.git/objects/b6/
+-r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/b6/9f632da541ff48fd18a636d74fca4d80935113
+-r--r--r--   0 dengyifan   (501) staff       (20)       20 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/b6/fc4c620b67d95f953a5c1c1230aaab5db5a1b0
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.256605 lazyinit-0.0.3/.git/objects/b7/
+-r--r--r--   0 dengyifan   (501) staff       (20)      500 2023-07-25 11:16:46.000000 lazyinit-0.0.3/.git/objects/b7/8ccba97db82f1ca4c6db7e0b5cd1bd8af07780
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.258394 lazyinit-0.0.3/.git/objects/b9/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/b9/0686ac668cc417b91f372b51c3a15920445b29
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.258617 lazyinit-0.0.3/.git/objects/bb/
+-r--r--r--   0 dengyifan   (501) staff       (20)       31 2023-07-26 06:54:32.000000 lazyinit-0.0.3/.git/objects/bb/b84aa70c64fb0114dfa2f1df1cfffbc0123de9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.259341 lazyinit-0.0.3/.git/objects/bc/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/bc/771507d6ab55b2ca55d1b567dc38064561aa6f
+-r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01
+-r--r--r--   0 dengyifan   (501) staff       (20)     2346 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385
+-r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-25 11:41:16.000000 lazyinit-0.0.3/.git/objects/bc/e5df5b3fb9303de75d9ba662475c2e0940387e
+-r--r--r--   0 dengyifan   (501) staff       (20)      200 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/bc/ed2eb0d31276a7b1ddfe5855190dc53fec2a91
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.259493 lazyinit-0.0.3/.git/objects/c1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/c1/b6c43ce95f33b1c96bb259fd2c2facd4406ef8
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.259625 lazyinit-0.0.3/.git/objects/c4/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2032 2023-07-25 11:33:45.000000 lazyinit-0.0.3/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.260868 lazyinit-0.0.3/.git/objects/c5/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/c5/4ad76a5bccb99831a7a16f98637da3903c2cec
+-r--r--r--   0 dengyifan   (501) staff       (20)      450 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/c5/f23c1c12745e22b14c79b57d397ae6685cf564
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.261083 lazyinit-0.0.3/.git/objects/c7/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1654 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.261234 lazyinit-0.0.3/.git/objects/c9/
+-r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.261374 lazyinit-0.0.3/.git/objects/ca/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1263 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.261966 lazyinit-0.0.3/.git/objects/cc/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/cc/3a12d725fdd1884f2f104e1c11d8b87c1367cc
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/cc/46e850693cec9659b52d57dd78d6f60c242ebb
+-r--r--r--   0 dengyifan   (501) staff       (20)      716 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.262541 lazyinit-0.0.3/.git/objects/cd/
+-r--r--r--   0 dengyifan   (501) staff       (20)     5189 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591
+-r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 06:54:32.000000 lazyinit-0.0.3/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.262688 lazyinit-0.0.3/.git/objects/ce/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/ce/3694e653f842cc70a8c5ef32cd9f75639bb14a
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.262841 lazyinit-0.0.3/.git/objects/d2/
+-r--r--r--   0 dengyifan   (501) staff       (20)      163 2023-07-28 04:10:06.000000 lazyinit-0.0.3/.git/objects/d2/99be9b16073ba179c8b1558984116cd0eb9f3b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.262992 lazyinit-0.0.3/.git/objects/d9/
+-r--r--r--   0 dengyifan   (501) staff       (20)     5194 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.263289 lazyinit-0.0.3/.git/objects/da/
+-r--r--r--   0 dengyifan   (501) staff       (20)      116 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/da/34810fd3a6a883dbaf24d1123d0c38468460a5
+-r--r--r--   0 dengyifan   (501) staff       (20)      491 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/da/9fd18a499c0821bea6c2313d252a1d4bcf5846
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.263443 lazyinit-0.0.3/.git/objects/de/
+-r--r--r--   0 dengyifan   (501) staff       (20)      100 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/de/8f446f94a50f937fed1c254a966f3ed6088e81
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.263591 lazyinit-0.0.3/.git/objects/df/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1977 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.263737 lazyinit-0.0.3/.git/objects/e4/
+-r--r--r--   0 dengyifan   (501) staff       (20)      149 2023-07-25 14:00:51.000000 lazyinit-0.0.3/.git/objects/e4/632035cac16d026cc02de90ae31aef87867116
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.273971 lazyinit-0.0.3/.git/objects/e6/
+-r--r--r--   0 dengyifan   (501) staff       (20)       15 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.274495 lazyinit-0.0.3/.git/objects/e8/
+-r--r--r--   0 dengyifan   (501) staff       (20)      556 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b
+-r--r--r--   0 dengyifan   (501) staff       (20)     1289 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.274774 lazyinit-0.0.3/.git/objects/eb/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/eb/758cdc0fe911d913b208b48ee0ac14886927eb
+-r--r--r--   0 dengyifan   (501) staff       (20)      566 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.274920 lazyinit-0.0.3/.git/objects/ec/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/ec/47fd64ca8d46a3a1c345708cf6dd4b19e2d7a6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.275277 lazyinit-0.0.3/.git/objects/ef/
+-r--r--r--   0 dengyifan   (501) staff       (20)      219 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/ef/0a2b00e7e0280dfe13a94d5abfeeba9aafabae
+-r--r--r--   0 dengyifan   (501) staff       (20)      517 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/ef/cd52b6011e351ce3a00aa0473feeb8b10fe43d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.275581 lazyinit-0.0.3/.git/objects/f0/
+-r--r--r--   0 dengyifan   (501) staff       (20)     8516 2023-07-26 04:07:28.000000 lazyinit-0.0.3/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c
+-r--r--r--   0 dengyifan   (501) staff       (20)      433 2023-07-24 06:27:07.000000 lazyinit-0.0.3/.git/objects/f0/b6b75cf9a30d91dab0d80449c7c76a0191d8a7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.275727 lazyinit-0.0.3/.git/objects/f1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      559 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.275868 lazyinit-0.0.3/.git/objects/f2/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/f2/f3ccb260633b09276ccaaa358ce7df1a0025f6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.276008 lazyinit-0.0.3/.git/objects/f5/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 14:32:29.000000 lazyinit-0.0.3/.git/objects/f5/96444b272664dff576dc8ac874152f461a4f6e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.276149 lazyinit-0.0.3/.git/objects/f6/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2002 2023-07-26 03:36:35.000000 lazyinit-0.0.3/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.229722 lazyinit-0.0.3/.git/refs/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.276297 lazyinit-0.0.3/.git/refs/heads/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-29 00:34:07.000000 lazyinit-0.0.3/.git/refs/heads/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.229773 lazyinit-0.0.3/.git/refs/remotes/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.276562 lazyinit-0.0.3/.git/refs/remotes/origin/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-29 00:34:13.000000 lazyinit-0.0.3/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-29 00:34:10.000000 lazyinit-0.0.3/.git/refs/remotes/origin/master
+-rw-r--r--   0 dengyifan   (501) staff       (20)       17 2023-07-26 05:01:41.000000 lazyinit-0.0.3/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      424 2023-07-31 02:35:28.286148 lazyinit-0.0.3/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      184 2023-07-29 00:34:01.000000 lazyinit-0.0.3/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.277545 lazyinit-0.0.3/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.3/lazyinit/__init__.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.278758 lazyinit-0.0.3/lazyinit/__pycache__/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      179 2023-07-27 12:30:23.000000 lazyinit-0.0.3/lazyinit/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)    10748 2023-07-27 12:30:23.000000 lazyinit-0.0.3/lazyinit/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3763 2023-07-25 04:13:11.000000 lazyinit-0.0.3/lazyinit/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3874 2023-07-31 02:35:22.000000 lazyinit-0.0.3/lazyinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8543 2023-07-31 02:35:09.000000 lazyinit-0.0.3/lazyinit/init.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.282138 lazyinit-0.0.3/lazyinit/lazydl/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-07-23 08:07:15.000000 lazyinit-0.0.3/lazyinit/lazydl/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.282257 lazyinit-0.0.3/lazyinit/lazydl/configs/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1375 2023-07-29 00:33:21.000000 lazyinit-0.0.3/lazyinit/lazydl/configs/default_config.yaml
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.230300 lazyinit-0.0.3/lazyinit/lazydl/configs/exps/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.282577 lazyinit-0.0.3/lazyinit/lazydl/configs/exps/exp1/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3903 2023-07-25 13:51:05.000000 lazyinit-0.0.3/lazyinit/lazydl/configs/exps/exp1/baseline.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1152 2023-07-29 00:31:59.000000 lazyinit-0.0.3/lazyinit/lazydl/configs/exps/exp1/exp_plan.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1179 2023-07-23 08:16:18.000000 lazyinit-0.0.3/lazyinit/lazydl/minist.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)       16 2023-07-23 08:07:15.000000 lazyinit-0.0.3/lazyinit/lazydl/requirements.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2727 2023-07-23 08:07:15.000000 lazyinit-0.0.3/lazyinit/lazydl/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-24 14:38:46.000000 lazyinit-0.0.3/lazyinit/lazydl/start.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.284166 lazyinit-0.0.3/lazyinit/ranger/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6148 2023-07-24 04:18:46.000000 lazyinit-0.0.3/lazyinit/ranger/.DS_Store
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)       23 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.285174 lazyinit-0.0.3/lazyinit/ranger/colorschemes/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/colorschemes/__init__.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      139 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/colorschemes/__init__.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     5769 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/colorschemes/default.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      696 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/colorschemes/jungle.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1171 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/colorschemes/snow.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1335 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/colorschemes/snow.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4929 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/colorschemes/zenburn.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4758 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/commands.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.285928 lazyinit-0.0.3/lazyinit/ranger/plugins/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/plugins/__init__.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      134 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/plugins/__init__.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    10718 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/plugins/devicons.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     6817 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/plugins/devicons.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      479 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/plugins/devicons_linemode.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1271 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/plugins/devicons_linemode.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    23026 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/rc-sample.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    18894 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/rc.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    13012 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/rifle.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    10000 2023-07-23 10:15:36.000000 lazyinit-0.0.3/lazyinit/ranger/scope.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.3/lazyinit/redis.conf
+-rw-r--r--   0 dengyifan   (501) staff       (20)      142 2023-07-27 04:35:53.000000 lazyinit-0.0.3/lazyinit/redis.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-29 00:29:59.000000 lazyinit-0.0.3/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6724 2023-07-27 11:48:11.000000 lazyinit-0.0.3/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-31 02:35:28.278342 lazyinit-0.0.3/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      424 2023-07-31 02:35:28.000000 lazyinit-0.0.3/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)    11165 2023-07-31 02:35:28.000000 lazyinit-0.0.3/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-31 02:35:28.000000 lazyinit-0.0.3/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-31 02:35:28.000000 lazyinit-0.0.3/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-31 02:35:28.000000 lazyinit-0.0.3/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-31 02:35:28.000000 lazyinit-0.0.3/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1059 2023-07-23 12:54:16.000000 lazyinit-0.0.3/push.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-31 02:35:28.286371 lazyinit-0.0.3/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      843 2023-07-31 02:35:26.000000 lazyinit-0.0.3/setup.py
```

### Comparing `lazyinit-0.0.29/.git/hooks/commit-msg.sample` & `lazyinit-0.0.3/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/hooks/fsmonitor-watchman.sample` & `lazyinit-0.0.3/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/hooks/pre-commit.sample` & `lazyinit-0.0.3/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/hooks/pre-push.sample` & `lazyinit-0.0.3/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/hooks/pre-rebase.sample` & `lazyinit-0.0.3/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/hooks/pre-receive.sample` & `lazyinit-0.0.3/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/hooks/prepare-commit-msg.sample` & `lazyinit-0.0.3/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/hooks/push-to-checkout.sample` & `lazyinit-0.0.3/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/hooks/update.sample` & `lazyinit-0.0.3/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/index` & `lazyinit-0.0.3/.git/index`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/logs/HEAD` & `lazyinit-0.0.3/.git/logs/HEAD`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/logs/refs/heads/master` & `lazyinit-0.0.3/.git/logs/refs/heads/master`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/logs/refs/remotes/origin/HEAD` & `lazyinit-0.0.3/.git/logs/refs/remotes/origin/HEAD`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/logs/refs/remotes/origin/master` & `lazyinit-0.0.3/.git/logs/refs/remotes/origin/master`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063` & `lazyinit-0.0.3/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9` & `lazyinit-0.0.3/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6` & `lazyinit-0.0.3/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/08/ea4e268e6f806a7f000c9ae9f7d48f4a770cd9` & `lazyinit-0.0.3/.git/objects/08/ea4e268e6f806a7f000c9ae9f7d48f4a770cd9`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead` & `lazyinit-0.0.3/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/0b/9c91dcf98edb3b3bf9ab9474944a29b6868823` & `lazyinit-0.0.3/.git/objects/0b/9c91dcf98edb3b3bf9ab9474944a29b6868823`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d` & `lazyinit-0.0.3/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae` & `lazyinit-0.0.3/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/27/1af1abadcaf261f7305ee5239e60d63a2a49ac` & `lazyinit-0.0.3/.git/objects/27/1af1abadcaf261f7305ee5239e60d63a2a49ac`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8` & `lazyinit-0.0.3/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34` & `lazyinit-0.0.3/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/31/93627be78d312d8aca9e6da7d9d2aad6a5b1d3` & `lazyinit-0.0.3/.git/objects/31/93627be78d312d8aca9e6da7d9d2aad6a5b1d3`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d` & `lazyinit-0.0.3/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3` & `lazyinit-0.0.3/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7` & `lazyinit-0.0.3/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3` & `lazyinit-0.0.3/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9` & `lazyinit-0.0.3/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd` & `lazyinit-0.0.3/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd` & `lazyinit-0.0.3/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb` & `lazyinit-0.0.3/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d` & `lazyinit-0.0.3/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1` & `lazyinit-0.0.3/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b` & `lazyinit-0.0.3/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f` & `lazyinit-0.0.3/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084` & `lazyinit-0.0.3/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4` & `lazyinit-0.0.3/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04` & `lazyinit-0.0.3/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66` & `lazyinit-0.0.3/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/73/ddeb46272ee036799c78fb7748411ffef6da2a` & `lazyinit-0.0.3/.git/objects/73/ddeb46272ee036799c78fb7748411ffef6da2a`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86` & `lazyinit-0.0.3/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25` & `lazyinit-0.0.3/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717` & `lazyinit-0.0.3/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c` & `lazyinit-0.0.3/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c` & `lazyinit-0.0.3/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0` & `lazyinit-0.0.3/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef` & `lazyinit-0.0.3/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/9c/a267b4612588367daa875d4f23cb8458c21e03` & `lazyinit-0.0.3/.git/objects/9c/a267b4612588367daa875d4f23cb8458c21e03`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e` & `lazyinit-0.0.3/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd` & `lazyinit-0.0.3/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083` & `lazyinit-0.0.3/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d` & `lazyinit-0.0.3/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875` & `lazyinit-0.0.3/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/a9/95569e1ac0accec5b1acc68f0ab077023bc4f4` & `lazyinit-0.0.3/.git/objects/a9/95569e1ac0accec5b1acc68f0ab077023bc4f4`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b` & `lazyinit-0.0.3/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487` & `lazyinit-0.0.3/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477` & `lazyinit-0.0.3/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb` & `lazyinit-0.0.3/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76` & `lazyinit-0.0.3/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45` & `lazyinit-0.0.3/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c` & `lazyinit-0.0.3/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01` & `lazyinit-0.0.3/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385` & `lazyinit-0.0.3/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893` & `lazyinit-0.0.3/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586` & `lazyinit-0.0.3/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd` & `lazyinit-0.0.3/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d` & `lazyinit-0.0.3/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c` & `lazyinit-0.0.3/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591` & `lazyinit-0.0.3/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943` & `lazyinit-0.0.3/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac` & `lazyinit-0.0.3/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463` & `lazyinit-0.0.3/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b` & `lazyinit-0.0.3/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e` & `lazyinit-0.0.3/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23` & `lazyinit-0.0.3/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/ef/cd52b6011e351ce3a00aa0473feeb8b10fe43d` & `lazyinit-0.0.3/.git/objects/ef/cd52b6011e351ce3a00aa0473feeb8b10fe43d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c` & `lazyinit-0.0.3/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb` & `lazyinit-0.0.3/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91` & `lazyinit-0.0.3/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/__pycache__/utils.cpython-311.pyc` & `lazyinit-0.0.3/lazyinit/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/__pycache__/utils.cpython-38.pyc` & `lazyinit-0.0.3/lazyinit/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/bash_config.txt` & `lazyinit-0.0.3/lazyinit/bash_config.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# >>> zhei-init >>>
+# >>> lazyinit >>>
 
 tn() {
   tmux new -s "$@"
 }
 
 tk(){
   tmux kill-session -t "$@"
@@ -127,8 +127,8 @@
 # Bash 主题
 PS1='\[\033[0;31m\]\342\224\214\342\224\200$([[ $? != 0 ]] && echo "[\[\033[0;31m\]\342\234\227\[\033[0;37m\]\[\033[0;31m\]]")\[\033[0;31m\][\[\033[0;39m\]\[\e[0;33;40m\]\@\[\033[01;33m\]\[\e[0;95;40m\]-->\[\033[01;96m\]\u\[\033[0;31m\]]\342\224\200[\[\033[0;32m\]\w\[\033[0;31m\]]\n\[\033[0;31m\]\342\224\224\342\224\200\342\224\200\342\225\274 \[\033[0m\]\[\e[01;33m\]>\[\e[0m\]'
 
 # Add an "alert" alias for long running commands.  Use like so:
 #   sleep 10; alert
 alias alert='notify-send --urgency=low -i "$([ $? = 0 ] && echo terminal || echo error)" "$(history|tail -n1|sed -e '\''s/^\s*[0-9]\+\s*//;s/[;&|]\s*alert$//'\'')"'
 
-# >>> zhei-init >>>
+# >>> lazyinit >>>
```

### Comparing `lazyinit-0.0.29/lazyinit/init.py` & `lazyinit-0.0.3/lazyinit/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     python_version = "3.9"
     env_name = "lazydl"
 
     # 读取 ~/.bashrc 文件内容
     if not os.path.exists("~/.bashrc"):
         run_cmd("touch ~/.bashrc", show_cmd=False)
     bashrc = run_cmd("cat ~/.bashrc", show_cmd=False)
-    if "lazydl-init" not in bashrc:
-        print("未找到 lazydl-init 配置，即将注入配置到 ~/.bashrc（完成后可能需要重启初始化工具）")
+    if "lazyinit" not in bashrc:
+        print("未找到 lazyinit 配置，即将注入配置到 ~/.bashrc（完成后可能需要重启初始化工具）")
         # ---------------------------------------------------------------------------- #
         #                         配置 Bash 环境变量                                     
         # ---------------------------------------------------------------------------- #
         bash = [
             "cd ~/",
             "cat {}/bash_config.txt >> ~/.bashrc".format(pkg_current_path),
         ]
```

### Comparing `lazyinit-0.0.29/lazyinit/lazydl/configs/default_config.yaml` & `lazyinit-0.0.3/lazyinit/lazydl/configs/default_config.yaml`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/lazydl/configs/exps/exp1/baseline.yaml` & `lazyinit-0.0.3/lazyinit/lazydl/configs/exps/exp1/baseline.yaml`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/lazydl/configs/exps/exp1/exp_plan.yaml` & `lazyinit-0.0.3/lazyinit/lazydl/configs/exps/exp1/exp_plan.yaml`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/lazydl/minist.py` & `lazyinit-0.0.3/lazyinit/lazydl/minist.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/lazydl/run.py` & `lazyinit-0.0.3/lazyinit/lazydl/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/.DS_Store` & `lazyinit-0.0.3/lazyinit/ranger/.DS_Store`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/colorschemes/default.py` & `lazyinit-0.0.3/lazyinit/ranger/colorschemes/default.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/colorschemes/jungle.py` & `lazyinit-0.0.3/lazyinit/ranger/colorschemes/jungle.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/colorschemes/snow.py` & `lazyinit-0.0.3/lazyinit/ranger/colorschemes/snow.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/colorschemes/snow.pyo` & `lazyinit-0.0.3/lazyinit/ranger/colorschemes/snow.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/colorschemes/zenburn.py` & `lazyinit-0.0.3/lazyinit/ranger/colorschemes/zenburn.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/commands.py` & `lazyinit-0.0.3/lazyinit/ranger/commands.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/plugins/devicons.py` & `lazyinit-0.0.3/lazyinit/ranger/plugins/devicons.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/plugins/devicons.pyo` & `lazyinit-0.0.3/lazyinit/ranger/plugins/devicons.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/plugins/devicons_linemode.pyo` & `lazyinit-0.0.3/lazyinit/ranger/plugins/devicons_linemode.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/rc-sample.conf` & `lazyinit-0.0.3/lazyinit/ranger/rc-sample.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/rc.conf` & `lazyinit-0.0.3/lazyinit/ranger/rc.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/rifle.conf` & `lazyinit-0.0.3/lazyinit/ranger/rifle.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/ranger/scope.sh` & `lazyinit-0.0.3/lazyinit/ranger/scope.sh`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/redis.conf` & `lazyinit-0.0.3/lazyinit/redis.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/run.py` & `lazyinit-0.0.3/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit/utils.py` & `lazyinit-0.0.3/lazyinit/utils.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/lazyinit.egg-info/SOURCES.txt` & `lazyinit-0.0.3/lazyinit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/push.sh` & `lazyinit-0.0.3/push.sh`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.29/setup.py` & `lazyinit-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.29',
+    version='0.0.3',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init lazydl environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

